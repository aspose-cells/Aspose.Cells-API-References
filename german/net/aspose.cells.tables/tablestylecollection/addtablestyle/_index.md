---
title: "TableStyleCollection.AddTableStyle"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "TableStyleCollection-Methode. Fügt einen benutzerdefinierten Tabellenstil hinzu"
type: docs
url: /de/net/aspose.cells.tables/tablestylecollection/addtablestyle/
---
## TableStyleCollection.AddTableStyle method

Fügt einen benutzerdefinierten Tabellenstil hinzu.

```csharp
public int AddTableStyle(string name)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Name | String | Der Tabellenstilname. |

### Rückgabewert

Der Index des Tabellenstils.

### Beispiele

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

            // Erstelle Beispieldaten
            for (int i = 0; i < 5; i++)
            {
                worksheet.Cells[0, i].PutValue("Header " + (i + 1));
                for (int row = 1; row < 6; row++)
                {
                    worksheet.Cells[row, i].PutValue(row * (i + 1));
                }
            }

            // Erstelle einen benutzerdefinierten Tabellenstil
            string styleName = "MyCustomStyle";
            TableStyleCollection tableStyles = workbook.Worksheets.TableStyles;
            int styleIndex = tableStyles.AddTableStyle(styleName);
            TableStyle tableStyle = tableStyles[styleIndex];

            // Stil für die Kopfzeile festlegen
            Style headerStyle = workbook.CreateStyle();
            headerStyle.Font.IsBold = true;
            headerStyle.ForegroundColor = System.Drawing.Color.LightBlue;
            headerStyle.Pattern = BackgroundType.Solid;

            tableStyle.TableStyleElements.Add(TableStyleElementType.HeaderRow);
            TableStyleElement headerElement = tableStyle.TableStyleElements[TableStyleElementType.HeaderRow];
            headerElement.SetElementStyle(headerStyle);

            // Stil für die erste Spalte festlegen
            Style firstColStyle = workbook.CreateStyle();
            firstColStyle.Font.Color = System.Drawing.Color.Red;

            tableStyle.TableStyleElements.Add(TableStyleElementType.FirstColumn);
            TableStyleElement firstColElement = tableStyle.TableStyleElements[TableStyleElementType.FirstColumn];
            firstColElement.SetElementStyle(firstColStyle);

            // Erstelle eine Tabelle mit dem benutzerdefinierten Stil
            int tableIndex = worksheet.ListObjects.Add(0, 0, 5, 4, true);
            ListObject table = worksheet.ListObjects[tableIndex];
            table.TableStyleName = styleName;
            table.ShowTableStyleFirstColumn = true;

            workbook.Save("CustomTableStyleDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [TableStyleCollection](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


