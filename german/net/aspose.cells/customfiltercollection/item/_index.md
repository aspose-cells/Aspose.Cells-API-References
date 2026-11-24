---
title: "CustomFilterCollection.Item"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "CustomFilterCollection-Eigenschaft. Gibt den benutzerdefinierten Filter am angegebenen Index zurück"
type: docs
url: /de/net/aspose.cells/customfiltercollection/item/
---
## CustomFilterCollection indexer

Liefert den benutzerdefinierten Filter am angegebenen Index.

```csharp
public CustomFilter this[int index] { get; }
```

| Parameter | Beschreibung |
| --- | --- |
| Index | Der Index. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CustomFilterCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fügen Sie Beispieldaten hinzu
            worksheet.Cells["A1"].Value = "Numbers";
            worksheet.Cells["A2"].Value = 10;
            worksheet.Cells["A3"].Value = 20;
            worksheet.Cells["A4"].Value = 30;
            worksheet.Cells["A5"].Value = 40;
            worksheet.Cells["A6"].Value = 50;

            try
            {
                // Erstellen Sie eine neue CustomFilterCollection
                CustomFilterCollection filters = new CustomFilterCollection();

                // Greifen Sie über den Indexer auf die Item-Eigenschaft (schreibgeschützt) zu
                // Da die Sammlung leer ist, zeigen wir nur das Zugreifen auf die Eigenschaft
                // In einem realen Szenario würden Sie zunächst Filter auf andere Weise hinzufügen
                if (filters.Count > 0)
                {
                    CustomFilter firstFilter = filters[0];
                    Console.WriteLine($"First filter operator: {firstFilter.FilterOperatorType}");
                    Console.WriteLine($"First filter criteria: {firstFilter.Criteria}");
                }
                else
                {
                    Console.WriteLine("No filters in collection to demonstrate Item property");
                }

                // Speichere die Arbeitsmappe
                workbook.Save("CustomFilterCollectionItemDemo.xlsx");
                Console.WriteLine("CustomFilterCollection Item property demonstrated successfully");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error demonstrating Item property: {ex.Message}");
            }
        }
    }
}
```

### Siehe auch

* class [CustomFilter](../../customfilter/)
* class [CustomFilterCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


