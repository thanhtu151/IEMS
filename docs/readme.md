```
Nơi lưu trữ tài liệu học tập
Gợi ý cấu trúc thư mục:
docs/
├─ design-notes/
│  ├─ iot.md           # sơ đồ mạch, công thức P=V×I
│  ├─ ai.md            # công thức moving average, z-score
│  └─ web.md           # flow upload CSV → render → call API
├─ gpt-log/
│  ├─ iot_[name].md
│  ├─ ai_[name].md
│  └─ web_[name].md
└─ diagrams/
   ├─ system.drawio    # sơ đồ IoT→MQTT→AI→Web
   └─ dataflow.png

Note: 
Trong folder: gpt-log/

Mỗi lần dùng GPT để xin code/gợi ý → copy prompt + đoạn code → lưu "mụcđích.md".

Kèm comment: giữ gì, bỏ gì, vì sao.

PR merge phải có gpt-log-ngày .
```
