---
title: "تعداد TableDataSourceType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "تعداد Aspose.Cells.Tables.TableDataSourceType. يمثل نوع مصدر بيانات الجداول"
type: docs
url: /ar/net/aspose.cells.tables/tabledatasourcetype/
---
## TableDataSourceType enumeration

يمثل نوع مصدر بيانات الجدول.

```csharp
public enum TableDataSourceType
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| Worksheet | `0` | جدول ورقة عمل Excel |
| SharePoint | `1` | قائمة SharePoint المرتبطة للقراءة والكتابة |
| XML | `2` | جدول محول XML |
| QueryTable | `3` | جدول الاستعلام |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Tables;
    using System;

    public class TableDataSourceTypeDemo
    {
        public static void TableDataSourceTypeExample()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();

            // إضافة ورقة عمل جديدة إلى المصنف
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة بيانات عينة إلى ورقة العمل
            worksheet.Cells["A1"].PutValue("ID");
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["A3"].PutValue(2);
            worksheet.Cells["A4"].PutValue(3);

            worksheet.Cells["B1"].PutValue("Name");
            worksheet.Cells["B2"].PutValue("Alice");
            worksheet.Cells["B3"].PutValue("Bob");
            worksheet.Cells["B4"].PutValue("Charlie");

            // أضف ListObject (جدول) إلى ورقة العمل
            int listObjectIndex = worksheet.ListObjects.Add(1, 0, 4, 1, true);
            ListObject listObject = worksheet.ListObjects[listObjectIndex];

            // تعيين اسم العرض للجدول
            listObject.DisplayName = "SampleTable";

            // تعيين نوع مصدر البيانات للجدول
            TableDataSourceType dataSourceType = listObject.DataSourceType;

            // إخراج نوع مصدر البيانات
            Console.WriteLine("Data Source Type: " + dataSourceType);

            // احفظ المصنف
            workbook.Save("TableDataSourceTypeExample.xlsx");
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells.Tables](../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../)


