---
title: "Klasse ListColumn"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Tables.ListColumn Klasse. Stellt eine Spalte in einer Tabelle dar"
type: docs
url: /de/net/aspose.cells.tables/listcolumn/
---
## ListColumn class

Stellt eine Spalte in einer Tabelle dar.

```csharp
public class ListColumn
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [Formula](../../aspose.cells.tables/listcolumn/formula/) { get; set; } | Liefert und setzt die Formel der Listenspalte. |
| [IsArrayFormula](../../aspose.cells.tables/listcolumn/isarrayformula/) { get; } | Gibt an, ob die Formel eine Array-Formel ist. |
| [Name](../../aspose.cells.tables/listcolumn/name/) { get; set; } | Liefert und setzt den Namen der Spalte. |
| [Range](../../aspose.cells.tables/listcolumn/range/) { get; } | Liefert den Bereich dieser Listenspalte. |
| [TotalsCalculation](../../aspose.cells.tables/listcolumn/totalscalculation/) { get; set; } | Liefert und setzt den Berechnungstyp in der Gesamtsummenzeile der Listenspalte. |
| [TotalsRowLabel](../../aspose.cells.tables/listcolumn/totalsrowlabel/) { get; set; } | Liefert und setzt die Anzeigeetiketten der Gesamtsummenzeile. |

## Methoden

| Name | Beschreibung |
| --- | --- |
| [GetCustomCalculatedFormula](../../aspose.cells.tables/listcolumn/getcustomcalculatedformula/)(bool, bool) | Liefert die Formel dieser Listenspalte. |
| [GetCustomTotalsRowFormula](../../aspose.cells.tables/listcolumn/getcustomtotalsrowformula/)(bool, bool) | Liefert die Formel der Gesamtsummenzeile dieser Listenspalte. |
| [GetDataStyle](../../aspose.cells.tables/listcolumn/getdatastyle/)() | Liefert den Stil der Daten in dieser Spalte der Tabelle. |
| [SetCustomCalculatedFormula](../../aspose.cells.tables/listcolumn/setcustomcalculatedformula/)(string, bool, bool) | Setzt die Formel für diese Listenspalte. |
| [SetCustomTotalsRowFormula](../../aspose.cells.tables/listcolumn/setcustomtotalsrowformula/)(string, bool, bool) | Liefert die Formel der Gesamtsummenzeile dieser Listenspalte. |
| [SetDataStyle](../../aspose.cells.tables/listcolumn/setdatastyle/)(Style) | Setzt den Stil der Daten in dieser Spalte der Tabelle. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Tables;
    using System;

    public class ListColumnDemo
    {
        public static void ListColumnExample()
        {
            // Erstelle eine neue Arbeitsmappe und greife auf das erste Arbeitsblatt zu
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

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

            // Füge ein ListObject (Tabelle) zum Arbeitsblatt hinzu
            ListObjectCollection tables = worksheet.ListObjects;
            int index = tables.Add(0, 0, 9, 4, true);
            ListObject table = tables[index];
            table.ShowTotals = true;

            // Greife auf die ListColumn zu und setze ihre Eigenschaften
            ListColumn listColumn = table.ListColumns[4];
            listColumn.TotalsCalculation = TotalsCalculation.Sum;
            listColumn.Formula = "=[A]";
            listColumn.Name = "CustomColumn";
            listColumn.TotalsRowLabel = "Total";

            // Speichere die Arbeitsmappe
            workbook.Save("ListColumnExample.xlsx");
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells.Tables](../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../)


