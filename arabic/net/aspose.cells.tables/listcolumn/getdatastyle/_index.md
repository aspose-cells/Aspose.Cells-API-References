---
title: "ListColumn.GetDataStyle"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة ListColumn. تحصل على نمط البيانات في هذا العمود من الجدول"
type: docs
url: /ar/net/aspose.cells.tables/listcolumn/getdatastyle/
---
## ListColumn.GetDataStyle method

يحصل على نمط البيانات في هذا العمود من الجدول.

```csharp
public Style GetDataStyle()
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ListColumnMethodGetDataStyleDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            
            // أضف بيانات تجريبية إلى الخلايا
            worksheet.Cells["A1"].PutValue("Header");
            worksheet.Cells["A2"].PutValue("Data1");
            worksheet.Cells["A3"].PutValue("Data2");
            
            // إنشاء كائن قائمة (جدول)
            int index = worksheet.ListObjects.Add(0, 0, 2, 0, true);
            Aspose.Cells.Tables.ListObject table = worksheet.ListObjects[index];
            
            // احصل على النمط من العمود الأول في القائمة
            Style style = table.ListColumns[0].GetDataStyle();
            
            // تعديل النمط
            style.Pattern = BackgroundType.Solid;
            style.BackgroundColor = System.Drawing.Color.Red;
            
            // تطبيق النمط المعدل مرة أخرى على العمود
            table.ListColumns[0].SetDataStyle(style);
            
            // احفظ المصنف
            workbook.Save("output.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Style](../../../aspose.cells/style/)
* class [ListColumn](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


