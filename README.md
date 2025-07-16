# Online Course Platform (Microservices Architecture)

🎯 هدف این پروژه، ساخت یک پلتفرم فروش دوره‌های آنلاین با معماری مایکروسرویس، توسعه‌پذیر، قابل تست و مناسب برای دیپلوی production است.

## 🧱 سرویس‌ها

| سرویس      | توضیح                                 |
|------------|----------------------------------------|
| Backend    | پیاده‌سازی APIها با Django + DRF       |
| Frontend   | رابط کاربری با Next.js (React)         |
| Database   | پایگاه‌داده PostgreSQL در کانتینر جدا  |
| Reverse Proxy | اضافه خواهد شد (NGINX)              |

## ⚙️ ساختار دایرکتوری

online-course-platform/
├── docker-compose.yml
├── README.md
│
├── backend/ # Django backend
│ └── Dockerfile
│
├── frontend/ # Next.js frontend
│ └── Dockerfile
│
├── nginx/ # برای reverse proxy در آینده
│ └── nginx.conf
│
└── db/ # Volume و اسکریپت‌های اولیه DB
└── init.sql


## 🚀 اجرای اولیه با Docker

```bash
docker-compose up --build
