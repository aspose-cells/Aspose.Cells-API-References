---
title: "ListObject.TableStyleName"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ListObject. تحصل وتحدد اسم نمط الجدول"
type: docs
url: /ar/net/aspose.cells.tables/listobject/tablestylename/
---
## ListObject.TableStyleName property

يحصل ويضبط اسم نمط الجدول.

```csharp
public string TableStyleName { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class ListObjectPropertyTableStyleNameDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف بيانات تجريبية
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("Alice");
            worksheet.Cells["B3"].PutValue(25);

            // إنشاء كائن/جدول قائمة
            int index = worksheet.ListObjects.Add(0, 0, 2, 1, true);
            ListObject table = worksheet.ListObjects[index];

            // تعيين وعرض نمط الجدول
            table.TableStyleName = "TableStyleLight15";
            Console.WriteLine("Table style name: " + table.TableStyleName);

            // احفظ المصنف
            workbook.Save("TableStyleDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


