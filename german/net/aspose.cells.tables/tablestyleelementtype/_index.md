---
title: "Aufzählung TableStyleElementType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Tables.TableStyleElementType-Enum. Stellt den Stil-Elementtyp für Tabellen oder PivotTables dar"
type: docs
url: /de/net/aspose.cells.tables/tablestyleelementtype/
---
## TableStyleElementType enumeration

Stellt den Stil-Elementtyp einer Tabelle oder PivotTable dar.

```csharp
public enum TableStyleElementType
```

### Werte

| Name | Wert | Beschreibung |
| --- | --- | --- |
| BlankRow | `18` | Tabellestil-Element, das auf leere Zeilen einer PivotTable angewendet wird. |
| FirstColumn | `8` | Tabellestil-Element, das auf die erste Spalte einer Tabelle angewendet wird. |
| FirstColumnStripe | `3` | Tabellestil-Element, das auf die Streifen der ersten Spalte einer Tabelle angewendet wird. |
| FirstColumnSubheading | `22` | Tabellestil-Element, das auf die Unterüberschrift der ersten Spalte einer PivotTable angewendet wird. |
| FirstHeaderCell | `11` | Tabellestil-Element, das auf die Zelle der ersten Kopfzeile einer Tabelle angewendet wird. |
| FirstRowStripe | `5` | Tabellestil-Element, das auf die Streifen der ersten Zeile einer Tabelle angewendet wird. |
| FirstRowSubheading | `25` | Tabellenformat-Element, das auf die erste Zeilenunterüberschrift der PivotTable angewendet wird. |
| FirstSubtotalColumn | `15` | Tabellenformat-Element, das auf die erste Zwischensummenspalte der PivotTable angewendet wird. |
| FirstSubtotalRow | `19` | Tabellenformat-Element, das auf die erste Zwischensummenzeile der Pivot-Tabelle angewendet wird. |
| GrandTotalColumn | `28` | Tabellenformat-Element, das auf die Gesamtsummenspalte der Pivot-Tabelle angewendet wird. |
| GrandTotalRow | `29` | Tabellenformat-Element, das auf die Gesamtsummenzeile der Pivot-Tabelle angewendet wird. |
| FirstTotalCell | `13` | Tabellenformat-Element, das auf die Zelle der ersten Gesamtsummenzeile der Tabelle angewendet wird. |
| HeaderRow | `9` | Tabellenformat-Element, das auf die Kopfzeile der Tabelle angewendet wird. |
| LastColumn | `7` | Tabellenformat-Element, das auf die letzte Spalte der Tabelle angewendet wird. |
| LastHeaderCell | `12` | Tabellenformat-Element, das auf die Zelle der letzten Kopfzeilenzeile der Tabelle angewendet wird. |
| LastTotalCell | `14` | Tabellenformat-Element, das auf die Zelle der letzten Gesamtsummenzeile der Tabelle angewendet wird. |
| PageFieldLabels | `1` | Tabellenformat-Element, das auf die Seitenfeldbeschriftungen der Pivot-Tabelle angewendet wird. |
| PageFieldValues | `2` | Tabellenformat-Element, das auf die Seitenfeldwerte der Pivot-Tabelle angewendet wird. |
| SecondColumnStripe | `4` | Tabellenformat-Element, das auf die Streifen der zweiten Spalte der Tabelle angewendet wird. |
| SecondColumnSubheading | `23` | Tabellenformat-Element, das auf die Unterüberschrift der zweiten Spalte der Pivot-Tabelle angewendet wird. |
| SecondRowStripe | `6` | Tabellenformat-Element, das auf die Streifen der zweiten Zeile der Tabelle angewendet wird. |
| SecondRowSubheading | `26` | Tabellenformat-Element, das auf die Unterüberschrift der zweiten Zeile der Pivot-Tabelle angewendet wird. |
| SecondSubtotalColumn | `16` | Tabellenformat-Element, das auf die zweite Zwischensummenspalte der PivotTable angewendet wird. |
| SecondSubtotalRow | `20` | Tabellenformat-Element, das auf die zweite Zwischensummenzeile der PivotTable angewendet wird. |
| ThirdColumnSubheading | `24` | Tabellenformat-Element, das auf die Unterüberschrift der dritten Spalte der PivotTable angewendet wird. |
| ThirdRowSubheading | `27` | Tabellenformat-Element, das auf die Unterüberschrift der dritten Zeile der PivotTable angewendet wird. |
| ThirdSubtotalColumn | `17` | Tabellenformat-Element, das auf die dritte Zwischensummenspalte der Pivot-Tabelle angewendet wird. |
| ThirdSubtotalRow | `21` | Tabellenformat-Element, das auf die dritte Zwischensummenzeile der PivotTable angewendet wird. |
| TotalRow | `10` | Tabellenformat-Element, das auf die Gesamtsummenzeile von Table angewendet wird. |
| WholeTable | `0` | Tabellenformat-Element, das auf den gesamten Inhalt der Tabelle angewendet wird. |
| LastColumnSubheading | `130` | Tabellenformat-Element, das auf das letzte Spaltenfeld der Pivot-Tabelle angewendet wird. |
| LastRowSubheading | `131` | Tabellenstil-Element, das auf das letzte Zeilenfeld der Pivot-Tabelle angewendet wird. |
| LastSubtotalRow | `133` | Tabellenstil-Element, das auf das letzte Zwischensummen-Zeilenfeld der Pivot-Tabelle angewendet wird. |

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class TablesClassTableStyleElementTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            
            Style firstColumnStyle = workbook.CreateStyle();
            firstColumnStyle.Pattern = BackgroundType.Solid;
            firstColumnStyle.ForegroundColor = System.Drawing.Color.LightBlue;
            
            Style lastColumnStyle = workbook.CreateStyle();
            lastColumnStyle.Font.IsBold = true;
            lastColumnStyle.Pattern = BackgroundType.Solid;
            lastColumnStyle.ForegroundColor = System.Drawing.Color.LightGreen;

            string tableStyleName = "CustomStyle1";
            TableStyleCollection tableStyles = workbook.Worksheets.TableStyles;
            int styleIndex = tableStyles.AddTableStyle(tableStyleName);
            TableStyle tableStyle = tableStyles[styleIndex];

            TableStyleElementCollection elements = tableStyle.TableStyleElements;
            
            int elementIndex = elements.Add(TableStyleElementType.FirstColumn);
            elements[elementIndex].SetElementStyle(firstColumnStyle);
            
            elementIndex = elements.Add(TableStyleElementType.LastColumn);
            elements[elementIndex].SetElementStyle(lastColumnStyle);

            Cells cells = workbook.Worksheets[0].Cells;
            for (int i = 0; i < 5; i++)
            {
                cells[0, i].PutValue($"Column {i + 1}");
            }

            for (int row = 1; row < 5; row++)
            {
                for (int col = 0; col < 5; col++)
                {
                    cells[row, col].PutValue(row * col);
                }
            }

            ListObject table = workbook.Worksheets[0].ListObjects[workbook.Worksheets[0].ListObjects.Add(0, 0, 4, 4, true)];
            table.ShowTableStyleFirstColumn = true;
            table.ShowTableStyleLastColumn = true;
            table.TableStyleName = tableStyleName;

            workbook.Save("TableStyleDemo.xlsx");
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells.Tables](../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../)


