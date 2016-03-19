

[![Build Status](https://travis-ci.org/ThePrudents/nginx.svg?branch=master)](https://travis-ci.org/ThePrudents/nginx)


Usage example:

roles:
     - {
         role: "pr-nginx",
         option_ssl: true,
         option_use_pregenerated_pem: true,

         nginx_sites:
           - {
             name: "default",
             config: "{{role_dir}}/templates/nginx/nginx.conf.j2"
             }
        }
 
