# https-to-http-redirect
Use this piece of code to redirect from https to http or www to http in the htaccess of a website.

`<IfModule mod_rewrite.c>
  RewriteEngine On
  RewriteCond %{HTTP_HOST} ^https://sangamadhikari.com.np$ [OR]
  RewriteCond %{HTTP_HOST} ^www.sangamadhikari.com.np$
  RewriteRule (.*)$ http://sangamadhikari.com.np/$1 [R=301,L]
</IfModule>`
