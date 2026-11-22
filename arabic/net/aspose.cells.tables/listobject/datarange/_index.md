---
title: "ListObject.DataRange"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ListObject. يحصل على نطاق البيانات للجدول"
type: docs
url: /ar/net/aspose.cells.tables/listobject/datarange/
---
## ListObject.DataRange property

يحصل على نطاق البيانات للجدول.

```csharp
public Range DataRange { get; }
```

### أمثلة

```csharp
using System;
using System.Text;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ListObjectPropertyDataRangeDemo
    {
        public static void Run()
        {
            Encoding.RegisterProvider(CodePagesEncodingProvider.Instance);
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف بيانات تجريبية
            worksheet.Cells["A1"].PutValue("ID");
            worksheet.Cells["B1"].PutValue("Name");
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["B2"].PutValue("John");
            worksheet.Cells["A3"].PutValue(2);
            worksheet.Cells["B3"].PutValue("Mary");

            // أنشئ ListObject (جدول)
            int tableIndex = worksheet.ListObjects.Add(0, 0, 2, 1, true);
            Aspose.Cells.Tables.ListObject table = worksheet.ListObjects[tableIndex];
            table.DisplayName = "EmployeeTable";

            // احصل على نطاق البيانات للجدول
            Aspose.Cells.Range dataRange = table.DataRange;

            // عرض استخدام DataRange
            Console.WriteLine("Table Data Range: " + dataRange.Address);
            Console.WriteLine("Row Count: " + dataRange.RowCount);
            Console.WriteLine("Column Count: " + dataRange.ColumnCount);

            // إضافة صيغة إلى العمود الأخير باستخدام DataRange
            string formula = "=CONCATENATE(\"ID-\", [ID])";
            int lastColIndex = dataRange.ColumnCount - 1;
            dataRange[0, lastColIndex].PutValue("FormattedID");
            for (int i = 1; i < dataRange.RowCount; i++)
            {
                dataRange[i, lastColIndex].Formula = formula;
            }

            // احفظ المصنف
            workbook.Save("ListObjectDataRangeDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Range](../../../aspose.cells/range/)
* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


