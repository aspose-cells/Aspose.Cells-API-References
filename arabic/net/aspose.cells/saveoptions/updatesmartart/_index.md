---
title: "SaveOptions.UpdateSmartArt"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية SaveOptions. تشير إلى ما إذا كان يتم تحديث إعدادات SmartArt. القيمة الافتراضية هي false"
type: docs
url: /ar/net/aspose.cells/saveoptions/updatesmartart/
---
## SaveOptions.UpdateSmartArt property

يشير إلى ما إذا كان يتم تحديث إعداد Smart Art. القيمة الافتراضية هي false.

```csharp
public bool UpdateSmartArt { get; set; }
```

### ملاحظات

يظهر التأثير فقط بعد استدعاء طريقة Shape.GetResultOfSmartArt() ووجود الأشكال المخزنة مؤقتًا في ملف القالب.

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class SaveOptionsPropertyUpdateSmartArtDemo
    {
        public static void Run()
        {
            // تحميل دفتر العمل المصدر
            Workbook workbook = new Workbook("example.xlsx");

            // تعديل الأشكال و SmartArt
            foreach (Worksheet worksheet in workbook.Worksheets)
            {
                foreach (Shape shape in worksheet.Shapes)
                {
                    shape.AlternativeText = "ReplacedAlternativeText";
                    
                    if (shape.IsSmartArt)
                    {
                        foreach (Shape smartArtShape in shape.GetResultOfSmartArt().GetGroupedShapes())
                        {
                            smartArtShape.Text = "ReplacedText";
                        }
                    }
                }
            }

            // حفظ مع تمكين UpdateSmartArt
            OoxmlSaveOptions saveOptions = new OoxmlSaveOptions();
            saveOptions.UpdateSmartArt = true;
            workbook.Save("output.xlsx", saveOptions);

            // تحقق من التغييرات
            Workbook savedWorkbook = new Workbook("output.xlsx");
            foreach (Worksheet worksheet in savedWorkbook.Worksheets)
            {
                foreach (Shape shape in worksheet.Shapes)
                {
                    Console.WriteLine($"Shape Alt Text: {shape.AlternativeText}");
                    
                    if (shape.IsSmartArt)
                    {
                        foreach (Shape smartArtShape in shape.GetResultOfSmartArt().GetGroupedShapes())
                        {
                            Console.WriteLine($"SmartArt Text: {smartArtShape.Text}");
                        }
                    }
                }
            }
        }
    }
}
```

### انظر أيضًا

* class [SaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


