---
title: "ListObject.ShowHeaderRow"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ListObject. يحصل ويضبط ما إذا كان هذا الجدول يعرض صف الرأس"
type: docs
url: /ar/net/aspose.cells.tables/listobject/showheaderrow/
---
## ListObject.ShowHeaderRow property

يحصل ويضبط ما إذا كان هذا الجدول يعرض صف الرأس.

```csharp
public bool ShowHeaderRow { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class ListObjectPropertyShowHeaderRowDemo
    {
        public static void Run()
        {
            // إنشاء مصنف وورقة عمل
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف بيانات تجريبية
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Banana");
            worksheet.Cells["A4"].PutValue("Cherry");

            // إنشاء كائن/جدول قائمة
            int tableIndex = worksheet.ListObjects.Add(0, 0, 3, 0, true);
            ListObject table = worksheet.ListObjects[tableIndex];
            table.TableStyleType = TableStyleType.TableStyleMedium2;
            table.ShowHeaderRow = true; // Header row is visible by default

            Console.WriteLine("Header row is visible: " + table.ShowHeaderRow);
            Console.WriteLine("Header cell value: " + worksheet.Cells["A1"].StringValue);

            // إخفاء صف الرأس
            table.ShowHeaderRow = false;
            Console.WriteLine("\nAfter setting ShowHeaderRow to false:");
            Console.WriteLine("Header row is visible: " + table.ShowHeaderRow);
            Console.WriteLine("Header cell value: " + worksheet.Cells["A1"].StringValue);

            // احفظ المصنف
            workbook.Save("ListObjectShowHeaderRowDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


