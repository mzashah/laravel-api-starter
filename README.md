# Laravel REST API Starter

A production-ready Laravel 11 REST API boilerplate with JWT authentication, role-based access control, rate limiting, and Swagger documentation.

![Laravel](https://img.shields.io/badge/Laravel-11-FF2D20?style=for-the-badge&logo=laravel)
![PHP](https://img.shields.io/badge/PHP-8.2-777BB4?style=for-the-badge&logo=php)
![MySQL](https://img.shields.io/badge/MySQL-8.0-4479A1?style=for-the-badge&logo=mysql)

## Features

- ✅ JWT Authentication (login, register, refresh, logout)
- ✅ Role & Permission system (Spatie)
- ✅ API Rate Limiting
- ✅ Request Validation
- ✅ Resource Transformers
- ✅ Swagger/OpenAPI Documentation
- ✅ File Upload handling
- ✅ Email verification
- ✅ Password reset
- ✅ Audit logging
- ✅ Docker ready

## Quick Start

```bash
git clone https://github.com/mzashah/laravel-api-starter
cd laravel-api-starter
composer install
cp .env.example .env
php artisan key:generate
php artisan jwt:secret
php artisan migrate --seed
php artisan serve
```

## API Endpoints

### Auth
- `POST /api/auth/register`
- `POST /api/auth/login`
- `POST /api/auth/logout`
- `POST /api/auth/refresh`
- `GET  /api/auth/me`

### Users
- `GET    /api/users`
- `GET    /api/users/{id}`
- `PUT    /api/users/{id}`
- `DELETE /api/users/{id}`

### Posts (Example Resource)
- `GET    /api/posts`
- `POST   /api/posts`
- `GET    /api/posts/{id}`
- `PUT    /api/posts/{id}`
- `DELETE /api/posts/{id}`

## Tech Stack

- **Framework**: Laravel 11
- **Auth**: JWT (tymon/jwt-auth)
- **Permissions**: spatie/laravel-permission
- **Docs**: darkaonline/l5-swagger
- **Testing**: PHPUnit / Pest
- **Database**: MySQL 8 / PostgreSQL

## License

MIT © [Zohaib Ali Shah](https://github.com/mzashah)
