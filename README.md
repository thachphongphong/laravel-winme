#build
- docker build -t laravel-winme .

#defaut
- docker run -p 80:80 -p 443:443 -d laravel-winme

#mount with exist code in app code:
- docker run -p 80:80 -p 443:443 -v D:/WINME/code-winme/:/var/www/laravel/ -d laravel-winme

#custom port
- docker run -p 8080:80 -p 8443:443 -v D:/WINME/code-winme/:/var/www/laravel/ -d laravel-winme

# comand line:
- composer create-project --prefer-dist laravel/laravel blog
