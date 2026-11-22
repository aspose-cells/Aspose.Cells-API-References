---
title: "DataModelTable.Id"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية DataModelTable. تحصل على معرف جدول نموذج البيانات"
type: docs
url: /ar/net/aspose.cells.datamodels/datamodeltable/id/
---
## DataModelTable.Id property

يحصل على معرف جدول نموذج البيانات.

```csharp
public string Id { get; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.DataModels;
    using Aspose.Cells.Tables;
    using System;

    public class DataModelTablePropertyIdDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف بيانات عينة لإنشاء جدول
            worksheet.Cells["A1"].PutValue("ID");
            worksheet.Cells["B1"].PutValue("Name");
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["B2"].PutValue("Item 1");
            worksheet.Cells["A3"].PutValue(2);
            worksheet.Cells["B3"].PutValue("Item 2");

            // إنشاء ListObject (جدول)
            int index = worksheet.ListObjects.Add(0, 0, 2, 1, true);
            ListObject table = worksheet.ListObjects[index];

            // احصل على DataModelTable (هذا للقراءة فقط في دفتر العمل)
            DataModelTable dataModelTable = workbook.DataModel.Tables[0];

            // عرض قيمة المعرف الحالية
            Console.WriteLine("Current DataModelTable Id: " + dataModelTable.Id);

            // ملاحظة: خاصية Id للقراءة فقط، لذلك لا يمكننا تعيينها
            // هذا يوضح كيفية الوصول إلى واستخدام الـ Id الموجود

            // مثال على الاستخدام: قارن معرفات الجداول عند العمل مع جداول متعددة
            DataModelTable secondTable = null;
            if (workbook.DataModel.Tables.Count > 1)
            {
                secondTable = workbook.DataModel.Tables[1];
                if (dataModelTable.Id != secondTable.Id)
                {
                    Console.WriteLine("Different table IDs detected");
                }
            }

            // احفظ المصنف
            workbook.Save("DataModelTableIdDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [DataModelTable](../)
* namespace [Aspose.Cells.DataModels](../../../aspose.cells.datamodels/)
* assembly [Aspose.Cells](../../../)


