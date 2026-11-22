---
title: "Cell.IsTableFormula"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Cell. تشير إلى ما إذا كانت هذه الخلية جزءًا من صيغة الجدول"
type: docs
url: /ar/net/aspose.cells/cell/istableformula/
---
## Cell.IsTableFormula property

يشير إلى ما إذا كانت هذه الخلية جزءًا من صيغة جدول.

```csharp
public bool IsTableFormula { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class CellPropertyIsTableFormulaDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            
            // إنشاء جدول
            int index = worksheet.ListObjects.Add(0, 0, 5, 3, true);
            ListObject table = worksheet.ListObjects[index];
            
            // إضافة صيغة جدول إلى الخلية D2
            Cell cell = worksheet.Cells["D2"];
            cell.Formula = "=SUM(Table1[[#This Row],[Column1]:[Column3]])";
            
            // تحقق مما إذا كانت الخلية تحتوي على صيغة جدول
            Console.WriteLine("Is table formula: " + cell.IsTableFormula);
            
            // احفظ المصنف
            workbook.Save("output.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### انظر أيضًا

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


