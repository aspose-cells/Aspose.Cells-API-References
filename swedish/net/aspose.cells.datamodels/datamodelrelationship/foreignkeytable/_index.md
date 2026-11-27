---
title: "DataModelRelationship.ForeignKeyTable"
second_title: "Aspose.Cells för .NET API‑referens"
description: "DataModelRelationship‑egenskap. Hämtar namnet på den främmande nyckelns tabell för detta förhållande"
type: docs
url: /sv/net/aspose.cells.datamodels/datamodelrelationship/foreignkeytable/
---
## DataModelRelationship.ForeignKeyTable property

Hämtar namnet på den främmande nyckelns tabell för denna relation.

```csharp
public string ForeignKeyTable { get; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.DataModels;
    using System;

    public class DataModelRelationshipPropertyForeignKeyTableDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata för att skapa ett meningsfullt sammanhang
            worksheet.Cells["A1"].PutValue("Orders");
            worksheet.Cells["A2"].PutValue("OrderID");
            worksheet.Cells["A3"].PutValue("CustomerID");

            worksheet.Cells["C1"].PutValue("Customers");
            worksheet.Cells["C2"].PutValue("CustomerID");
            worksheet.Cells["C3"].PutValue("CustomerName");

            try
            {
                // Få åtkomst till den första relationen om den finns
                DataModelRelationship relationship = workbook.DataModel?.Relationships?[0];

                if (relationship != null)
                {
                    // Visa värdet för egenskapen ForeignKeyTable (skrivskyddad)
                    Console.WriteLine("Foreign Key Table: " + relationship.ForeignKeyTable);
                }
                else
                {
                    Console.WriteLine("No relationships found in the data model.");
                }

                // Spara arbetsboken
                workbook.Save("ForeignKeyTableDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Se även

* class [DataModelRelationship](../)
* namespace [Aspose.Cells.DataModels](../../../aspose.cells.datamodels/)
* assembly [Aspose.Cells](../../../)


