---
title: "DataModelRelationship.ForeignKeyColumn"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "DataModelRelationship-Eigenschaft. Ruft den Namen der Fremdschlüssel-Tabellenspalte für diese Beziehung ab"
type: docs
url: /de/net/aspose.cells.datamodels/datamodelrelationship/foreignkeycolumn/
---
## DataModelRelationship.ForeignKeyColumn property

Ermittelt den Namen der Fremdschlüssel-Tabellenspalte für diese Beziehung.

```csharp
public string ForeignKeyColumn { get; }
```

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fügen Sie Beispieldaten hinzu, um einen sinnvollen Kontext zu erstellen
            worksheet.Cells["A1"].PutValue("Orders");
            worksheet.Cells["A2"].PutValue("OrderID");
            worksheet.Cells["A3"].PutValue("CustomerID");

            worksheet.Cells["C1"].PutValue("Customers");
            worksheet.Cells["C2"].PutValue("CustomerID");
            worksheet.Cells["C3"].PutValue("CustomerName");

            try
            {
                // Greifen Sie auf die erste Beziehung zu, falls sie existiert
                DataModelRelationship relationship = workbook.DataModel?.Relationships?[0];

                if (relationship != null)
                {
                    // Anzeige des ForeignKeyColumn-Eigenschaftswerts (schreibgeschützt)
                    Console.WriteLine("Foreign Key Column: " + relationship.ForeignKeyColumn);
                }
                else
                {
                    Console.WriteLine("No relationships found in the data model.");
                }

                // Speichere die Arbeitsmappe
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

### Siehe auch

* class [DataModelRelationship](../)
* namespace [Aspose.Cells.DataModels](../../../aspose.cells.datamodels/)
* assembly [Aspose.Cells](../../../)


