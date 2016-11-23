#build
- docker build -t laravel-winme .

#defaut
- docker run -p 80:80 -p 443:443 -d laravel-winme

#mount with exist code in app code: /Users/linhdo/WORKSPACES/blog/
- docker run -p 80:80 -p 443:443 -v D:/WINME/code-winme/app/:/var/www/laravel/app/ -v  D:/WINME/code-winme/public/:/var/www/laravel/public/ -d laravel-winme

#custom port
- docker run -p 8080:80 -p 8443:443 -v D:/WINME/code-winme/app/:/var/www/laravel/app/ -v  D:/WINME/code-winme/public/:/var/www/laravel/public/ -d laravel-winme

# Anh chạy linux nên cài laravel qua comand line:
- composer create-project --prefer-dist laravel/laravel blog