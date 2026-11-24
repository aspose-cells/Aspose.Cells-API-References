---
title: "DataModelRelationship.PrimaryKeyTable"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "DataModelRelationship-Eigenschaft. Ruft den Namen der Primärschlüssel-Tabelle für diese Beziehung ab"
type: docs
url: /de/net/aspose.cells.datamodels/datamodelrelationship/primarykeytable/
---
## DataModelRelationship.PrimaryKeyTable property

Ermittelt den Namen der Primärschlüssel-Tabelle für diese Beziehung.

```csharp
public string PrimaryKeyTable { get; }
```

### Beispiele

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
                    // Zeigen Sie den Wert der PrimaryKeyTable-Eigenschaft (schreibgeschützt) an
                    Console.WriteLine("Primary Key Table: " + relationship.PrimaryKeyTable);
                }
                else
                {
                    Console.WriteLine("No relationships found in the data model.");
                }

                // Speichere die Arbeitsmappe
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

### Siehe auch

* class [DataModelRelationship](../)
* namespace [Aspose.Cells.DataModels](../../../aspose.cells.datamodels/)
* assembly [Aspose.Cells](../../../)


