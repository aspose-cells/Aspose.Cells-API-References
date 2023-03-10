---
title: طريقة set_header
second_title: Aspose.Cells for Python via .NET API المراجع
description:
type: docs
weight: 200
url: /ar/python-net/aspose.cells/pagesetup/set_header/
is_root: false
---
##  set_header(section, header_script) {#int-str}
يعيّن برنامج نصي بتنسيق رأس ملف Excel.



```python
def set_header(self, section, header_script):
    ...
```


| معامل| يكتب| وصف|
| :- | :- | :- |
| section | int | 0: القسم الأيسر ، 1: القسم الأوسط ، 2: القسم الأيمن.|
| header_script | str | برنامج نصي بتنسيق الرأس.|
###  ملاحظات

أوامر البرنامج النصي:

| يأمر| وصف|
| :- | :- |
| & ص| رقم الصفحة الحالية|
| &ن| عدد الصفحات|
| &د| التاريخ الحالي|
| & ت| الوقت الحالي|
| &أ| اسم الورقة|
| &F| اسم الملف بدون مسار|
| &"<FontName>"| اسم الخط ، على سبيل المثال: & "Arial"|
| &"<FontName>, <FontStyle>"| اسم الخط ونمطه ، على سبيل المثال: & "Arial، Bold"|
| &<FontSize>| حجم الخط. إذا كان هذا الأمر متبوعًا برقم عادي ليتم طباعته في الرأس ، فسيتم فصله عن ارتفاع الخط بحرف مسافة.|
| &ك<RRGGBB>|لون الخط ، على سبيل المثال (أحمر): & KFF0000|
| & ج| نص الصورة|

على سبيل المثال: "& Arial، Bold & 8Header Note"


###  أنظر أيضا
* وحدة [aspose.cells](../../)
* فئة [PageSetup](/cells/ar/python-net/aspose.cells/pagesetup)
