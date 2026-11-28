---
title: "DataModelRelationship.PrimaryKeyTable"
second_title: "Aspose.Cells için .NET API Referansı"
description: "DataModelRelationship özelliği. Bu ilişki için birincil anahtar tablosunun adını alır"
type: docs
url: /tr/net/aspose.cells.datamodels/datamodelrelationship/primarykeytable/
---
## DataModelRelationship.PrimaryKeyTable property

Bu ilişki için birincil anahtar tablo adını alır.

```csharp
public string PrimaryKeyTable { get; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.DataModels;
    using System;

    public class DataModelRelationshipPropertyPrimaryKeyTableDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Anlamlı bir bağlam oluşturmak için örnek veri ekleyin
            worksheet.Cells["A1"].PutValue("Orders");
            worksheet.Cells["A2"].PutValue("OrderID");
            worksheet.Cells["A3"].PutValue("CustomerID");

            worksheet.Cells["C1"].PutValue("Customers");
            worksheet.Cells["C2"].PutValue("CustomerID");
            worksheet.Cells["C3"].PutValue("CustomerName");

            try
            {
                // Var ise ilk ilişkiye erişin
                DataModelRelationship relationship = workbook.DataModel?.Relationships?[0];

                if (relationship != null)
                {
                    // PrimaryKeyTable özelliği değerini gösterin (yalnızca okunur)
                    Console.WriteLine("Primary Key Table: " + relationship.PrimaryKeyTable);
                }
                else
                {
                    Console.WriteLine("No relationships found in the data model.");
                }

                // Çalışma kitabını kaydedin
                workbook.Save("PrimaryKeyTableDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [DataModelRelationship](../)
* namespace [Aspose.Cells.DataModels](../../../aspose.cells.datamodels/)
* assembly [Aspose.Cells](../../../)


