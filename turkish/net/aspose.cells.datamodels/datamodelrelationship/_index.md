---
title: "Sınıf DataModelRelationship"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.DataModels.DataModelRelationship sınıfı. Elektronik tablo veri modelinde tek bir ilişkiyi temsil eder"
type: docs
url: /tr/net/aspose.cells.datamodels/datamodelrelationship/
---
## DataModelRelationship class

Elektronik tablo veri modelinde tek bir ilişkiyi temsil eder.

```csharp
public class DataModelRelationship
```

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [ForeignKeyColumn](../../aspose.cells.datamodels/datamodelrelationship/foreignkeycolumn/) { get; } | Bu ilişki için dış anahtar tablo sütununun adını alır. |
| [ForeignKeyTable](../../aspose.cells.datamodels/datamodelrelationship/foreignkeytable/) { get; } | Bu ilişki için dış anahtar tablo adını alır. |
| [PrimaryKeyColumn](../../aspose.cells.datamodels/datamodelrelationship/primarykeycolumn/) { get; } | Bu ilişki için birincil anahtar tablo sütununun adını alır. |
| [PrimaryKeyTable](../../aspose.cells.datamodels/datamodelrelationship/primarykeytable/) { get; } | Bu ilişki için birincil anahtar tablo adını alır. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.DataModels;
    using System;

    public class DataModelsClassDataModelRelationshipDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Gösterim için örnek veri oluştur
            worksheet.Cells["A1"].PutValue("Orders");
            worksheet.Cells["A2"].PutValue("OrderID");
            worksheet.Cells["A3"].PutValue("CustomerID");
            worksheet.Cells["A4"].PutValue("OrderDate");
            
            worksheet.Cells["C1"].PutValue("Customers");
            worksheet.Cells["C2"].PutValue("CustomerID");
            worksheet.Cells["C3"].PutValue("CustomerName");
            worksheet.Cells["C4"].PutValue("ContactName");

            // Bu, mevcut bir ilişkinin özelliklerine erişimi gösterir
            // Gerçek bir senaryoda, bunu DataModel'den alırdınız
            DataModelRelationship relationship = workbook.DataModel?.Relationships?[0];
            if (relationship != null)
            {
                // İlişki özelliklerini göster (yalnızca okunur)
                Console.WriteLine("Sample Data Model Relationship Properties:");
                Console.WriteLine("Primary Key Table: " + relationship.PrimaryKeyTable);
                Console.WriteLine("Primary Key Column: " + relationship.PrimaryKeyColumn);
                Console.WriteLine("Foreign Key Table: " + relationship.ForeignKeyTable);
                Console.WriteLine("Foreign Key Column: " + relationship.ForeignKeyColumn);
            }
            else
            {
                Console.WriteLine("No data model relationships found");
            }

            // Çalışma kitabını kaydedin
            workbook.Save("DataModelRelationshipDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells.DataModels](../../aspose.cells.datamodels/)
* assembly [Aspose.Cells](../../)


