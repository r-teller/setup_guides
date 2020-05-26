This setup guide will assume you already have the following setup

- BIG-IP Initial configuration with virtual-server listening on HTTPS and a valid license for BIG-IP Access
  - Initial config docs &rarr; https://techdocs.f5.com/en-us/bigip-15-1-0/big-ip-system-initial-configuration.html
- NGINX JQ,NGINX and NGINX-NJS module installed
  - Installing NGINX+ &rarr; https://docs.nginx.com/nginx/admin-guide/installing-nginx/installing-nginx-plus/ 
  - Installing NGINX-NodeJS &rarr; https://docs.nginx.com/nginx/admin-guide/dynamic-modules/nginscript/ 
- NGINX & OpenID Connect: This document is based on this example setup &rarr;  https://github.com/nginxinc/nginx-openid-connect


<!-- deployed and completed the initial configuration and NGINX+ installed -->
<!-- 
-- Example topology goes here --

- BIG-IP Configuration (Example was based on BIG-IP v15)
-- This example will use a localDB for Authentication, for your deployment you can use any authentication method supported by F5 APM
https://techdocs.f5.com/en-us/bigip-15-1-0/big-ip-access-policy-manager-authentication-methods.html

-JWT Token
--Create Certificate
---oauthCert_federate.acmefinancial.net
--Create JWT Key
---Note:When creating the key it must have the ID field filled out, without it the oAuth profile will not be able to select it from the drop down list
--Create JWT Token
-oAuth Claims
--company/email/first/last
-Client Application
--Note: Pay close attention to port in Redirect URI
-Resource Server
-oAuth Profile
--Note: Highlight changes
-APM Profile
--Note:Since this is a demo notice the fields are populated dynamically



-- Create Access Profile
--- Select OAuth-Resource Server
--- Specify the supported languages

 -->
