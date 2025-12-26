## سوال 1:
<div dir="rtl" align="right">
  PID اولین فرآیندی که در سیستم شما اجرا میشود (معروف به init یا systemd). چیست و چرا این فرآیند والد تمام فرآیندهای دیگر محسوب میشود؟
 میتوان گفت که PID یک شماره منحصر به فرد که سیستم عامل به هر فرآیند اختصاص میدهد.
  PID 1 اولین فرآیندی است که بعد از بوت توسط کرنل اجرا می‌شود 
و چون همهٔ فرآیندها به‌صورت درختی ایجاد می‌شوند، ریشهٔ این درخت PID 1 است و والد تمام فرایند های دیگر محسوب میشود.
</div>

## سوال 2:
<div dir="rtl" align="right">
 با استفاده از man kill یا kill -l، شماره سیگنال SIGTSTP (معادل Ctrl+Z) چیست؟
</div>

<div dir="rtl" align="right">
 با استفاده از دستور kill -l، شماره سیگنال SIGTSTP معادل 20 است.
</div>

## سوال 3:

<div dir="rtl" align="right">
 تفاوت اصلی بین سیگنال SIGTERM (که kill به صورت پیشفرض میفرستد) و SIGKILL (سیگنال شماره ۹) چیست؟ در چه شرایطی از SIGKILL استفاده میکنیم؟ 
</div>

<div dir="rtl" align="right">
  SIGTERM : سیگنال پیشفرض دستور kill. یک درخواست محترمانه برای خاتمه دادن 
به فرآیند است و به آن اجازه میدهد کارهای پاکسازی نهایی را انجام دهد. 
</div>

<div dir="rtl" align="right">
  SIGKILL : یک دستور قتل فوری است. فرآیند بلافاصله و بدون فرصت 
پاکسازی، از بین میرود و این آخرین راه حل است.  
</div>

<div dir="rtl" align="right">
از SIGKILL زمانی استفاده می‌کنیم که یک فرآیند به SIGTERM پاسخ ندهد و دچار هنگ یا بن‌بست (deadlock) شده باشد، یا به‌صورت غیرعادی در حال مصرف کردن منابعی مانند CPU یا RAM باشد. 
</div>

## سوال 4:

<div dir="rtl" align="right">
  تفاوت اصلی بین دو دستور زیر چیست؟ 


cat file.txt | grep "word"

grep "word" file.txt 

(راهنمایی: هر دو یک کار را انجام میدهند، اما یکی از آنها یک فرآیند اضافه و غیرضروری ایجاد میکند. به این حالت "Useless Use of cat" میگویند).  
</div>

</div>

<div dir="rtl" align="right">
ابتدا با cat file.txt فایل را میخوانیم و خروجی را از طریق pipe به grep میفرستیم تا کلمه word را پیدا کند اما با grep "word" file.txt، دستور grep مستقیماً فایل را می‌خواند و همان کار را با یک فرآیند کمتر انجام میدهد بنابراین میتوان گفت که دستور cat یک کار اضافه تر انجام میدهد به همین جهت useless است. 
</div>

## سوال 5:

<div dir="rtl" align="right">
دستوری بنویسید که تمام پیغامهای مربوط به کرنل سیستم را (با دستور dmesg) گرفته، فقط خطوطی که شامل کلمه error یا fail هستند را فیلتر کرده و نتیجه را در فایلی به نام kernel_errors.log ذخیره کند. 
</div>

<div dir="rtl" align="right">
با استفاده از دستور

   dmesg | grep -Ei "error|fail" > kernel_errors.log
</div>

<div dir="rtl" align="right">
<img src="https://raw.githubusercontent.com/hastishafiei/Operating-System-Laboratory-Assignment/main/pic5.1.jpg" width="750">
</div>

## سوال 6:
<div dir="rtl" align="right">
 دستور tr چیست و چه کاری انجام میدهد؟ (با man tr تحقیق کنید). یک مثال از ترکیب tr ،cat و sort با استفاده از pipe ارائه دهید.  
 
</div>

<div dir="rtl" align="right">
چیزی که man tr نوشته است:
  
 
   Translate,  squeeze,  and/or  delete  characters from standard input, writing to standard output.  STRING1 and STRING2 specify arrays of characters ARRAY1 and ARRAY2 that control the action.

   
  یعنی عمل ترجمه مثل فشرده سازی حذف کاراکتر ها از ورودی را انجام میدهد و در خروجی نمایش میدهد به عنوان مثال
  
</div>
<div dir="rtl" align="right">

<img src="https://raw.githubusercontent.com/hastishafiei/Operating-System-Laboratory-Assignment/main/pic5.2.jpg" width="750">
</div>







