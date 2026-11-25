---
title: "TableStyleCollection.AddTableStyle"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo TableStyleCollection. Aggiunge uno stile di tabella personalizzato"
type: docs
url: /it/net/aspose.cells.tables/tablestylecollection/addtablestyle/
---
## TableStyleCollection.AddTableStyle method

Aggiunge uno stile personalizzato per la tabella.

```csharp
public int AddTableStyle(string name)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| name | String | Il nome dello stile della tabella. |

### Valore di ritorno

L'indice dello stile di tabella.

### Esempi

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

            // Crea dati di esempio
            for (int i = 0; i < 5; i++)
            {
                worksheet.Cells[0, i].PutValue("Header " + (i + 1));
                for (int row = 1; row < 6; row++)
                {
                    worksheet.Cells[row, i].PutValue(row * (i + 1));
                }
            }

            // Crea uno stile di tabella personalizzato
            string styleName = "MyCustomStyle";
            TableStyleCollection tableStyles = workbook.Worksheets.TableStyles;
            int styleIndex = tableStyles.AddTableStyle(styleName);
            TableStyle tableStyle = tableStyles[styleIndex];

            // Stilizza la riga di intestazione
            Style headerStyle = workbook.CreateStyle();
            headerStyle.Font.IsBold = true;
            headerStyle.ForegroundColor = System.Drawing.Color.LightBlue;
            headerStyle.Pattern = BackgroundType.Solid;

            tableStyle.TableStyleElements.Add(TableStyleElementType.HeaderRow);
            TableStyleElement headerElement = tableStyle.TableStyleElements[TableStyleElementType.HeaderRow];
            headerElement.SetElementStyle(headerStyle);

            // Stilizza la prima colonna
            Style firstColStyle = workbook.CreateStyle();
            firstColStyle.Font.Color = System.Drawing.Color.Red;

            tableStyle.TableStyleElements.Add(TableStyleElementType.FirstColumn);
            TableStyleElement firstColElement = tableStyle.TableStyleElements[TableStyleElementType.FirstColumn];
            firstColElement.SetElementStyle(firstColStyle);

            // Crea una tabella con lo stile personalizzato
            int tableIndex = worksheet.ListObjects.Add(0, 0, 5, 4, true);
            ListObject table = worksheet.ListObjects[tableIndex];
            table.TableStyleName = styleName;
            table.ShowTableStyleFirstColumn = true;

            workbook.Save("CustomTableStyleDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [TableStyleCollection](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


