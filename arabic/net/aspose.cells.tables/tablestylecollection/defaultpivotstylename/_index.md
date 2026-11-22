---
title: "TableStyleCollection.DefaultPivotStyleName"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية TableStyleCollection. تحصل وتضبط اسم النمط الافتراضي لجدول المحور"
type: docs
url: /ar/net/aspose.cells.tables/tablestylecollection/defaultpivotstylename/
---
## TableStyleCollection.DefaultPivotStyleName property

يحصل على ويضبط اسم النمط الافتراضي لجدول المحور.

```csharp
public string DefaultPivotStyleName { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class TableStyleCollectionPropertyDefaultPivotStyleNameDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى مجموعة أنماط الجدول
            TableStyleCollection tableStyles = workbook.Worksheets.TableStyles;
            
            // عرض اسم النمط الافتراضي لجدول المحور
            Console.WriteLine("Default Pivot Style: " + tableStyles.DefaultPivotStyleName);
            
            // تغيير النمط الافتراضي لجدول المحور
            tableStyles.DefaultPivotStyleName = "PivotStyleDark2";
            
            // تحقق من التغيير
            Console.WriteLine("Updated Default Pivot Style: " + tableStyles.DefaultPivotStyleName);
            
            // احفظ المصنف
            workbook.Save("output.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [TableStyleCollection](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


