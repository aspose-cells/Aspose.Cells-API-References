---
title: "Enum TotalsCalculation"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Tables.TotalsCalculation enum. Bestimmt den Typ der Berechnung in der Totals‑Zeile der Listenspalte"
type: docs
url: /de/net/aspose.cells.tables/totalscalculation/
---
## TotalsCalculation enumeration

Bestimmt den Berechnungstyp in der Gesamtsumme‑Zeile der Listenspalte.

```csharp
public enum TotalsCalculation
```

### Werte

| Name | Wert | Beschreibung |
| --- | --- | --- |
| Sum | `6` | Stellt die Summen‑Totals‑Berechnung dar. |
| Count | `2` | Stellt die Zähl‑Totals‑Berechnung dar. |
| Average | `1` | Stellt die Durchschnitts‑Totals‑Berechnung dar. |
| Max | `4` | Stellt die Max‑Totals‑Berechnung dar. |
| Min | `5` | Stellt die Min‑Totals‑Berechnung dar. |
| Var | `8` | Stellt die Var‑Totals‑Berechnung dar. |
| CountNums | `3` | Stellt die Zähl‑Nummern‑Totals‑Berechnung dar. |
| StdDev | `7` | Stellt die StdDev‑Totals‑Berechnung dar. |
| None | `0` | Stellt die Keine‑Totals‑Berechnung dar. |
| Custom | `9` | Stellt eine benutzerdefinierte Berechnung dar. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Tables;
    using System;

    public class TotalsCalculationDemo
    {
        public static void TotalsCalculationExample()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;

            // Fülle das Arbeitsblatt mit einigen Daten
            for (int i = 0; i < 5; i++)
            {
                cells[0, i].PutValue(CellsHelper.ColumnIndexToName(i));
            }
            for (int row = 1; row < 10; row++)
            {
                for (int column = 0; column < 4; column++)
                {
                    cells[row, column].PutValue(row * column);
                }
            }

            // Fügen Sie dem Arbeitsblatt eine Tabelle hinzu
            ListObjectCollection tables = workbook.Worksheets[0].ListObjects;
            int index = tables.Add(0, 0, 9, 4, true);
            ListObject table = tables[index];

            // Totals‑Zeile anzeigen
            table.ShowTotals = true;

            // Zugriff auf die fünfte Spalte in der Tabelle
            ListColumn listColumn = table.ListColumns[4];

            // Setze die TotalsCalculation‑Eigenschaft auf Summe
            listColumn.TotalsCalculation = TotalsCalculation.Sum;

            // Optional eine Formel für die Spalte festlegen
            listColumn.Formula = "=[A]";

            // Speichere die Arbeitsmappe
            workbook.Save("TotalsCalculationExample.xlsx");
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells.Tables](../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../)


