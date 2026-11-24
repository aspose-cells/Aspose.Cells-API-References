---
title: "Klasse DataModelRelationship"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.DataModels.DataModelRelationship Klasse. Stellt eine einzelne Beziehung im Tabellenkalkulationsdatenmodell dar"
type: docs
url: /de/net/aspose.cells.datamodels/datamodelrelationship/
---
## DataModelRelationship class

Stellt eine einzelne Beziehung im Datenmodell der Tabellenkalkulation dar.

```csharp
public class DataModelRelationship
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [ForeignKeyColumn](../../aspose.cells.datamodels/datamodelrelationship/foreignkeycolumn/) { get; } | Ermittelt den Namen der Fremdschlüssel-Tabellenspalte für diese Beziehung. |
| [ForeignKeyTable](../../aspose.cells.datamodels/datamodelrelationship/foreignkeytable/) { get; } | Ermittelt den Namen der Fremdschlüssel-Tabelle für diese Beziehung. |
| [PrimaryKeyColumn](../../aspose.cells.datamodels/datamodelrelationship/primarykeycolumn/) { get; } | Ermittelt den Namen der Primärschlüssel-Tabellenspalte für diese Beziehung. |
| [PrimaryKeyTable](../../aspose.cells.datamodels/datamodelrelationship/primarykeytable/) { get; } | Ermittelt den Namen der Primärschlüssel-Tabelle für diese Beziehung. |

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Erstelle Beispieldaten zur Demonstration
            worksheet.Cells["A1"].PutValue("Orders");
            worksheet.Cells["A2"].PutValue("OrderID");
            worksheet.Cells["A3"].PutValue("CustomerID");
            worksheet.Cells["A4"].PutValue("OrderDate");
            
            worksheet.Cells["C1"].PutValue("Customers");
            worksheet.Cells["C2"].PutValue("CustomerID");
            worksheet.Cells["C3"].PutValue("CustomerName");
            worksheet.Cells["C4"].PutValue("ContactName");

            // Dies demonstriert den Zugriff auf die Eigenschaften einer bestehenden Beziehung
            // In einem realen Szenario würden Sie dies aus dem DataModel erhalten
            DataModelRelationship relationship = workbook.DataModel?.Relationships?[0];
            if (relationship != null)
            {
                // Anzeige der Beziehungseigenschaften (schreibgeschützt)
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

            // Speichere die Arbeitsmappe
            workbook.Save("DataModelRelationshipDemo.xlsx");
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells.DataModels](../../aspose.cells.datamodels/)
* assembly [Aspose.Cells](../../)


