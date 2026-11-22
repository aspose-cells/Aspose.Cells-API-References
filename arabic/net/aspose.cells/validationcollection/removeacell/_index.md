---
title: "ValidationCollection.RemoveACell"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة ValidationCollection. تزيل جميع إعدادات التحقق من الصحة على الخلية"
type: docs
url: /ar/net/aspose.cells/validationcollection/removeacell/
---
## ValidationCollection.RemoveACell method

يزيل جميع إعدادات التحقق على الخلية.

```csharp
public void RemoveACell(int row, int column)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| صف | Int32 | فهرس الصف للخلية. |
| عمود | Int32 | فهرس العمود للخلية. |

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ValidationCollectionMethodRemoveACellWithInt32Int32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // أضف التحقق من الصحة إلى الخلية A1 (الصف 0، العمود 0)
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.StartColumn = 0;
            area.EndRow = 0;
            area.EndColumn = 0;
            
            Validation validation = worksheet.Validations[worksheet.Validations.Add(area)];
            validation.Type = ValidationType.List;
            validation.Formula1 = "Item1,Item2,Item3";

            // أزل التحقق من الصحة من الخلية A1
            worksheet.Validations.RemoveACell(0, 0);

            Console.WriteLine("Validations count after removal: " + worksheet.Validations.Count);
        }
    }
}
```

### انظر أيضًا

* class [ValidationCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


