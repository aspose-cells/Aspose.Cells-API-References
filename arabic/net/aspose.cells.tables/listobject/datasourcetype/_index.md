---
title: "ListObject.DataSourceType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ListObject. تحصل على نوع مصدر البيانات للجدول"
type: docs
url: /ar/net/aspose.cells.tables/listobject/datasourcetype/
---
## ListObject.DataSourceType property

يحصل على نوع مصدر البيانات للجدول.

```csharp
public TableDataSourceType DataSourceType { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class ListObjectPropertyDataSourceTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف بيانات تجريبية
            worksheet.Cells["A1"].PutValue("ID");
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["A3"].PutValue(2);
            worksheet.Cells["B1"].PutValue("Name");
            worksheet.Cells["B2"].PutValue("Alice");
            worksheet.Cells["B3"].PutValue("Bob");

            // إنشاء كائن قائمة والحصول عليه من المجموعة
            int listObjectIndex = worksheet.ListObjects.Add(0, 0, 2, 1, true);
            ListObject listObject = worksheet.ListObjects[listObjectIndex];
            listObject.DisplayName = "EmployeeTable";

            // الحصول على وعرض DataSourceType
            TableDataSourceType dataSourceType = listObject.DataSourceType;
            Console.WriteLine("ListObject DataSourceType: " + dataSourceType);

            workbook.Save("ListObjectDataSourceTypeDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* enum [TableDataSourceType](../../tabledatasourcetype/)
* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


