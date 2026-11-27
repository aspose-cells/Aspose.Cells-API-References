---
title: "Klass DataModelRelationship"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.DataModels.DataModelRelationship klass. Representerar en enskild relation i kalkylbladets datamodell"
type: docs
url: /sv/net/aspose.cells.datamodels/datamodelrelationship/
---
## DataModelRelationship class

Representerar ett enskilt förhållande i kalkylbladets datamodell.

```csharp
public class DataModelRelationship
```

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [ForeignKeyColumn](../../aspose.cells.datamodels/datamodelrelationship/foreignkeycolumn/) { get; } | Hämtar namnet på kolumnen i den främmande nyckelns tabell för denna relation. |
| [ForeignKeyTable](../../aspose.cells.datamodels/datamodelrelationship/foreignkeytable/) { get; } | Hämtar namnet på den främmande nyckelns tabell för denna relation. |
| [PrimaryKeyColumn](../../aspose.cells.datamodels/datamodelrelationship/primarykeycolumn/) { get; } | Hämtar namnet på kolumnen i den primära nyckelns tabell för denna relation. |
| [PrimaryKeyTable](../../aspose.cells.datamodels/datamodelrelationship/primarykeytable/) { get; } | Hämtar namnet på den primära nyckelns tabell för denna relation. |

### Exempel

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
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Skapa exempeldata för demonstration
            worksheet.Cells["A1"].PutValue("Orders");
            worksheet.Cells["A2"].PutValue("OrderID");
            worksheet.Cells["A3"].PutValue("CustomerID");
            worksheet.Cells["A4"].PutValue("OrderDate");
            
            worksheet.Cells["C1"].PutValue("Customers");
            worksheet.Cells["C2"].PutValue("CustomerID");
            worksheet.Cells["C3"].PutValue("CustomerName");
            worksheet.Cells["C4"].PutValue("ContactName");

            // Detta demonstrerar åtkomst till egenskaperna för en befintlig relation
            // I ett verkligt scenario skulle du hämta detta från DataModel
            DataModelRelationship relationship = workbook.DataModel?.Relationships?[0];
            if (relationship != null)
            {
                // Visa relations egenskaper (skrivskyddade)
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

            // Spara arbetsboken
            workbook.Save("DataModelRelationshipDemo.xlsx");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells.DataModels](../../aspose.cells.datamodels/)
* assembly [Aspose.Cells](../../)


