---
title: "Klasse PasteOptions"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.PasteOptions Klasse. Stellt die Optionen für Spezial‑Einfügen dar"
type: docs
url: /de/net/aspose.cells/pasteoptions/
---
## PasteOptions class

Stellt die Optionen für Einfügen Speziell dar.

```csharp
public class PasteOptions
```

## Konstruktoren

| Name | Beschreibung |
| --- | --- |
| [PasteOptions](pasteoptions/)() | Der Standardkonstruktor. |

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [IgnoreLinksToOriginalFile](../../aspose.cells/pasteoptions/ignorelinkstooriginalfile/) { get; set; } | Ignoriere Links zur Originaldatei. |
| [KeepOldTables](../../aspose.cells/pasteoptions/keepoldtables/) { get; set; } | Behält die Tabellen im Zielbereich bei. |
| [OnlyVisibleCells](../../aspose.cells/pasteoptions/onlyvisiblecells/) { get; set; } | True bedeutet, dass nur sichtbare Zellen kopiert werden. |
| [OperationType](../../aspose.cells/pasteoptions/operationtype/) { get; set; } | Liest und setzt den Operationstyp beim Einfügen des Bereichs. |
| [PasteType](../../aspose.cells/pasteoptions/pastetype/) { get; set; } | Der Spezial‑Einfügetyp. |
| [ShiftFormulasOfShapes](../../aspose.cells/pasteoptions/shiftformulasofshapes/) { get; set; } | Gibt an, ob Formeln der Formen beim Kopieren von Bereichen verschoben werden sollen. |
| [SkipBlanks](../../aspose.cells/pasteoptions/skipblanks/) { get; set; } | Gibt an, ob leere Zellen übersprungen werden. |
| [Transpose](../../aspose.cells/pasteoptions/transpose/) { get; set; } | True, um Zeilen und Spalten beim Einfügen des Bereichs zu transponieren. Der Standardwert ist False. |

### Beispiele

```csharp
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PasteOptionsDemo
    {
        public static void PasteOptionsExample()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Füge einige Daten zum ersten Arbeitsblatt hinzu
            sheet.Cells["A1"].PutValue("Hello");
            sheet.Cells["A2"].PutValue("World");
            sheet.Cells["A3"].PutValue(123);

            // Erstelle ein weiteres Arbeitsblatt
            Worksheet sheet2 = workbook.Worksheets.Add("Sheet2");

            // Quellbereich definieren
            Aspose.Cells.Range sourceRange = sheet.Cells.CreateRange("A1:A3");

            // Zielbereich definieren
            Aspose.Cells.Range destRange = sheet2.Cells.CreateRange("B1:B3");

            // Erstelle ein PasteOptions‑Objekt
            PasteOptions pasteOptions = new PasteOptions
            {
                PasteType = PasteType.Values,
                SkipBlanks = true,
                OnlyVisibleCells = false,
                Transpose = false,
                OperationType = PasteOperationType.None,
                IgnoreLinksToOriginalFile = true
            };

            // Kopiere den Bereich mit den angegebenen Einfügeoptionen
            destRange.Copy(sourceRange, pasteOptions);

            // Speichere die Arbeitsmappe
            workbook.Save("PasteOptionsExample.xlsx");
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


