---
title: "DataModelTable.ConnectionName"
second_title: "Aspose.Cells için .NET API Referansı"
description: "DataModelTable özelliği. Veri modeli tablosunun bağlantı adını alır"
type: docs
url: /tr/net/aspose.cells.datamodels/datamodeltable/connectionname/
---
## DataModelTable.ConnectionName property

Veri modeli tablosunun bağlantı adını alır.

```csharp
public string ConnectionName { get; }
```

### Örnekler

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
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Bir tablo oluşturmak için örnek veri ekle
            worksheet.Cells["A1"].PutValue("OrderID");
            worksheet.Cells["B1"].PutValue("Customer");
            worksheet.Cells["A2"].PutValue(1001);
            worksheet.Cells["B2"].PutValue("John Doe");
            worksheet.Cells["A3"].PutValue(1002);
            worksheet.Cells["B3"].PutValue("Jane Smith");

            // Bir ListObject (tablo) oluştur
            int tableIndex = worksheet.ListObjects.Add(0, 0, 2, 1, true);
            ListObject table = worksheet.ListObjects[tableIndex];
            table.DisplayName = "OrdersTable";

            // DataModelTable'a eriş
            DataModelTable dataModelTable = workbook.DataModel.Tables[0];

            // Mevcut ConnectionName değerini göster
            Console.WriteLine("Current ConnectionName: " + dataModelTable.ConnectionName);

            // DataModelTable'ın bağlantısını kullanarak bir pivot tablo oluştur
            Worksheet pivotSheet = workbook.Worksheets.Add("PivotReport");
            int pivotIndex = pivotSheet.PivotTables.Add("PivotTable1", "A1", dataModelTable.Name);
            PivotTable pivotTable = pivotSheet.PivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Customer");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "OrderID");

            // Not: ConnectionName yalnızca okunabilir, bu yüzden ayarlayamıyoruz
            // Bu, mevcut bağlantı adının nasıl kullanılacağını gösterir
            if (!string.IsNullOrEmpty(dataModelTable.ConnectionName))
            {
                Console.WriteLine("This table is connected via: " + dataModelTable.ConnectionName);
            }

            // Çalışma kitabını kaydedin
            workbook.Save("DataModelTableConnectionNameDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [DataModelTable](../)
* namespace [Aspose.Cells.DataModels](../../../aspose.cells.datamodels/)
* assembly [Aspose.Cells](../../../)


