# 🚨 Real-Time Object Detection & Alert System using YOLOv11 (Raspberry Pi 4B)

A **real-time object and person detection system** powered by **YOLOv11** and deployed on a **Raspberry Pi 4B**, featuring a **dual alert mechanism**:

* 🔊 Buzzer alert (instant local warning)
* 📧 Automated email alert (remote notification)

This project combines **computer vision + IoT + automation** to create a portable and reliable surveillance solution.

---

## 📌 Features

* 🎯 Real-time object & person detection using YOLOv11
* ⚡ Fast inference with Ultralytics framework
* 🔊 Instant buzzer alert on detection
* 📧 Automated email notifications with captured image
* 🍓 Raspberry Pi 4B integration for portability
* 🔁 Continuous monitoring system
* 🧠 Smart detection filtering (person-specific alerts possible)

---

## 🖼️ Project Demo

### 📷 System Setup

![System Setup](images/setup.jpg)

### 📷 Detection Output

![Detection Output](images/detection.jpg)

### 📷 Email Alert Sample

![Email Alert](images/email_alert.png)

> 📁 Place your images inside a folder named `images/` in your repository.

---

## 🏗️ System Architecture

```plaintext
Camera Module → Raspberry Pi → YOLOv11 Model
                           ↓
                Object Detection Trigger
                   ↓             ↓
              Buzzer Alert    Email Alert
```

---

## 🛠️ Tech Stack

* **Hardware**

  * Raspberry Pi 4B
  * USB / Pi Camera
  * Buzzer Module

* **Software**

  * Python 3.x
  * Ultralytics YOLOv11
  * OpenCV
  * SMTP (Email Service)

---

## ⚙️ Installation

### 1️⃣ Clone Repository

```bash
git clone https://github.com/ARNESHA-1/RealTime-Object-Detection-and-Alert-System-using-YOLOv11--Integrated-with-Raspberry-pi4B.git
cd RealTime-Object-Detection-and-Alert-System-using-YOLOv11--Integrated-with-Raspberry-pi4B
```

### 2️⃣ Install Dependencies

```bash
pip install ultralytics opencv-python smtplib numpy
```

### 3️⃣ Setup Email Credentials

Edit your script:

```python
EMAIL_ADDRESS = "your_email@gmail.com"
EMAIL_PASSWORD = "your_app_password"
RECEIVER_EMAIL = "receiver_email@gmail.com"
```

> ⚠️ Use **App Passwords**, not your main email password.

---

## ▶️ Usage

Run the detection script:

```bash
python detect.py
```

* System starts camera feed
* Detects objects/persons in real-time
* Triggers:

  * 🔊 Buzzer (GPIO)
  * 📧 Email alert with snapshot

---



## 📊 Future Improvements

* 📱 Mobile app integration
* ☁️ Cloud storage for detections
* 🧠 Custom trained YOLO model
* 🔔 Push notifications (Telegram / WhatsApp)
* 🌙 Night vision support

---

## 🤝 Contributing

Pull requests are welcome. For major changes, please open an issue first to discuss.

---


## 👨‍💻 Author

**Your Name**
GitHub: https://github.com/ARNESHA-1

---

## ⭐ Support

If you like this project, give it a ⭐ on GitHub!
