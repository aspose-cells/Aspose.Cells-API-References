---
title: "TableStyle.Name"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "TableStyle-Eigenschaft. Gibt den Namen des Tabellenstils zurück"
type: docs
url: /de/net/aspose.cells.tables/tablestyle/name/
---
## TableStyle.Name property

Liest den Namen des Tabellenstils.

```csharp
public string Name { get; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Tables;
    using System;

    public class TableStylePropertyNameDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();

            // Greife auf die Sammlung der Tabellestile zu
            TableStyleCollection tableStyles = workbook.Worksheets.TableStyles;

            try
            {
                // Rufe den ersten Tabellenstil aus der Sammlung ab
                TableStyle tableStyle = tableStyles[0];

                // Anzeige des Werts der Eigenschaft Name
                Console.WriteLine("Table Style Name: " + tableStyle.Name);

                // Demonstriere den Zugriff auf die schreibgeschützte Eigenschaft
                string styleName = tableStyle.Name;
                Console.WriteLine("Retrieved style name: " + styleName);

                // Zeige, dass wir den Namen verwenden können, um auf den Stil zu verweisen
                Console.WriteLine("This table style can be referenced by name: " + tableStyle.Name);

                // Speichere die Arbeitsmappe
                workbook.Save("TableStyleNameDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
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

* class [TableStyle](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


