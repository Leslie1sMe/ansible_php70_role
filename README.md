PHP7.0 role
=========

Help u easily build php7.0 on Ubuntu.


Role Variables
--------------


---

 pkg_item: 
 
所需要安装版本的php和扩展
   - php7.0
   - php-pear
   - php7.0-dev
  
  安装php-pear和php7.0-dev,解锁使用pecl，安装扩展更方便。
   - php7.0-mbstring
   - php7.0-zip
   - php7.0-mysql
  
  日常所需要的扩展，可以在vars/main.yml中自定义添加
  
  配置文件路径：
  
 php_ini: /etc/ansible/roles/php/templates/php.ini.j2
 
 修改站点根目录index.php文件,查看phpinfo，安装成功.
 
 
 php_index: /etc/ansible/roles/php/templates/index.php.j2`
`

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      roles:
         - { role: username.rolename}

License
-------

BSD


