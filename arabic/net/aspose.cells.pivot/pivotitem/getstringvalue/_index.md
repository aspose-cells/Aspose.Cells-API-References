---
title: "PivotItem.GetStringValue"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة PivotItem. يحصل على القيمة النصية لعنصر المحور إذا كانت القيمة فارغة سيعيد"
type: docs
url: /ar/net/aspose.cells.pivot/pivotitem/getstringvalue/
---
## PivotItem.GetStringValue method

يحصل على القيمة النصية لعنصر المحور. إذا كانت القيمة فارغة، سيعيد ""

```csharp
public string GetStringValue()
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotItemMethodGetStringValueDemo
    {
        public static void Run()
        {
            // إنشاء مصنف من ملف Excel المصدر
            Workbook workbook = new Workbook("example.xlsx");
            
            // الوصول إلى ورقة العمل الأولى وجدول المحور
            Worksheet worksheet = workbook.Worksheets[0];
            PivotTable pivotTable = worksheet.PivotTables[0];
            
            // احصل على حقل الصف الأول وعناصره المحورية
            PivotField rowField = pivotTable.RowFields[0];
            PivotItemCollection pivotItems = rowField.PivotItems;
            
            // عرض طريقة GetStringValue()
            string itemValue = pivotItems[1].GetStringValue();
            Console.WriteLine("PivotItem value: " + itemValue);
            
            // احفظ المصنف المعدل
            workbook.Save("output.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [PivotItem](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


