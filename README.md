# PostgreSQL Assignment

This repository contains the complete SQL code for table creation, sample data insertion, and problem-based queries as part of the PostgreSQL lab assignment.

## 📁 File Structure

- `PostgreSQL_Assignment.sql`: Contains SQL code for:
  - Table creation
  - Data insertion
  - Problem-solving queries with appropriate comments

---

##  PostgreSQL Theory Questions

### ১️⃣ PostgreSQL কী?

PostgreSQL একটি ওপেন-সোর্স, অবজেক্ট-রিলেশনাল ডেটাবেস ম্যানেজমেন্ট সিস্টেম (ORDBMS)। এটি শক্তিশালী, নির্ভরযোগ্য এবং উন্নত ফিচার সমৃদ্ধ একটি ডেটাবেস যা জটিল অ্যাপ্লিকেশন ও বিশ্লেষণের জন্য ব্যবহৃত হয়।

---

### ২️⃣ PostgreSQL-এ Schema-এর কাজ কী?

একটি স্কিমা হল একটি নির্দিষ্ট নেমস্পেস বা গোষ্ঠী যা ডেটাবেসের টেবিল, ভিউ, ফাংশন ইত্যাদিকে সাজিয়ে রাখে। এটি ডেটাকে সংগঠিত ও আলাদা রাখার জন্য ব্যবহার হয়, একই ডেটাবেসে একাধিক স্কিমা থাকতে পারে।

---

### ৩️⃣ Primary Key এবং Foreign Key কী?

- **Primary Key**: টেবিলের প্রতিটি রেকর্ডকে ইউনিকভাবে শনাক্ত করতে ব্যবহৃত হয়। এটি কখনো NULL হতে পারে না।
- **Foreign Key**: অন্য একটি টেবিলের Primary Key কে রেফারেন্স করে। এটি টেবিলগুলোর মধ্যে সম্পর্ক তৈরি করে এবং ডেটার ইন্টিগ্রিটি বজায় রাখে।

---



### ৪️⃣ SELECT স্টেটমেন্টে WHERE ক্লজের উদ্দেশ্য কী?

`WHERE` ক্লজ ব্যবহার করে ডেটাবেস থেকে নির্দিষ্ট শর্ত অনুযায়ী রেকর্ড ফিল্টার করা যায়। এটি ডেটা রিড করার সময় কনডিশন অ্যাপ্লাই করতে সাহায্য করে।

উদাহরণ:
```sql
SELECT * FROM species WHERE conservation_status = 'Endangered';

---
## ৫️ GROUP BY কী এবং এটি কী কাজে ব্যবহৃত হয়?
GROUP BY ক্লজ ব্যবহার করে ডেটাগুলোকে নির্দিষ্ট কলামের মান অনুযায়ী গ্রুপ করা যায় এবং প্রতিটি গ্রুপের উপর অ্যাগ্রিগেট ফাংশন যেমন COUNT(), SUM() প্রয়োগ করা যায়।

উদাহরণ:SELECT ranger_id, COUNT(*) FROM sightings GROUP BY ranger_id;

---
৬️ VARCHAR এবং CHAR-এর মধ্যে পার্থক্য কী?
VARCHAR(n): পরিবর্তনশীল দৈর্ঘ্যের স্ট্রিং সংরক্ষণ করে। এটি স্টোরেজের জন্য বেশি কার্যকর কারণ এটি অতিরিক্ত স্পেস নেয় না।

CHAR(n): নির্দিষ্ট দৈর্ঘ্যের স্ট্রিং সংরক্ষণ করে। ছোট স্ট্রিং হলে অতিরিক্ত স্পেস পূরণ করা হয়।
---