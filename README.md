# 📍 Java Tracking System  
🚀 **نظام تتبع للخريجين باستخدام Java وواجهة رسومية (GUI)**  

## 📌 مقدمة  
يهدف هذا المشروع إلى **إدارة بيانات الطلاب الخريجين** باستخدام **Java GUI و MySQL**.  
يوفر البرنامج إمكانيات مثل:  
✔️ **إضافة بيانات الخريجين**  
✔️ **تحديث البيانات المسجلة**  
✔️ **حذف الخريجين**  
✔️ **البحث عن بيانات الطلاب**  
✔️ **عرض البيانات في جدول رسومي**  

## ⚙️ المتطلبات  
قبل تشغيل المشروع، تأكد من توفر المتطلبات التالية:  
- **Java SE 8 أو أحدث**  
- **NetBeans / IntelliJ IDEA / Eclipse** (أو أي بيئة تطوير تدعم Java)  
- **MySQL Database**  
- **JDBC Driver for MySQL**  

## 🛠️ إعداد قاعدة البيانات  
1. تأكد من تثبيت **MySQL Server** وتشغيله.  
2. أنشئ قاعدة بيانات جديدة باسم `tracking_system`.  
3. استخدم ملف **SQL** لإنشاء الجدول المطلوب داخل قاعدة البيانات.  

```sql
CREATE TABLE graduatestudent (
    StudentID INT AUTO_INCREMENT PRIMARY KEY,
    Name VARCHAR(255),
    Phone VARCHAR(20),
    Address TEXT,
    Department VARCHAR(100),
    AvailabilityStatus VARCHAR(50),
    LastCommunicationDate DATE
);
