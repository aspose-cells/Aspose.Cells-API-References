---
title: "Sınıf DataModelTable"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.DataModels.DataModelTable sınıfı. Elektronik tablo veri modelinde tek bir tablonun özelliklerini temsil eder"
type: docs
url: /tr/net/aspose.cells.datamodels/datamodeltable/
---
## DataModelTable class

Elektronik tablo veri modelindeki tek bir tablonun özelliklerini temsil eder.

```csharp
public class DataModelTable
```

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [ConnectionName](../../aspose.cells.datamodels/datamodeltable/connectionname/) { get; } | Veri modeli tablosunun bağlantı adını alır. |
| [Id](../../aspose.cells.datamodels/datamodeltable/id/) { get; } | Veri modeli tablosunun kimliğini alır. |
| [Name](../../aspose.cells.datamodels/datamodeltable/name/) { get; } | Veri modeli tablosunun adını alır. |

### Örnekler

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
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Bir tablo oluşturmak için örnek veri ekle
            worksheet.Cells["A1"].PutValue("ProductID");
            worksheet.Cells["B1"].PutValue("ProductName");
            worksheet.Cells["A2"].PutValue(101);
            worksheet.Cells["B2"].PutValue("Laptop");
            worksheet.Cells["A3"].PutValue(102);
            worksheet.Cells["B3"].PutValue("Monitor");

            // Bir ListObject (tablo) oluştur
            int tableIndex = worksheet.ListObjects.Add(0, 0, 2, 1, true);
            ListObject table = worksheet.ListObjects[tableIndex];
            table.DisplayName = "ProductsTable";

            // DataModelTable'a eriş
            DataModelTable dataModelTable = workbook.DataModel.Tables[0];

            // DataModelTable özelliklerini göster
            Console.WriteLine("Data Model Table Properties:");
            Console.WriteLine($"ID: {dataModelTable.Id}");
            Console.WriteLine($"Name: {dataModelTable.Name}");
            Console.WriteLine($"Connection Name: {dataModelTable.ConnectionName}");

            // DataModelTable kullanarak bir pivot tablo oluştur
            Worksheet pivotSheet = workbook.Worksheets.Add("PivotSheet");
            int pivotIndex = pivotSheet.PivotTables.Add("PivotTable1", "A1", dataModelTable.Name);
            PivotTable pivotTable = pivotSheet.PivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, "ProductName");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "ProductID");

            // Çalışma kitabını kaydedin
            workbook.Save("DataModelTableDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells.DataModels](../../aspose.cells.datamodels/)
* assembly [Aspose.Cells](../../)


