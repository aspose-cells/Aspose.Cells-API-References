---
title: "GridPdfSaveOptions.SetImageResample"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة GridPdfSaveOptions. تعيين عدد النقاط في البوصة (PPI) المطلوب للصور المعاد أخذ عيناتها وجودة JPEG. سيتم تحويل جميع الصور إلى JPEG باستخدام إعداد الجودة المحدد، وستُعاد أخذ عينات الصور التي تكون أكبر من عدد النقاط في البوصة المحدد"
type: docs
url: /ar/net/aspose.cells.griddesktop.data/gridpdfsaveoptions/setimageresample/
---
## GridPdfSaveOptions.SetImageResample method

يضبط قيمة PPI (بكسل لكل بوصة) المطلوبة لإعادة تحجيم الصور وجودة JPEG. سيتم تحويل جميع الصور إلى JPEG باستخدام إعداد الجودة المحدد، وستتم إعادة تحجيم الصور التي تتجاوز قيمة PPI المحددة (بكسل لكل بوصة).

```csharp
public void SetImageResample(int desiredPPI, int jpegQuality)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| desiredPPI | Int32 | البكسلات المطلوبة لكل بوصة. 220 جودة عالية. 150 جودة الشاشة. 96 جودة البريد الإلكتروني. |
| jpegQuality | Int32 | 0 - 100% جودة JPEG. |

### أمثلة

الكود التالي يحدد عدد النقاط في البوصة المطلوب إلى 96 وجودة JPEG إلى 80 للصور في ملف PDF الناتج.

```csharp
//حمّل ملف المصدر مع الصور.
Workbook wb = new Workbook("Book1.xlsx");

PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();

//حدد عدد النقاط في البوصة إلى 96 وجودة JPEG إلى 80.
pdfSaveOptions.SetImageResample(96, 80);

wb.Save("output.pdf", pdfSaveOptions);
```

### انظر أيضًا

* class [GridPdfSaveOptions](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)


