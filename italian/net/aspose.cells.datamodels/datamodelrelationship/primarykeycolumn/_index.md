---
title: "DataModelRelationship.PrimaryKeyColumn"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà DataModelRelationship. Ottiene il nome della colonna della tabella chiave primaria per questa relazione"
type: docs
url: /it/net/aspose.cells.datamodels/datamodelrelationship/primarykeycolumn/
---
## DataModelRelationship.PrimaryKeyColumn property

Ottiene il nome della colonna della tabella chiave primaria per questa relazione.

```csharp
public string PrimaryKeyColumn { get; }
```

### Esempi

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
                    // Visualizza il valore della proprietà PrimaryKeyColumn (sola lettura)
                    Console.WriteLine("Primary Key Column: " + relationship.PrimaryKeyColumn);
                }
                else
                {
                    Console.WriteLine("No relationships found in the data model.");
                }

                // Salva la cartella di lavoro
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

### Vedi anche

* class [DataModelRelationship](../)
* namespace [Aspose.Cells.DataModels](../../../aspose.cells.datamodels/)
* assembly [Aspose.Cells](../../../)


