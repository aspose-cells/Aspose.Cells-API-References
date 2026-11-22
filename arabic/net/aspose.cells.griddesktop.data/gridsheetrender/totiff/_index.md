---
title: "GridSheetRender.ToTiff"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة GridSheetRender. عرض كامل ورقة العمل كصورة Tiff إلى الدفق"
type: docs
url: /ar/net/aspose.cells.griddesktop.data/gridsheetrender/totiff/
---
## ToTiff(Stream) {#totiff}

عرض كامل ورقة العمل كصورة Tiff إلى تدفق.

```csharp
public void ToTiff(Stream stream)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| تدفق | Stream | تدفق الصورة الناتجة |

### انظر أيضًا

* class [GridSheetRender](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)

---

## ToTiff(string) {#totiff_1}

عرض كامل ورقة العمل كصورة Tiff إلى ملف.

```csharp
public void ToTiff(string filename)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| اسم الملف | String | اسم ملف الصورة الناتجة |

### أمثلة

الكود التالي يُخرج جميع صفحات الورقة الأولى إلى صورة Tiff.

```csharp
//حمّل ملف المصدر مع الصور.
Workbook wb = new Workbook("Book1.xlsx");

ImageOrPrintOptions imgOpt = new ImageOrPrintOptions();

//تعيين نوع صورة الإخراج.
imgOpt.SaveFormat = SaveFormat.Tiff;

//عرض الورقة الأولى.
SheetRender sr = new SheetRender(wb.Worksheets[0], imgOpt);

//إخراج جميع صفحات الورقة إلى صورة Tiff.
sr.ToTiff("output.tiff");
```

### انظر أيضًا

* class [GridSheetRender](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)


