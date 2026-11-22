---
title: "الفئة DataModelTable"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "الفئة Aspose.Cells.DataModels.DataModelTable. تمثل خصائص جدول واحد في نموذج بيانات جدول البيانات"
type: docs
url: /ar/net/aspose.cells.datamodels/datamodeltable/
---
## DataModelTable class

يمثل خصائص جدول واحد في نموذج بيانات جدول البيانات.

```csharp
public class DataModelTable
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [ConnectionName](../../aspose.cells.datamodels/datamodeltable/connectionname/) { get; } | يحصل على اسم الاتصال لجدول نموذج البيانات. |
| [Id](../../aspose.cells.datamodels/datamodeltable/id/) { get; } | يحصل على معرف جدول نموذج البيانات. |
| [Name](../../aspose.cells.datamodels/datamodeltable/name/) { get; } | يحصل على اسم جدول نموذج البيانات. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.DataModels;
    using Aspose.Cells.Tables;
    using Aspose.Cells.Pivot;
    using System;

    public class DataModelsClassDataModelTableDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف بيانات عينة لإنشاء جدول
            worksheet.Cells["A1"].PutValue("ProductID");
            worksheet.Cells["B1"].PutValue("ProductName");
            worksheet.Cells["A2"].PutValue(101);
            worksheet.Cells["B2"].PutValue("Laptop");
            worksheet.Cells["A3"].PutValue(102);
            worksheet.Cells["B3"].PutValue("Monitor");

            // إنشاء ListObject (جدول)
            int tableIndex = worksheet.ListObjects.Add(0, 0, 2, 1, true);
            ListObject table = worksheet.ListObjects[tableIndex];
            table.DisplayName = "ProductsTable";

            // الوصول إلى DataModelTable
            DataModelTable dataModelTable = workbook.DataModel.Tables[0];

            // عرض خصائص DataModelTable
            Console.WriteLine("Data Model Table Properties:");
            Console.WriteLine($"ID: {dataModelTable.Id}");
            Console.WriteLine($"Name: {dataModelTable.Name}");
            Console.WriteLine($"Connection Name: {dataModelTable.ConnectionName}");

            // إنشاء جدول محوري باستخدام DataModelTable
            Worksheet pivotSheet = workbook.Worksheets.Add("PivotSheet");
            int pivotIndex = pivotSheet.PivotTables.Add("PivotTable1", "A1", dataModelTable.Name);
            PivotTable pivotTable = pivotSheet.PivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, "ProductName");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "ProductID");

            // احفظ المصنف
            workbook.Save("DataModelTableDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells.DataModels](../../aspose.cells.datamodels/)
* assembly [Aspose.Cells](../../)


