---
title: "FindOptions.ConvertNumericData"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "FindOptions‑Eigenschaft. Gibt einen Wert zurück oder legt ihn fest, der angibt, ob der gesuchte Zeichenkettenwert in numerische Daten konvertiert wird"
type: docs
url: /de/net/aspose.cells/findoptions/convertnumericdata/
---
## FindOptions.ConvertNumericData property

Liest oder setzt einen Wert, der angibt, ob der gesuchte Zeichenfolgenwert in numerische Daten konvertiert wird.

```csharp
public bool ConvertNumericData { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FindOptionsPropertyConvertNumericDataDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge Beispieldaten hinzu, die numerische Werte als Zeichenketten enthalten
            worksheet.Cells["A1"].PutValue("123");
            worksheet.Cells["A2"].PutValue("456");
            worksheet.Cells["A3"].PutValue("01/28/2010");

            // Erstelle FindOptions und setze ConvertNumericData auf true
            FindOptions options = new FindOptions();
            options.ConvertNumericData = true;

            // Finde den Datumswert (als Zeichenkette gespeichert, aber während der Suche in numerisch konvertiert)
            Cell foundCell = worksheet.Cells.Find("01/28/2010", null, options);

            // Gib das Ergebnis aus
            if (foundCell != null)
            {
                Console.WriteLine("Found value at: " + foundCell.Name);
                Console.WriteLine("Cell value: " + foundCell.StringValue);
            }
            else
            {
                Console.WriteLine("Value not found");
            }
        }
    }
}
```

### Siehe auch

* class [FindOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


