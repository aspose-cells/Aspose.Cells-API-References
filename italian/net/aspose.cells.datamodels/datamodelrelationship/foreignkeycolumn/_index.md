---
title: "DataModelRelationship.ForeignKeyColumn"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà DataModelRelationship. Ottiene il nome della colonna della tabella chiave esterna per questa relazione"
type: docs
url: /it/net/aspose.cells.datamodels/datamodelrelationship/foreignkeycolumn/
---
## DataModelRelationship.ForeignKeyColumn property

Ottiene il nome della colonna della tabella chiave esterna per questa relazione.

```csharp
public string ForeignKeyColumn { get; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.DataModels;
    using System;

    public class DataModelRelationshipPropertyForeignKeyColumnDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio per creare un contesto significativo
            worksheet.Cells["A1"].PutValue("Orders");
            worksheet.Cells["A2"].PutValue("OrderID");
            worksheet.Cells["A3"].PutValue("CustomerID");

            worksheet.Cells["C1"].PutValue("Customers");
            worksheet.Cells["C2"].PutValue("CustomerID");
            worksheet.Cells["C3"].PutValue("CustomerName");

            try
            {
                // Accedi alla prima relazione se esiste
                DataModelRelationship relationship = workbook.DataModel?.Relationships?[0];

                if (relationship != null)
                {
                    // Visualizza il valore della proprietà ForeignKeyColumn (sola lettura)
                    Console.WriteLine("Foreign Key Column: " + relationship.ForeignKeyColumn);
                }
                else
                {
                    Console.WriteLine("No relationships found in the data model.");
                }

                // Salva la cartella di lavoro
                workbook.Save("ForeignKeyColumnDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Vedi anche

* class [DataModelRelationship](../)
* namespace [Aspose.Cells.DataModels](../../../aspose.cells.datamodels/)
* assembly [Aspose.Cells](../../../)


