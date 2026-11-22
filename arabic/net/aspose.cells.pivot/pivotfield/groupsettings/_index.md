---
title: "PivotField.GroupSettings"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية PivotField. تحصل على إعدادات التجميع للحقل المحوري"
type: docs
url: /ar/net/aspose.cells.pivot/pivotfield/groupsettings/
---
## PivotField.GroupSettings property

يحصل على إعدادات التجميع للحقل المحوري.

```csharp
public PivotFieldGroupSettings GroupSettings { get; }
```

### ملاحظات

إذا لم يتم تجميع هذا الحقل، سيتم إرجاع Null.

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldPropertyGroupSettingsDemo
    {
        public static void Run()
        {
            // إنشاء مصنف من ملف Excel المصدر
            Workbook workbook = new Workbook("example.xlsx");
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            
            // الوصول إلى أول جدول محوري
            PivotTable pivotTable = worksheet.PivotTables[0];
            
            // الوصول إلى الحقل الأساسي الثاني (بافتراض وجوده)
            if (pivotTable.BaseFields.Count > 1)
            {
                PivotField pivotField = pivotTable.BaseFields[1];
                
                // تحقق مما إذا كان الحقل يحتوي على إعدادات التجميع
                if (pivotField.GroupSettings != null)
                {
                    Console.WriteLine("Field has grouping enabled");
                    Console.WriteLine("Group type: " + pivotField.GroupSettings.Type);
                }
                else
                {
                    Console.WriteLine("Field has no grouping settings");
                }
                
                // مثال على تجميع حقل رقمي
                if (pivotField.GroupSettings == null && 
                    pivotField.PivotItems.Count > 0 && 
                    pivotField.PivotItems[0].Value is double)
                {
                    // التجميع حسب النطاق الرقمي (فواصل وحدة 10)
                    pivotField.GroupBy(10.0, false);
                    Console.WriteLine("Field grouped by numeric range");
                }
            }
            
            // احفظ المصنف المعدل
            workbook.Save("output.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [PivotFieldGroupSettings](../../pivotfieldgroupsettings/)
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


