---
title: "Enum TableStyleElementType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Tables.TableStyleElementType enum. Representerar tabell- eller pivottabellens stil‑elementtyp."
type: docs
url: /sv/net/aspose.cells.tables/tablestyleelementtype/
---
## TableStyleElementType enumeration

Representerar typ av stil-element för tabell eller pivottabell.

```csharp
public enum TableStyleElementType
```

### Värden

| Namn | Värde | Beskrivning |
| --- | --- | --- |
| BlankRow | `18` | Stil-element för tabell som tillämpas på pivottabellens tomma rader. |
| FirstColumn | `8` | Stil-element för tabell som tillämpas på tabellens första kolumn. |
| FirstColumnStripe | `3` | Stil-element för tabell som tillämpas på tabellens första kolumnstreck. |
| FirstColumnSubheading | `22` | Tabellstilselement som gäller för PivotTable's första kolumnunderrubrik. |
| FirstHeaderCell | `11` | Tabellstilselement som gäller för tabellens första rubrikradcell. |
| FirstRowStripe | `5` | Tabellstilselement som gäller för tabellens första radens ränder. |
| FirstRowSubheading | `25` | Tabellstilselement som gäller för PivotTable's första radunderrubrik. |
| FirstSubtotalColumn | `15` | Tabellstilselement som gäller för PivotTable's första deltotalkolumn. |
| FirstSubtotalRow | `19` | Tabellstilselement som gäller för pivottabellens första deltotalrad. |
| GrandTotalColumn | `28` | Tabellstilselement som gäller för pivottabellens totalkolumn. |
| GrandTotalRow | `29` | Tabellstilselement som gäller för pivottabellens totalrad. |
| FirstTotalCell | `13` | Tabellstilselement som gäller för tabellens första totalradcell. |
| HeaderRow | `9` | Tabellstilselement som gäller för tabellens rubrikrad. |
| LastColumn | `7` | Tabellstilselement som gäller för tabellens sista kolumn. |
| LastHeaderCell | `12` | Tabellstilselement som gäller för tabellens sista rubrikradcell. |
| LastTotalCell | `14` | Tabellstilselement som gäller för tabellens sista totalradcell. |
| PageFieldLabels | `1` | Tabellstilselement som gäller för pivottabellens sidfältetiketter. |
| PageFieldValues | `2` | Tabellstilselement som gäller för pivottabellens sidfältvärden. |
| SecondColumnStripe | `4` | Tabellstilselement som gäller för tabellens andra kolumnränder. |
| SecondColumnSubheading | `23` | Tabellstilselement som gäller för pivottabellens andra kolumnunderrubrik. |
| SecondRowStripe | `6` | Tabellstilselement som gäller för tabellens andra radens ränder. |
| SecondRowSubheading | `26` | Tabellstilselement som gäller för pivottabellens andra radunderrubrik. |
| SecondSubtotalColumn | `16` | Tabellstilselement som gäller för PivotTable's andra deltotalkolumn. |
| SecondSubtotalRow | `20` | Tabellstilselement som gäller för PivotTable's andra deltotalrad. |
| ThirdColumnSubheading | `24` | Tabellstilselement som gäller för PivotTable's tredje kolumnunderrubrik. |
| ThirdRowSubheading | `27` | Tabellstilselement som gäller för PivotTable's tredje radunderrubrik. |
| ThirdSubtotalColumn | `17` | Tabellstilselement som gäller för pivottabellens tredje deltotalkolumn. |
| ThirdSubtotalRow | `21` | Tabellstilselement som gäller för PivotTable's tredje deltotalrad. |
| TotalRow | `10` | Tabellstilelement som gäller för tabellens totalsrad. |
| WholeTable | `0` | Tabellstilelement som gäller för tabellens hela innehåll. |
| LastColumnSubheading | `130` | Tabellstilelement som gäller för pivottabellens sista kolumnfält. |
| LastRowSubheading | `131` | Tabellstilelement som gäller för pivottabellens sista radfält. |
| LastSubtotalRow | `133` | Tabellstilelement som gäller för pivottabellens sista delsumme-radfält. |

### Exempel

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

### Se även

* namespace [Aspose.Cells.Tables](../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../)


