# https-to-http-redirect
Use this piece of code to redirect from https to http or www to http in the htaccess of a website.

``<IfModule mod_rewrite.c>
  RewriteEngine On
  RewriteCond %{HTTP_HOST} ^https://radhikaadhikari.com.np$ [OR]
  RewriteCond %{HTTP_HOST} ^www.radhikaadhikari.com.np$
  RewriteRule (.*)$ http://radhikaadhikari.com.np/$1 [R=301,L]
</IfModule>``
