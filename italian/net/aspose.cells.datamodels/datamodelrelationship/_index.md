---
title: "Classe DataModelRelationship"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.DataModels.DataModelRelationship. Rappresenta una singola relazione nel modello dati del foglio di calcolo"
type: docs
url: /it/net/aspose.cells.datamodels/datamodelrelationship/
---
## DataModelRelationship class

Rappresenta una singola relazione nel modello di dati del foglio di calcolo.

```csharp
public class DataModelRelationship
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [ForeignKeyColumn](../../aspose.cells.datamodels/datamodelrelationship/foreignkeycolumn/) { get; } | Ottiene il nome della colonna della tabella chiave esterna per questa relazione. |
| [ForeignKeyTable](../../aspose.cells.datamodels/datamodelrelationship/foreignkeytable/) { get; } | Ottiene il nome della tabella chiave esterna per questa relazione. |
| [PrimaryKeyColumn](../../aspose.cells.datamodels/datamodelrelationship/primarykeycolumn/) { get; } | Ottiene il nome della colonna della tabella chiave primaria per questa relazione. |
| [PrimaryKeyTable](../../aspose.cells.datamodels/datamodelrelationship/primarykeytable/) { get; } | Ottiene il nome della tabella chiave primaria per questa relazione. |

### Esempi

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
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crea dati di esempio per la dimostrazione
            worksheet.Cells["A1"].PutValue("Orders");
            worksheet.Cells["A2"].PutValue("OrderID");
            worksheet.Cells["A3"].PutValue("CustomerID");
            worksheet.Cells["A4"].PutValue("OrderDate");
            
            worksheet.Cells["C1"].PutValue("Customers");
            worksheet.Cells["C2"].PutValue("CustomerID");
            worksheet.Cells["C3"].PutValue("CustomerName");
            worksheet.Cells["C4"].PutValue("ContactName");

            // Questo dimostra l'accesso alle proprietà di una relazione esistente
            // In uno scenario reale, otterresti questo dal DataModel
            DataModelRelationship relationship = workbook.DataModel?.Relationships?[0];
            if (relationship != null)
            {
                // Visualizza le proprietà della relazione (sola lettura)
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

            // Salva la cartella di lavoro
            workbook.Save("DataModelRelationshipDemo.xlsx");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells.DataModels](../../aspose.cells.datamodels/)
* assembly [Aspose.Cells](../../)


