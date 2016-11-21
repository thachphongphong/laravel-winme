README
- docker build -t laravel-winme .

#defaut
- docker run -p 80:80 -p 443:443 -d laravel-winme

#mount with exist code in app code: /home/linhdo/myapp/
- docker run -p 80:80 -p 443:443 -v /Users/linhdo/WORKSPACES/blog/app/:/var/www/laravel/app/ -v /Users/linhdo/WORKSPACES/blog/app/public/:/var/www/laravel/public/ -d laravel-winme

#custom port
- docker run -p 8080:80 -p 8443:443 -v /Users/linhdo/WORKSPACES/blog/app/:/var/www/laravel/app/ -v /Users/linhdo/WORKSPACES/blog/public/:/var/www/laravel/public/ -d laravel-winme