---
title: "Workbook.MergeNamedStyles"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Workbook. يدمج الأنماط المسماة من ملف Excel الآخر"
type: docs
url: /ar/net/aspose.cells/workbook/mergenamedstyles/
---
## Workbook.MergeNamedStyles method

يدمج الأنماط المسمّاة من ملف Excel الآخر.

```csharp
public void MergeNamedStyles(Workbook source)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| المصدر | المصنف | الملف الآخر |

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodMergeNamedStylesWithWorkbookDemo
    {
        public static void Run()
        {
            // إنشاء دفتر العمل الهدف (الذي سيتلقى الأنماط المسماة)
            using (Workbook targetWorkbook = new Workbook())
            {
                // إضافة بعض البيانات إلى دفتر العمل الهدف للسياق
                Worksheet targetSheet = targetWorkbook.Worksheets[0];
                targetSheet.Cells["A1"].PutValue("Target Workbook");

                // إنشاء دفتر العمل المصدر (الذي يحتوي على الأنماط المسماة للدمج)
                using (Workbook sourceWorkbook = new Workbook())
                {
                    // إضافة بعض البيانات إلى دفتر العمل المصدر للسياق
                    Worksheet sourceSheet = sourceWorkbook.Worksheets[0];
                    sourceSheet.Cells["A1"].PutValue("Source Workbook");

                    try
                    {
                        // دمج الأنماط المسماة من sourceWorkbook إلى targetWorkbook
                        targetWorkbook.MergeNamedStyles(sourceWorkbook);

                        Console.WriteLine("MergeNamedStyles executed successfully.");

                        // احفظ دفتر العمل الناتج
                        string outputPath = "MergedNamedStylesDemo.xlsx";
                        targetWorkbook.Save(outputPath, SaveFormat.Xlsx);
                        Console.WriteLine($"Workbook saved to '{outputPath}'.");
                    }
                    catch (Exception ex)
                    {
                        Console.WriteLine($"Error during MergeNamedStyles: {ex.Message}");
                    }
                }
            }
        }
    }
}
```

### انظر أيضًا

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


