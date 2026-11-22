---
title: "PivotField.OriginalItems"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية PivotField. احصل على العناصر الأساسية الأصلية"
type: docs
url: /ar/net/aspose.cells.pivot/pivotfield/originalitems/
---
## PivotField.OriginalItems property

احصل على العناصر الأساسية الأصلية؛

```csharp
public string[] OriginalItems { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldPropertyOriginalItemsDemo
    {
        public static void Run()
        {
            // إنشاء مصنف من ملف Excel المصدر
            Workbook workbook = new Workbook("AsposeGroupedField2.xlsx");
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            
            // الوصول إلى أول جدول محوري
            PivotTable pivotTable = worksheet.PivotTables[0];
            
            // الوصول إلى حقل الصف الأول
            PivotField pivotField = pivotTable.RowFields[0];
            
            // اعرض العناصر الأصلية والعناصر المجمعة
            Console.WriteLine("Original Item[0]: " + pivotField.OriginalItems[0]);
            Console.WriteLine("Grouped Item[0]: " + pivotField.Items[0]);
            
            // احفظ المصنف المعدل
            workbook.Save("PivotFieldOriginalItemsDemo_Output.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


