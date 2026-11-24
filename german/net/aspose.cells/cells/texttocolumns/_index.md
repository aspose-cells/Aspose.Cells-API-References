---
title: "Cells.TextToColumns"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Cells-Methode. Teilt den Inhalt in der angegebenen Spalte in mehrere Spalten auf"
type: docs
url: /de/net/aspose.cells/cells/texttocolumns/
---
## Cells.TextToColumns method

Teilt den Inhalt in der angegebenen Spalte in mehrere Spalten auf..

```csharp
public int TextToColumns(int row, int column, int totalRows, TxtLoadOptions options)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| row | Int32 | Der Zeilenindex. |
| column | Int32 | Der Spaltenindex. |
| totalRows | Int32 | Die Anzahl der Zeilen. |
| Optionen | TxtLoadOptions | Die Aufteilungsoptionen. |

### Rückgabewert

Gesamtzahl der Spalten der aufgeteilten Werte.

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodTextToColumnsWithInt32Int32Int32TxtLoadOptionsDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Setze Beispieldaten mit kommagetrennten Werten
            sheet.Cells["A1"].PutValue("John,Doe,30");
            sheet.Cells["A2"].PutValue("Jane,Smith,28");

            // Erstelle Text-Ladeoptionen mit Komma als Trennzeichen
            TxtLoadOptions options = new TxtLoadOptions();
            options.Separator = ',';

            // Teile Text in Spalten, beginnend bei Zelle A1, 3 Spalten breit
            sheet.Cells.TextToColumns(0, 0, 3, options);

            // Ergebnisse überprüfen.
            Console.WriteLine("B1: " + sheet.Cells["B1"].StringValue); // Should output "Doe"
            Console.WriteLine("C2: " + sheet.Cells["C2"].StringValue); // Should output "28"

            // Speichere die Arbeitsmappe
            workbook.Save("output.xlsx");
        }
    }
}
```

### Siehe auch

* class [TxtLoadOptions](../../txtloadoptions/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


