Nginx 
=====


Install Nginx webserver - optionally - along with SSL certificate.

Role Variables
--------------

- `ssl` - copies SSL certificate; default: False
- `cert` - path to public certificate
- `cert_key` - path to private SSL key


Example Playbook
----------------

    - hosts: servers
      roles:
         - role: nginx_base
           ssl: yes
           cert: ./example.com.cert
           cert_key: ./example.com.key

License
-------

BSD
