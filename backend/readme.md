"""Thiết kế & quản lý database (Postgres hoặc Supabase).

Viết API để IoT gửi dữ liệu vào, AI/Web đọc dữ liệu ra.

Xử lý ETL: đảm bảo dữ liệu từ IoT → DB sạch, đúng định dạng.

Hỗ trợ AI và Web bằng các query/endpoint tối ưu.

data/
├─ app/
│  ├─ main.py          # FastAPI app cho backend
│  ├─ routers/
│  │   ├─ ingest.py    # API nhận dữ liệu từ IoT
│  │   ├─ query.py     # API cho Web (lấy logs, summary cơ bản)
│  │   └─ health.py    # check service
│  ├─ models/
│  │   └─ power_log.py # ORM model (SQLAlchemy/Prisma)
│  ├─ db.py            # Kết nối Postgres
│  └─ utils.py         # Validate, parse dữ liệu
├─ migrations/         # Lưu schema (Alembic/Prisma migration)
├─ requirements.txt    # fastapi, psycopg2, sqlmodel, pydantic
└─ .env.example        # DATABASE_URL, MQTT_URL
"""
