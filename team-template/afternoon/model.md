<!-- workshop-header -->
<img width="1347" height="127" alt="Coding Thailand 2026 header" src="https://github.com/user-attachments/assets/ba5cf267-f460-4fb0-b69b-c461ae061a3b" />

# Afternoon — Model

- **Input ที่ใช้:** webcam
- **Classes:** ค้อน กระดาษ กรรไกร
- **จำนวนตัวอย่าง/class:** 20 ต่อ 1 คลาส
- **วิธีเชื่อมเข้า Edge Impulse:** [x] กล้อง/ไมค์ (`edge-impulse-linux`)  [ ] Modulino (`data-forwarder`)

## V1
- Accuracy (ใน Studio): 80%
- F1 score ราย class (class : F1): 0.80
- class ที่ F1 ต่ำสุด: 0.67
- รูป Confusion Matrix: ![cm-v1](https://drive.google.com/drive/folders/10AQ8QvoRv5y1Tbc9rn6gJOV6AXaCXznz?usp=drive_link)
- อ่านแล้วเห็นอะไร (class ไหนสับสนกับ class ไหน): กรรไกรกับกระดาษสับสน 25% , ค้อนกับกระดาษสับสน 50%

## V2 (ถ้าทัน)
- แก้อะไรจาก V1: _______________
- Accuracy V2: ____  | ดีขึ้น/แย่ลงตรงไหน: _______________

## รันบนบอร์ด
- [x] วิธีรัน: [x] กล้อง/ไมค์ → `edge-impulse-linux-runner` (Web UI :4912)  [ ] Modulino → Arduino library ในสเก็ตช์
- [ ] ป้อน input จริงแล้ว prediction เปลี่ยนตาม (inferencing time: ____ ms)
- คลิป/รูปตอนรัน: ![run](../assets/run.jpg)

## (ต่อยอด) Output logic
- threshold ที่ใช้: confidence ≥ ____
- map class → output: _______________ (เช่น "เตือน" → Buzzer + Pixels แดง)
