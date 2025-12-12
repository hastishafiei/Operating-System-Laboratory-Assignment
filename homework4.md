## سوال 1:

<div dir="rtl" align="right">
مجوز rwxr-x--- معادل چه عددی در سیستم Octal است؟
</div>



<div dir="rtl" align="right">
rwxr-x---  معادل عددی 075
  </div>

R=4   w=2    x=1

---=0+0+0=0

rwx=4+2+1=7   

r-x=4+1=5

## سوال 2:


<div dir="rtl" align="right">
دستوری بنویسید که مجوز اجرای یک اسکریپت به نام deploy.sh را فقط از گروه آن حذف کند، بدون اینکه مجوزهای دیگر تغییر کند.


با استفاده از دستور chmod g-x deploy.sh
  
</div>


<div dir="rtl" align="right">
  
<img src="https://raw.githubusercontent.com/hastishafiei/Operating-System-Laboratory-Assignment/main/homework4-q2.png" width="750">

</div>


## سوال 3:
<div dir="rtl" align="right">

اگر umask سیستم 0027 باشد، مجوز پیشفرض برای یک فایل جدید و یک دایرکتوری جدید چه خواهد بود؟ (به صورت نمادین rwx و عددی بنویسید).

750=777-027 برای دایرکتوری --- rwx r-x

640=666-027 برای فایل         --- --rw-  r  

به عنوان مثال برای فایل مجوز کاربران 6 است یعنی اجازه خواندن و نوشتن را دارند 

 و ماسک ما برای کاربران 7 است یعنی باید اجازه خواندن و نوشتن و اجرا رو از کاربران بگیریم 
 
ماسک مجوز خواندن و نوشتن را میگیرد و اجازه اجرا هم که از ابتدا نداشت پس جواب صفر میشود.



</div>










