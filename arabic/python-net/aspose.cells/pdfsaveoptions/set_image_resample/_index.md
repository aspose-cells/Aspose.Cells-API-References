---
title: طريقة set_image_resample
second_title: Aspose.Cells for Python via .NET API المراجع
description:
type: docs
weight: 20
url: /ar/python-net/aspose.cells/pdfsaveoptions/set_image_resample/
is_root: false
---
##  set_image_resample(desired_ppi, jpeg_quality) {#int-int}
 يضبط PPI المطلوب (بكسل لكل بوصة) لإعادة تشكيل الصور وجودة jpeg.
 سيتم تحويل جميع الصور إلى JPEG بإعداد الجودة المحدد ،
والصور التي تكون أكبر من PPI المحدد (بكسل لكل بوصة) سيتم إعادة تشكيلها.



```python
def set_image_resample(self, desired_ppi, jpeg_quality):
    ...
```


| معامل| يكتب| وصف|
| :- | :- | :- |
| desired_ppi | int | وحدات البكسل المرغوبة في البوصة. 220 جودة عالية. 150 شاشة بجودة. 96 جودة البريد الإلكتروني.|
| jpeg_quality | int | 0-100٪ JPEG الجودة.|

###  مثال

تحدد الكود التالي PPI المطلوب بجودة 96 و jpeg على 80 للصور في ملف pdf الناتج.

```python
from aspose.cells import PdfSaveOptions, Workbook

# load the source file with images.
wb = Workbook("Book1.xlsx")
pdfSaveOptions = PdfSaveOptions()
# set desired PPI as 96 and jpeg quality as 80.
pdfSaveOptions.set_image_resample(96, 80)
wb.save("output.pdf", pdfSaveOptions)

```



###  أنظر أيضا
* وحدة [aspose.cells](../../)
* فئة [PdfSaveOptions](/cells/ar/python-net/aspose.cells/pdfsaveoptions)
