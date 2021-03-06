---
title: Enumerations
localeTitle: التعدادات
---
# التعدادات

التعداد هو مجموعة من الثوابت الصحيحة المسماة التي يتم تعريفها باستخدام الكلمة `enum` .

## مثال

 `enum Gender 
 { 
  Male, 
  Female 
 } 
` 

بشكل افتراضي ، تبدأ قيم الأعداد الصحيحة عند 0 وتزيد بمقدار 1 ، لكل اسم تعداد أي ذكور = 0 ، أنثى = 1 إلخ.

يمكن تجاوز هذه عن طريق تحديد قيمة عدد صحيح لأي من أسماء التعداد.

## مثال

 `enum Gender 
 { 
  Male = 1, 
  Female 
 } 
` 

في هذه الحالة ، ستبدأ قيم عدد صحيح في 1 وتزيد من هناك.

لاستخدام تعداد ، يمكنك تعريف متغير من نوعه وتعيين قيمة له:

`Gender myVar = Gender.Male;`

يمكنك أيضًا إرسال قيمة اسم التعداد إلى القيمة الصحيحة الأساسية والعكس صحيح:

 `Console.WriteLine($"Male: {(int)Gender.Male}"); 
 Console.WriteLine($"Female: {(int)Gender.Female}"); 
` 

## انتاج:

 `Male: 1 
 Female: 2 
`