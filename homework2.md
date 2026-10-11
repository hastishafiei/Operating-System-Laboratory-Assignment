## سوال 1:

<div dir="rtl" align="right">
  یک ساختار دایرکتوری مانند زیر ایجاد کنید (فقط با یک دستور `mkdir`):
</div>

<div dir="rtl" align="right">

<pre>
project/
├── assets/
│   ├── css/
│   └── pages/
│   └── py/

</pre>
<img src="https://github.com/hastishafiei/Operating-System-Laboratory-Assignment/blob/main/hw2-q1.jpg" width="750">

</div>



## سوال 2:

<div dir="rtl" align="right">
یک فایل متنی به نام `info.txt` بسازید. برای آن یک هارد لینک به نام `info_h.txt` و یک سیمبولیک لینک به نام `info_s.txt` ایجاد کنید. سپس فایل `info.txt` را حذف کنید. چه اتفاقی برای دو لینک دیگر می‌افتد؟ (با `cat` محتوایشان را چک کنید.)
.
<img src="https://github.com/hastishafiei/Operating-System-Laboratory-Assignment/blob/main/hw2-q2.jpg" width="750">
 
**هارد لینک:** هنوز کار می‌کند چون مستقیماً به همان داده اشاره دارد.

**سافت لینک:** خراب می‌شود چون فقط به مسیر فایل اشاره می‌کند و آن مسیر دیگر وجود ندارد
</div>

## سوال 3:

<div dir="rtl" align="right">
با استفاده از دستور `man rm` در ترمینال، بگردید و سوییچی را پیدا گنید که برای حذف اجباری و بدون تایید استفاده میشود.
<img src="https://github.com/hastishafiei/Operating-System-Laboratory-Assignment/blob/main/hw2-q3.jpg" width="750">
 
 
آپشنی که قبل از حذف هر فایل تأیید می‌خواهد: `rm -i`

آپشنی که تأیید را غیرفعال می‌کند (`force`): `rm -f`
<img src="https://github.com/hastishafiei/Operating-System-Laboratory-Assignment/blob/main/hw2-q3-1.jpg" width="750">
</div>
