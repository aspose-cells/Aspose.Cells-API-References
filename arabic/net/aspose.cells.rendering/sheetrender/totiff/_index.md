---
title: ToTiff
second_title: Aspose.Cells لمرجع .NET API
description: عرض ورقة العمل بأكملها كصورة Tiff للتدفق .
type: docs
weight: 80
url: /ar/net/aspose.cells.rendering/sheetrender/totiff/
---
## ToTiff(Stream) {#totiff}

عرض ورقة العمل بأكملها كصورة Tiff للتدفق .

```csharp
public void ToTiff(Stream stream)
```

| معامل | يكتب | وصف |
| --- | --- | --- |
| stream | Stream | تيار الصورة الناتجة |

### أنظر أيضا

* class [SheetRender](../../sheetrender)
* مساحة الاسم [Aspose.Cells.Rendering](../../sheetrender)
* المجسم [Aspose.Cells](../../../)

---

## ToTiff(string) {#totiff_1}

عرض ورقة العمل بأكملها على هيئة Tiff Image إلى ملف.

```csharp
public void ToTiff(string filename)
```

| معامل | يكتب | وصف |
| --- | --- | --- |
| filename | String | اسم ملف الصورة الناتجة |

### أمثلة

تقوم الكود التالي بإخراج كافة صفحات الورقة الأولى إلى صورة Tiff.

```csharp
// تحميل الملف المصدر بالصور.
Workbook wb = new Workbook("Book1.xlsx");

ImageOrPrintOptions imgOpt = new ImageOrPrintOptions();

// تعيين نوع صورة الإخراج.
imgOpt.SaveFormat = SaveFormat.Tiff;

// تقديم الورقة الأولى.
SheetRender sr = new SheetRender(wb.Worksheets[0], imgOpt);

// إخراج جميع صفحات الورقة إلى صورة Tiff.
sr.ToTiff("output.tiff");
```

### أنظر أيضا

* class [SheetRender](../../sheetrender)
* مساحة الاسم [Aspose.Cells.Rendering](../../sheetrender)
* المجسم [Aspose.Cells](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
