---
title: PageIndex
second_title: Aspose.Cells لمرجع .NET API
description: الحصول على أو تعيين فهرس للصفحة الأولى على أساس 0 للحفظ.
type: docs
weight: 250
url: /ar/net/aspose.cells/pdfsaveoptions/pageindex/
---
## PdfSaveOptions.PageIndex property

الحصول على أو تعيين فهرس للصفحة الأولى على أساس 0 للحفظ.

```csharp
public int PageIndex { get; set; }
```

### ملاحظات

القيمة الافتراضية هي 0.

### أمثلة

يوضح المثال التالي كيفية عرض نطاق من الصفحات (3 و 4) في ملف Microsoft Excel إلى PDF.

```csharp
// افتح ملف Excel
Workbook wb = new Workbook("Book1.xlsx");

PdfSaveOptions options = new PdfSaveOptions();

// اطبع الصفحة 3 والصفحة 4 فقط في ملف PDF الناتج
// فهرس صفحة البداية (فهرس قائم على 0)
options.PageIndex = 3;
// عدد الصفحات المراد طباعتها
options.PageCount = 2;

// احفظ ملف PDF
wb.Save("output.pdf", options);
```

### أنظر أيضا

* class [PdfSaveOptions](../../pdfsaveoptions)
* مساحة الاسم [Aspose.Cells](../../pdfsaveoptions)
* المجسم [Aspose.Cells](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
