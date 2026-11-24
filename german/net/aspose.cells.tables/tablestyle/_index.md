---
title: "Klasse TableStyle"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Tables.TableStyle Klasse. Stellt den Stil der Tabelle dar"
type: docs
url: /de/net/aspose.cells.tables/tablestyle/
---
## TableStyle class

Stellt den Stil der Tabelle dar.

```csharp
public class TableStyle
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [Name](../../aspose.cells.tables/tablestyle/name/) { get; } | Liest den Namen des Tabellenstils. |
| [TableStyleElements](../../aspose.cells.tables/tablestyle/tablestyleelements/) { get; } | Liest alle Elemente des Tabellenstils. |

## Methoden

| Name | Beschreibung |
| --- | --- |
| static [Create](../../aspose.cells.tables/tablestyle/create/)(string, WorksheetCollection) | Erstellt einen leeren Tabellen-/Pivot-Tabellenstil. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Tables;
    using System;

    public class TableStyleDemo
    {
        public static void TableStyleExample()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();

            // Erstelle Stile für die erste und letzte Spalte
            Style firstColumnStyle = workbook.CreateStyle();
            firstColumnStyle.Pattern = BackgroundType.Solid;
            firstColumnStyle.BackgroundColor = System.Drawing.Color.Red;

            Style lastColumnStyle = workbook.CreateStyle();
            lastColumnStyle.Font.IsBold = true;
            lastColumnStyle.Pattern = BackgroundType.Solid;
            lastColumnStyle.BackgroundColor = System.Drawing.Color.Red;

            // Definiere einen benutzerdefinierten Tabellestilnamen
            string tableStyleName = "Custom1";

            // Greife auf die Sammlung der Tabellestile zu
            TableStyleCollection tableStyles = workbook.Worksheets.TableStyles;

            // Fügen Sie der Sammlung einen neuen Tabellestil hinzu
            int index1 = tableStyles.AddTableStyle(tableStyleName);
            TableStyle tableStyle = tableStyles[index1];

            // Greifen Sie auf die Sammlung der Tabellestil-Elemente zu
            TableStyleElementCollection elements = tableStyle.TableStyleElements;

            // Hinzufügen und Stil für die erste Spalte festlegen
            index1 = elements.Add(TableStyleElementType.FirstColumn);
            TableStyleElement element = elements[index1];
            element.SetElementStyle(firstColumnStyle);

            // Hinzufügen und Stil für die letzte Spalte festlegen
            index1 = elements.Add(TableStyleElementType.LastColumn);
            element = elements[index1];
            element.SetElementStyle(lastColumnStyle);

            // Zugriff auf die Zellen des ersten Arbeitsblatts
            Cells cells = workbook.Worksheets[0].Cells;

            // Fülle die erste Zeile mit Spaltennamen
            for (int i = 0; i < 5; i++)
            {
                cells[0, i].PutValue(CellsHelper.ColumnIndexToName(i));
            }

            // Fülle die restlichen Zellen mit Beispieldaten
            for (int row = 1; row < 10; row++)
            {
                for (int column = 0; column < 5; column++)
                {
                    cells[row, column].PutValue(row * column);
                }
            }

            // Fügen Sie dem Arbeitsblatt eine Tabelle hinzu
            ListObjectCollection tables = workbook.Worksheets[0].ListObjects;
            int index = tables.Add(0, 0, 9, 4, true);
            ListObject table = tables[index];

            // Wenden Sie den benutzerdefinierten Tabellestil auf die Tabelle an
            table.ShowTableStyleFirstColumn = true;
            table.ShowTableStyleLastColumn = true;
            table.TableStyleName = tableStyleName;

            // Speichere die Arbeitsmappe
            workbook.Save("TableStyleExample.xlsx");
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells.Tables](../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../)


