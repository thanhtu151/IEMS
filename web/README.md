```
Mục tiêu: web cho người dùng cuối xem dữ liệu điện năng & AI insights.
Gợi ý cấu trúc thư mục:
web/
├─ app/                        # Next.js App Router
│  ├─ dashboard/page.tsx       # Tổng quan (charts: power, energy)
│  ├─ upload/page.tsx          # Upload CSV test
│  ├─ insights/page.tsx        # Kết quả AI (forecast, anomaly)
│  └─ api/                     # (tùy chọn) proxy gọi AI API
├─ lib/
│  ├─ api.ts                   # Gọi API AI service
│  └─ utils.ts                 # Format dữ liệu
├─ components/
│  ├─ charts/PowerChart.tsx    # Biểu đồ điện năng theo thời gian
│  ├─ charts/ForecastChart.tsx # Biểu đồ dự báo
│  └─ ui/                      # Table, Card, Button
├─ public/                     # Logo, icon
├─ prisma/ (nếu có DB)         # Schema Postgres
├─ package.json
└─ README.md
```
