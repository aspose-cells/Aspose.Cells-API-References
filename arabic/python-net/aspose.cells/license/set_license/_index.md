---
title: طريقة set_license
second_title: Aspose.Cells for Python via .NET API المراجع
description:
type: docs
weight: 20
url: /ar/python-net/aspose.cells/license/set_license/
is_root: false
---
##  set_license(license_name) {#str}
تراخيص المكونات.



```python
def set_license(self, license_name):
    ...
```


| حدود| يكتب| وصف|
| :- | :- | :- |
| license_name | str |  |
###  ملاحظات

حاول العثور على الترخيص في المواقع التالية:


1. مسار صريح.


2. المجلد الذي يحتوي على تجميع المكون Aspose.


3. المجلد الذي يحتوي على تجميع استدعاء العميل.


4. المجلد الذي يحتوي على دخول (بدء التشغيل) التجمع.


5. مورد مضمن في تجميع استدعاء العميل.


**ملحوظات:** في .NET Compact Framework ، يحاول العثور على الترخيص في هذه المواقع فقط:


1. مسار صريح.


2. مورد مضمن في تجميع استدعاء العميل.
###  أمثلة


في هذا المثال ، سيتم إجراء محاولة للعثور على ملف ترخيص باسم MyLicense.lic
 في المجلد الذي يحتوي على


المكون ، في المجلد الذي يحتوي على التجميع المتصل ،
في مجلد تجميع الإدخال ثم في الموارد المضمنة للتجميع المتصل.

```python
from aspose.cells import License

license = License()
license.set_license("MyLicense.lic")

```
يمكن أن يكون اسم ملف كامل أو قصير أو اسم مورد مضمن.
استخدم سلسلة فارغة للتبديل إلى وضع التقييم.


##  set_license(stream) {#io.RawIOBase}
تراخيص المكونات.



```python
def set_license(self, stream):
    ...
```


| حدود| يكتب| وصف|
| :- | :- | :- |
| stream | io.RawIOBase | دفق يحتوي على الترخيص.|
###  ملاحظات

استخدم هذه الطريقة لتحميل ترخيص من دفق.
###  أمثلة


```python
from aspose.cells import License

license = License()
license.set_license(myStream)

```



###  أنظر أيضا
* وحدة [aspose.cells](../../)
* فئة [License](/cells/ar/python-net/aspose.cells/license)
