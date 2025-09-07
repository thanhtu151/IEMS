```
Mục tiêu: xử lý CSV/stream dữ liệu, phân tích & dự báo.
Gợi ý cấu trúc thư mục:
ai/
├─ app/
│  ├─ main.py              # FastAPI app (endpoint /ai/*)
│  ├─ routers/
│  │   ├─ summary.py       # /ai/summary: tổng hợp kWh theo ngày/giờ
│  │   ├─ forecast.py      # /ai/forecast: dự báo tiêu thụ
│  │   └─ anomaly.py       # /ai/anomaly: phát hiện bất thường
│  ├─ services/
│  │   ├─ stats.py         # Trung bình, min, max
│  │   ├─ moving_avg.py    # Dự báo bằng MA
│  │   ├─ zscore.py        # Phát hiện bất thường
│  │   └─ utils.py         # Đọc CSV, format JSON
│  └─ data/
│      └─ samples/         # CSV test
├─ requirements.txt        # pandas, numpy, scikit-learn, fastapi
└─ .env.example            # DB_URL, MQTT_URL...
```
