---
title: "DataModelTable.Id"
second_title: "Aspose.Cells för .NET API‑referens"
description: "DataModelTable‑egenskap. Hämtar id för datamodelltabellen"
type: docs
url: /sv/net/aspose.cells.datamodels/datamodelrelationship/primarykeycolumn/
---
## DataModelRelationship.PrimaryKeyColumn property

Hämtar namnet på kolumnen i den primära nyckelns tabell för denna relation.

```csharp
public string PrimaryKeyColumn { get; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.DataModels;
    using System;

    public class DataModelRelationshipPropertyPrimaryKeyColumnDemo
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
                    // Hämta DataModelTable (denna är skrivskyddad i arbetsboken)
                    Console.WriteLine("Primary Key Column: " + relationship.PrimaryKeyColumn);
                }
                else
                {
                    Console.WriteLine("No relationships found in the data model.");
                }

                // Spara arbetsboken
                workbook.Save("PrimaryKeyColumnDemo.xlsx");
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


