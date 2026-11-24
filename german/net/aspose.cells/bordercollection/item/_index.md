---
title: "BorderCollection.Item"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "BorderCollection‑Eigenschaft. Gibt das Border‑Element am angegebenen Index zurück"
type: docs
url: /de/net/aspose.cells/bordercollection/item/
---
## BorderCollection indexer

Gibt das [`Border`](../../border/)‑Element am angegebenen Index zurück.

```csharp
public Border this[BorderType borderType] { get; }
```

| Parameter | Beschreibung |
| --- | --- |
| borderType | Der abzurufende Rand. |

### Rückgabewert

Das Element am angegebenen Index.

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class BorderCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();

            // Erstelle ein Beispiel-Arbeitsblatt
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge einige Daten hinzu, um das Beispiel sinnvoll zu machen.
            worksheet.Cells["A1"].Value = "Sample Data";

            try
            {
                // Hole die Zelle und ihren Stil.
                Cell cell = worksheet.Cells["A1"];
                Style style = cell.GetStyle();

                // Greife auf die BorderCollection aus dem Stil zu.
                BorderCollection borders = style.Borders;

                // Zeige den aktuellen Wert der Item-Eigenschaft (Lesevorgang) an.
                // Hinweis: Die Item-Eigenschaft ist schreibgeschützt und gibt ein Border-Objekt zurück.
                // Die Item-Eigenschaft erfordert einen BorderType-Parameter.
                Border border = borders[BorderType.LeftBorder];
                Console.WriteLine("Border type: " + border.LineStyle);
                Console.WriteLine("Border color: " + border.Color);

                // Ergebnis speichern
                workbook.Save("ItemDemo.xlsx");
                Console.WriteLine("Item property has been demonstrated");
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

* class [Border](../../border/)
* enum [BorderType](../../bordertype/)
* class [BorderCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


