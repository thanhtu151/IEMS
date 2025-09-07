```
Mục tiêu: đọc dữ liệu từ cảm biến, gửi ra CSV/JSON qua serial hoặc MQTT.
Gợi ý cấu trúc thư mục:
iot/
├─ firmware/
│  └─ esp32_energy.ino      # ESP32 code đọc sensor, tính công suất
├─ scripts/
│  ├─ log_serial.py         # Python: đọc serial, ghi CSV
│  ├─ mqtt_pub.py           # Publish data lên MQTT broker
│  └─ mqtt_sub.py           # Subscribe data, lưu DB
└─ data/
   └─ samples/              # CSV mẫu: time, voltage, current, power
```
