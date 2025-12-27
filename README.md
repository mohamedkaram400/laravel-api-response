# Laravel API Response

A simple and reusable API response trait for Laravel applications.  
It helps you return consistent JSON responses across your APIs.

## ✨ Features

- Unified JSON response structure
- Custom message and HTTP status code
- Optional pagination support
- Lightweight and easy to use

## 📦 Installation

```bash
composer require mohamedkaram500/laravel-api-response
```

## 🚀 Usage
```bash
use MohamedKaram500\LaravelApiResponse\Traits\ApiResponseTrait;

class UserController extends Controller
{
    use ApiResponseTrait;

    public function index()
    {
        return $this->apiResponse(
            'Users fetched successfully',
            200,
            ['users' => []]
        );
    }
}
```

## Response Format
```bash
{
  "message": "Success message",
  "status_code": 200,
  "data": {},
  "pagination": {}
}
```


## 🧑‍💻 Author
### Mohamed Karam
Backend Developer | Laravel

## 📄 License
This project is open-source and licensed under the MIT License.
