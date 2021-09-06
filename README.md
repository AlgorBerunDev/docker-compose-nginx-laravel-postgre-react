# docker-compose-nginx-laravel-postgre-react
This is a laravel 5.8, PostgreSQL, Nginx and React builded project with docker-compose.

# docker-compose-nginx-laravel-postgres
docker-compose,  Nginx, Laravel
## Base configure
- mkdir src
- cd ./src && composer create-project laravel/laravel
- npm init react-app frontend
- cd frontend && npm install
- npm run build
- cd ../../ && docker-compose up -d

## Nginx urls
- File links /uploads/* and /src/frontend/build
- File uploaded paths /src/storage/app/public/
- /api/* redirected to laravel project
- /* redirected to react build project (react build project path: /src/frontend/build) 
