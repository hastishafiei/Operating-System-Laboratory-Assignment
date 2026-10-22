## سوال 1:
<div dir="rtl" align="right">
  با خواندن man grep، آپشنی را پیدا کنید که کار grep| wc-l را به تنهایی انجام دهد(یعنی فقط تعداد تطابق ها را در خروجی نمایش دهد)

  
</div>
<img src="https://github.com/hastishafiei/Operating-System-Laboratory-Assignment/blob/main/hw3-q1.jpg" width="750">
<div dir="rtl" align="right"> 

</div>





## سوال 2:

<div dir="rtl" align="right">
  دستوری بنویسید که تمام فایلهای با پسوند .conf را در کل دایرکتوری /etc و زیرشاخه های آن را پیدا کند به صورت بازگشتی. 
با استفاده از دستور

</div>
<div dir="ltr" align="left">
  find /etc -type f -name "*.conf"
</div>
</div>
<img src="https://github.com/hastishafiei/Operating-System-Laboratory-Assignment/blob/main/hw3-q2.jpg" width="750">
<div dir="rtl" align="right"> 



## سوال 3:

<div dir="rtl" align="right">
شما یک فایل بزرگ به نام `data.csv` دارید. با ترکیب دستورات `head` و `tail` (با پایپ `|`)، کاری کنید که دقیقاً فقط خط ۱۰۰۰ تا خط ۱۰۱۰ روی صفحه چاپ شود.
</div>
<img src="https://github.com/hastishafiei/Operating-System-Laboratory-Assignment/blob/main/hw3-q3.jpg" width="750">
<div dir="rtl" align="right"> 
 head -n 1010 data.csv | tail -n 10
   

با استفاده از دستور بالا به این صورت که ابتدا با head 1010 خط اول را دریافت میکنیم و سپس با پایپ خروجی را به tail میدهیم و tail نیز از 1010خط، 10 خط اخر را نمایش میدهد. 
</div> 

