---
title: "TableStyleCollection.DefaultTableStyleName"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية TableStyleCollection. تحصل وتضبط اسم النمط الافتراضي للجدول"
type: docs
url: /ar/net/aspose.cells.tables/tablestylecollection/defaulttablestylename/
---
## TableStyleCollection.DefaultTableStyleName property

يحصل على اسم النمط الافتراضي للجدول ويضبطه.

```csharp
public string DefaultTableStyleName { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class TableStyleCollectionPropertyDefaultTableStyleNameDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى مجموعة أنماط الجدول
            TableStyleCollection tableStyles = workbook.Worksheets.TableStyles;
            
            // عرض اسم نمط الجدول الافتراضي
            Console.WriteLine("Default Table Style: " + tableStyles.DefaultTableStyleName);
            
            // تغيير نمط الجدول الافتراضي
            tableStyles.DefaultTableStyleName = "TableStyleMedium9";
            Console.WriteLine("New Default Table Style: " + tableStyles.DefaultTableStyleName);
            
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


