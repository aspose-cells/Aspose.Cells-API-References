---
title: "ValidationCollection.GetValidationInCell"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة ValidationCollection. تحصل على التحقق المطبق على الخلية المعطاة"
type: docs
url: /ar/net/aspose.cells/validationcollection/getvalidationincell/
---
## ValidationCollection.GetValidationInCell method

يحصل على التحقق المطبق على الخلية المعطاة.

```csharp
public Validation GetValidationInCell(int row, int column)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| صف | Int32 | فهرس الصف. |
| عمود | Int32 | فهرس العمود. |

### قيمة الإرجاع

تُرجع كائن [`Validation`](../../validation/) أو null إذا لم يكن هناك تحقق للخلية المعطاة

### أمثلة

```csharp
using System;
using System.Text;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ValidationCollectionMethodGetValidationInCellWithInt32Int32Demo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف التحقق من صحة البيانات إلى الخلية A1 (0,0)
            Validation validation = worksheet.Validations[worksheet.Validations.Add()];
            validation.Type = ValidationType.List;
            validation.Formula1 = "\"Option1,Option2,Option3\"";
            
            // إنشاء CellArea مع StartRow، StartColumn، EndRow، EndColumn
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.StartColumn = 0;
            area.EndRow = 0;
            area.EndColumn = 0;
            validation.AddArea(area);

            // احصل على التحقق من الصحة من الخلية A1 (0,0)
            Validation validationInCell = worksheet.Validations.GetValidationInCell(0, 0);
            
            if (validationInCell != null && validationInCell.Type == ValidationType.List)
            {
                Console.WriteLine("Cell A1 has list validation with formula: " + validationInCell.Formula1);
            }
        }
    }
}
```

### انظر أيضًا

* class [Validation](../../validation/)
* class [ValidationCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


