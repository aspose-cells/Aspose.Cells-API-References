---
title: "TableStyleCollection.AddTableStyle"
second_title: "Aspose.Cells för .NET API‑referens"
description: "TableStyleCollection-metod. Lägger till en anpassad tabellstil"
type: docs
url: /sv/net/aspose.cells.tables/tablestylecollection/addtablestyle/
---
## TableStyleCollection.AddTableStyle method

Lägger till en anpassad tabellstil.

```csharp
public int AddTableStyle(string name)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| namn | String | Tabellstilens namn. |

### Returvärde

Index för tabellstilen.

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class TableStyleCollectionMethodAddTableStyleWithStringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Skapa exempeldata
            for (int i = 0; i < 5; i++)
            {
                worksheet.Cells[0, i].PutValue("Header " + (i + 1));
                for (int row = 1; row < 6; row++)
                {
                    worksheet.Cells[row, i].PutValue(row * (i + 1));
                }
            }

            // Skapa en anpassad tabellstil
            string styleName = "MyCustomStyle";
            TableStyleCollection tableStyles = workbook.Worksheets.TableStyles;
            int styleIndex = tableStyles.AddTableStyle(styleName);
            TableStyle tableStyle = tableStyles[styleIndex];

            // Styla rubrikraden
            Style headerStyle = workbook.CreateStyle();
            headerStyle.Font.IsBold = true;
            headerStyle.ForegroundColor = System.Drawing.Color.LightBlue;
            headerStyle.Pattern = BackgroundType.Solid;

            tableStyle.TableStyleElements.Add(TableStyleElementType.HeaderRow);
            TableStyleElement headerElement = tableStyle.TableStyleElements[TableStyleElementType.HeaderRow];
            headerElement.SetElementStyle(headerStyle);

            // Styla den första kolumnen
            Style firstColStyle = workbook.CreateStyle();
            firstColStyle.Font.Color = System.Drawing.Color.Red;

            tableStyle.TableStyleElements.Add(TableStyleElementType.FirstColumn);
            TableStyleElement firstColElement = tableStyle.TableStyleElements[TableStyleElementType.FirstColumn];
            firstColElement.SetElementStyle(firstColStyle);

            // Skapa en tabell med den anpassade stilen
            int tableIndex = worksheet.ListObjects.Add(0, 0, 5, 4, true);
            ListObject table = worksheet.ListObjects[tableIndex];
            table.TableStyleName = styleName;
            table.ShowTableStyleFirstColumn = true;

            workbook.Save("CustomTableStyleDemo.xlsx");
        }
    }
}
```

### Se även

* class [TableStyleCollection](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


