---
title: "ValidationCollection.RemoveArea"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة ValidationCollection. تزيل جميع إعدادات التحقق على النطاق"
type: docs
url: /ar/net/aspose.cells/validationcollection/removearea/
---
## ValidationCollection.RemoveArea method

يزيل جميع إعدادات التحقق على النطاق..

```csharp
public void RemoveArea(CellArea ca)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| ca | CellArea | النطاق الذي يحتوي على إعدادات التحقق. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ValidationCollectionMethodRemoveAreaDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // إنشاء تحقق في منطقة محددة
            ValidationCollection validations = worksheet.Validations;
            CellArea validationArea = CellArea.CreateCellArea(0, 0, 5, 5);
            int validationIndex = validations.Add(validationArea);
            
            // إنشاء منطقة لإزالتها من التحقق
            CellArea removeArea = CellArea.CreateCellArea(2, 2, 4, 4);
            
            try
            {
                // استدعاء طريقة RemoveArea مع معامل CellArea
                validations.RemoveArea(removeArea);
                
                Console.WriteLine("Validation area removed successfully.");
                
                // عرض مناطق التحقق المتبقية
                foreach (Validation validation in validations)
                {
                    if (validation.Areas.Length > 0)
                    {
                        Console.WriteLine($"Remaining validation area: {validation.Areas[0]}");
                    }
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing RemoveArea method: {ex.Message}");
            }
            
            // حفظ النتيجة
            workbook.Save("ValidationRemoveAreaDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* struct [CellArea](../../cellarea/)
* class [ValidationCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


