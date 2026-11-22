---
title: "ImageOrPrintOptions.IsFontSubstitutionCharGranularity"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ImageOrPrintOptions. تشير إلى ما إذا كان يجب استبدال خط الحرف فقط عندما يكون خط الخلية غير متوافق معه"
type: docs
url: /ar/net/aspose.cells.rendering/imageorprintoptions/isfontsubstitutionchargranularity/
---
## ImageOrPrintOptions.IsFontSubstitutionCharGranularity property

يشير إلى ما إذا كان يجب استبدال خط الحرف فقط عندما يكون خط الخلية غير متوافق معه.

```csharp
public bool IsFontSubstitutionCharGranularity { get; set; }
```

### ملاحظات

القيمة الافتراضية هي false. سنحاول أولاً خط دفتر العمل الافتراضي و PdfSaveOption/system لخط الخلية.

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing; // Added missing namespace AsposeCellsExamples
    using Aspose.Cells.Rendering;
    using System;

    public class ImageOrPrintOptionsPropertyIsFontSubstitutionCharGranularityDemo
    {
        public static void Run()
        {
            // إنشاء مصنف جديد والوصول إلى الورقة الأولى
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // قم بتكوين الخلية بخط قد لا يكون مدعومًا
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Text with unavailable font");
            Style style = cell.GetStyle();
            style.Font.Name = "NonExistentFont";
            cell.SetStyle(style);

            // إنشاء خيارات تصيير الصورة
            ImageOrPrintOptions options = new ImageOrPrintOptions
            {
                ImageType = ImageType.Png, // Namespace reference now valid
                DefaultFont = "Arial",
                CheckWorkbookDefaultFont = false
            };

            // اعرض وقم بتعديل قيمة الخاصية
            Console.WriteLine($"Initial IsFontSubstitutionCharGranularity: {options.IsFontSubstitutionCharGranularity}");
            
            // اعرض باستخدام الإعداد الافتراضي
            new SheetRender(worksheet, options).ToImage(0, "BeforeFontSubstitutionChange.png");

            // غيّر الخاصية وأعد العرض مرة أخرى
            options.IsFontSubstitutionCharGranularity = true;
            Console.WriteLine($"Updated IsFontSubstitutionCharGranularity: {options.IsFontSubstitutionCharGranularity}");
            new SheetRender(worksheet, options).ToImage(0, "AfterFontSubstitutionChange.png");

            // احفظ المصنف للرجوع إليه
            workbook.Save("FontSubstitutionDemoWorkbook.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


