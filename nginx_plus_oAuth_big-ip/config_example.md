# BIG-IP
Reference https://clouddocs.f5.com/training/community/iam/html/class2/class2.html
Access > Profiles/Policies > Create
- Name = oAuth_to_NGINX-Plus
- Profile Type = All
- Languages = [English]

# NGINX
OpenID configuration is based on https://github.com/nginxinc/nginx-openid-connect
Reference https://www.nginx.com/blog/validating-oauth-2-0-access-tokens-nginx/

```bash
./configure.sh \
    -x \
    -i 1010250281fcef1771d83f2848d906b8368c4ce300c7a95e \
    -s 1b91b8740a5b959a9bc17bce9945e703cbdceead76e306b8368c4ce3e4eea95e \
    "https://oauth.acmefinancial.net/f5-oauth2/v1/.well-known/openid-configuration"
```