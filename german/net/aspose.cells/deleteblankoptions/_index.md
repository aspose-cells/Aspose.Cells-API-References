---
title: "Klasse DeleteBlankOptions"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.DeleteBlankOptions‑Klasse. Stellt die Einstellung zum Löschen leerer Zellen/Zeilen/Spalten dar."
type: docs
url: /de/net/aspose.cells/deleteblankoptions/
---
## DeleteBlankOptions class

Stellt die Einstellung zum Löschen leerer Zellen/Zeilen/Spalten dar.

```csharp
public class DeleteBlankOptions : DeleteOptions
```

## Konstruktoren

| Name | Beschreibung |
| --- | --- |
| [DeleteBlankOptions](deleteblankoptions/)() | Der Standardkonstruktor. |

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [DrawingsAsBlank](../../aspose.cells/deleteblankoptions/drawingsasblank/) { get; set; } | Gibt an, ob zeichnungsbezogene Objekte wie Bild, Form, Diagramm… als leer betrachtet werden. Standardwert ist true. |
| [EmptyFormulaValueAsBlank](../../aspose.cells/deleteblankoptions/emptyformulavalueasblank/) { get; set; } | Ob eine Zelle als leer betrachtet wird, wenn sie eine Formel ist und das berechnete Ergebnis null oder ein leerer String ist. Standardwert ist false. |
| [EmptyStringAsBlank](../../aspose.cells/deleteblankoptions/emptystringasblank/) { get; set; } | Gibt an, ob eine Zelle als leer betrachtet wird, wenn ihr Wert ein leerer String ist. Standardwert ist true. |
| [EndIndex](../../aspose.cells/deleteblankoptions/endindex/) { get; set; } | Gibt den End‑Zeilen‑/Spalten‑Index (einschließlich) des zu prüfenden Bereichs zum Löschen leerer Zeilen/Spalten an. Standardwert ist -1, wobei -1 den maximalen Bereich aller zu prüfenden Objekte (Zellen, Zeichnungen, …) bedeutet. |
| [FormulaChangeMonitor](../../aspose.cells/deleteoptions/formulachangemonitor/) { get; set; } | Ruft den Monitor zum Verfolgen von Änderungen durch das Löschen ab bzw. setzt ihn. (Vererbt von [`DeleteOptions`](../deleteoptions/).) |
| [MergedCellsShrinkType](../../aspose.cells/deleteblankoptions/mergedcellsshrinktype/) { get; set; } | Gibt an, wie zusammengeführte Zellen beim Löschen leerer Zeilen/Spalten verarbeitet werden. |
| [StartIndex](../../aspose.cells/deleteblankoptions/startindex/) { get; set; } | Gibt den Start‑Zeilen‑/Spalten‑Index des zu prüfenden Bereichs zum Löschen leerer Zeilen/Spalten an. |
| [UpdateReference](../../aspose.cells/deleteoptions/updatereference/) { get; set; } | Gibt an, ob Verweise in anderen Arbeitsblättern aktualisiert werden. (Vererbt von [`DeleteOptions`](../deleteoptions/).) |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class DeleteBlankOptionsDemo
    {
        public static void DeleteBlankOptionsExample()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fülle das Arbeitsblatt mit einigen Daten
            worksheet.Cells["A1"].PutValue("Data");
            worksheet.Cells["A2"].PutValue("");
            worksheet.Cells["A3"].PutValue("More Data");
            worksheet.Cells["A4"].PutValue("");
            worksheet.Cells["A5"].PutValue("Even More Data");

            // Erstelle eine Instanz von DeleteBlankOptions
            DeleteBlankOptions options = new DeleteBlankOptions
            {
                EmptyStringAsBlank = true,
                EmptyFormulaValueAsBlank = false,
                UpdateReference = true
            };

            // Leere Zeilen basierend auf den Optionen löschen
            worksheet.Cells.DeleteBlankRows(options);

            // Speichere die Arbeitsmappe
            workbook.Save("DeleteBlankOptionsExample.xlsx");
            workbook.Save("DeleteBlankOptionsExample.pdf");
            return;
        }
    }
}
```

### Siehe auch

* class [DeleteOptions](../deleteoptions/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


