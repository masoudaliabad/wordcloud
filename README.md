# wordcloud
Persian review sentiment analysis using DistilBERT + Google Translate | تحلیل احساسات نظرات فارسی
# تحلیل احساسات نظرات فارسی 💬

پروژه‌ای برای تحلیل احساسات متن فارسی با استفاده از ترجمه خودکار و مدل Transformers

---

## درباره پروژه

در این پروژه نظرات فارسی کاربران (از فایل CSV) خوانده می‌شود، با Google Translate به انگلیسی ترجمه می‌شود و سپس توسط مدل DistilBERT از HuggingFace تحلیل احساسات انجام می‌شود. نتیجه به صورت مثبت یا منفی با درصد اطمینان نمایش داده می‌شه.

---

## ویژگی‌های پروژه

- تحلیل احساسات متن فارسی بدون نیاز به مدل فارسی
- ترجمه خودکار فارسی به انگلیسی با Google Translator
- استفاده از مدل پیش‌آموزش‌دیده DistilBERT
- ساخت ابر کلمات (WordCloud) از نظرات فارسی
- نمایش نتیجه با ایموجی و درصد اطمینان

---

## نمونه خروجی

```
😊 100 %   ← نظر مثبت
😔 99 %    ← نظر منفی
```

---

## مراحل پروژه

**1. ساخت WordCloud فارسی**
- خواندن متن فارسی
- نرمال‌سازی فارسی
- حذف stop words از فایل stopwords.txt
- ذخیره تصویر wordcloud

**2. ترجمه متن فارسی**
- استفاده از کتابخانه deep_translator
- ترجمه خودکار فارسی به انگلیسی با Google Translate

**3. تحلیل احساسات**
- بارگذاری مدل DistilBERT از HuggingFace
- تحلیل هر نظر پس از ترجمه
- نمایش برچسب مثبت یا منفی با درصد

**4. تحلیل دیتاست نظرات**
- خواندن نظرات از فایل CSV
- تحلیل تک‌تک نظرات
- ساخت WordCloud از مجموع نظرات

---

## نتیجه روی دیتاست

اکثر نظرات با اطمینان بالای **95% تا 100%** مثبت تشخیص داده شدند که با محتوای واقعی نظرات مطابقت دارد.

---

## تکنولوژی‌های استفاده شده

- Python
- HuggingFace Transformers (DistilBERT)
- deep_translator (Google Translate)
- wordcloud_fa (ابر کلمات فارسی)
- Pandas
- Matplotlib

---

## نحوه نصب

```bash
pip install transformers deep-translator wordcloud-fa pandas matplotlib
```

---

## نحوه اجرا

فایل CSV نظرات را با ستون `nazaar` آماده کنید، سپس notebook را اجرا کنید.

---

## سازنده

[masoudaliabad](https://github.com/masoudaliabad)
