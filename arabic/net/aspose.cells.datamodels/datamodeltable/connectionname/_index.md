---
title: "DataModelTable.ConnectionName"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية DataModelTable. تحصل على اسم الاتصال لجدول نموذج البيانات"
type: docs
url: /ar/net/aspose.cells.datamodels/datamodeltable/connectionname/
---
## DataModelTable.ConnectionName property

يحصل على اسم الاتصال لجدول نموذج البيانات.

```csharp
public string ConnectionName { get; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.DataModels;
    using Aspose.Cells.Tables;
    using Aspose.Cells.Pivot;
    using System;

    public class DataModelTablePropertyConnectionNameDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف بيانات عينة لإنشاء جدول
            worksheet.Cells["A1"].PutValue("OrderID");
            worksheet.Cells["B1"].PutValue("Customer");
            worksheet.Cells["A2"].PutValue(1001);
            worksheet.Cells["B2"].PutValue("John Doe");
            worksheet.Cells["A3"].PutValue(1002);
            worksheet.Cells["B3"].PutValue("Jane Smith");

            // إنشاء ListObject (جدول)
            int tableIndex = worksheet.ListObjects.Add(0, 0, 2, 1, true);
            ListObject table = worksheet.ListObjects[tableIndex];
            table.DisplayName = "OrdersTable";

            // الوصول إلى DataModelTable
            DataModelTable dataModelTable = workbook.DataModel.Tables[0];

            // اعرض قيمة ConnectionName الحالية
            Console.WriteLine("Current ConnectionName: " + dataModelTable.ConnectionName);

            // أنشئ جدول محوري باستخدام اتصال DataModelTable
            Worksheet pivotSheet = workbook.Worksheets.Add("PivotReport");
            int pivotIndex = pivotSheet.PivotTables.Add("PivotTable1", "A1", dataModelTable.Name);
            PivotTable pivotTable = pivotSheet.PivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Customer");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "OrderID");

            // ملاحظة: ConnectionName للقراءة فقط، لذلك لا يمكننا تعيينه
            // هذا يوضح كيفية استخدام اسم الاتصال الموجود
            if (!string.IsNullOrEmpty(dataModelTable.ConnectionName))
            {
                Console.WriteLine("This table is connected via: " + dataModelTable.ConnectionName);
            }

            // احفظ المصنف
            workbook.Save("DataModelTableConnectionNameDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [DataModelTable](../)
* namespace [Aspose.Cells.DataModels](../../../aspose.cells.datamodels/)
* assembly [Aspose.Cells](../../../)


