---
title: "Klass TableStyleElement"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Tables.TableStyleElement-klass. Representerar elementet i tabellstilen"
type: docs
url: /sv/net/aspose.cells.tables/tablestyleelement/
---
## TableStyleElement class

Representerar elementet i tabellstilen.

```csharp
public class TableStyleElement
```

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [Size](../../aspose.cells.tables/tablestyleelement/size/) { get; set; } | Antal rader eller kolumner i ett enda band av ränder. Gäller endast när typen är firstRowStripe, secondRowStripe, firstColumnStripe eller secondColumnStripe. |
| [Type](../../aspose.cells.tables/tablestyleelement/type/) { get; } | Hämtar elementtypen. |

## Metoder

| Namn | Beskrivning |
| --- | --- |
| [GetElementStyle](../../aspose.cells.tables/tablestyleelement/getelementstyle/)() | Hämtar elementstilen. |
| [SetElementStyle](../../aspose.cells.tables/tablestyleelement/setelementstyle/)(Style) | Ställer in elementstilen. |

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class TablesClassTableStyleElementDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            
            Style firstColumnStyle = workbook.CreateStyle();
            firstColumnStyle.Pattern = BackgroundType.Solid;
            firstColumnStyle.BackgroundColor = System.Drawing.Color.LightBlue;

            Style lastColumnStyle = workbook.CreateStyle();
            lastColumnStyle.Font.IsBold = true;
            lastColumnStyle.ForegroundColor = System.Drawing.Color.Yellow;
            lastColumnStyle.Pattern = BackgroundType.Solid;

            string tableStyleName = "CustomStyle1";
            TableStyleCollection tableStyles = workbook.Worksheets.TableStyles;
            int styleIndex = tableStyles.AddTableStyle(tableStyleName);
            TableStyle tableStyle = tableStyles[styleIndex];

            TableStyleElementCollection elements = tableStyle.TableStyleElements;
            
            int elementIndex = elements.Add(TableStyleElementType.FirstColumn);
            TableStyleElement element = elements[elementIndex];
            element.SetElementStyle(firstColumnStyle);

            elementIndex = elements.Add(TableStyleElementType.LastColumn);
            element = elements[elementIndex];
            element.SetElementStyle(lastColumnStyle);

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

            ListObjectCollection tables = workbook.Worksheets[0].ListObjects;
            int tableIndex = tables.Add(0, 0, 4, 4, true);
            ListObject table = tables[tableIndex];

            table.ShowTableStyleFirstColumn = true;
            table.ShowTableStyleLastColumn = true;
            table.TableStyleName = tableStyleName;

            workbook.Save("TableStyleElementDemo.xlsx");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells.Tables](../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../)


