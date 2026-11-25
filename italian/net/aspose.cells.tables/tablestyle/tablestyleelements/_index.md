---
title: "TableStyle.TableStyleElements"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà TableStyle. Ottiene tutti gli elementi dello stile di tabella"
type: docs
url: /it/net/aspose.cells.tables/tablestyle/tablestyleelements/
---
## TableStyle.TableStyleElements property

Ottiene tutti gli elementi dello stile della tabella.

```csharp
public TableStyleElementCollection TableStyleElements { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class TableStylePropertyTableStyleElementsDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crea dati di esempio per la tabella
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("Alice");
            worksheet.Cells["B3"].PutValue(25);

            // Crea una tabella
            int index = worksheet.ListObjects.Add(0, 0, 2, 1, true);
            ListObject table = worksheet.ListObjects[index];
            table.ShowTableStyleFirstColumn = true;

            // Ottieni lo stile di tabella (usa lo stile esistente invece di crearne uno nuovo)
            TableStyle style = workbook.Worksheets.TableStyles[0];

            // Modifica gli elementi dello stile di tabella
            TableStyleElement wholeTableElement = style.TableStyleElements[TableStyleElementType.WholeTable];
            Style wholeTableStyle = wholeTableElement.GetElementStyle();
            wholeTableStyle.Borders[BorderType.TopBorder].LineStyle = CellBorderType.Thick;
            wholeTableStyle.Borders[BorderType.TopBorder].Color = System.Drawing.Color.Red;

            // Applica lo stile modificato alla tabella
            table.TableStyleName = style.Name;

            // Salva la cartella di lavoro
            workbook.Save("TableStyleElementsDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [TableStyleElementCollection](../../tablestyleelementcollection/)
* class [TableStyle](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


