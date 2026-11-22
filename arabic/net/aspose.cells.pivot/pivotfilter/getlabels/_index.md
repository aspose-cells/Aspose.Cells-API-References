---
title: "PivotFilter.GetLabels"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة PivotFilter. يحصل على ملصقات فلتر العنوان"
type: docs
url: /ar/net/aspose.cells.pivot/pivotfilter/getlabels/
---
## PivotFilter.GetLabels method

يحصل على تسميات مرشح التسمية.

```csharp
public string[] GetLabels()
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotFilterMethodGetLabelsDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // إنشاء بنية جدول محور صالحة
                worksheet.Cells["A1"].Value = "Category";
                worksheet.Cells["A2"].Value = "A";
                worksheet.Cells["A3"].Value = "B";
                worksheet.Cells["A4"].Value = "A";
                
                // إنشاء جدول محوري باستخدام المعلمات الصحيحة
                int pivotIndex = worksheet.PivotTables.Add("A1:A4", "C3", "PivotTable1");
                PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
                
                // إنشاء فلتر محور بمعلمات صالحة
                int filterIndex = pivotTable.PivotFilters.Add(0, PivotFilterType.CaptionEqual);
                PivotFilter pivotFilter = pivotTable.PivotFilters[filterIndex];

                // تكوين خصائص الفلتر
                pivotFilter.Name = "SampleFilter";
                pivotFilter.EvaluationOrder = 1;

                // تنفيذ طريقة GetLabels
                string[] labels = pivotFilter.GetLabels();

                Console.WriteLine($"Retrieved {labels?.Length ?? 0} labels:");
                if (labels != null)
                {
                    foreach (string label in labels)
                    {
                        Console.WriteLine($"- {label}");
                    }
                }

                workbook.Save("GetLabelsDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling GetLabels: {ex.Message}");
            }
        }
    }
}
```

### انظر أيضًا

* class [PivotFilter](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


