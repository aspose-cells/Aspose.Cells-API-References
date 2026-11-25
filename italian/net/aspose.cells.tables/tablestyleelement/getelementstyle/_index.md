---
title: "TableStyleElement.GetElementStyle"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo TableStyleElement. Ottiene lo stile dell'elemento"
type: docs
url: /it/net/aspose.cells.tables/tablestyleelement/getelementstyle/
---
## TableStyleElement.GetElementStyle method

Ottiene lo stile dell'elemento.

```csharp
public Style GetElementStyle()
```

### Valore di ritorno

Restituisce l'oggetto [`Style`](../../../aspose.cells/style/).

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class TableStyleElementMethodGetElementStyleDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio
            worksheet.Cells["A1"].PutValue("Item");
            worksheet.Cells["B1"].PutValue("Price");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["B2"].PutValue(2.5);
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["B3"].PutValue(1.8);
            
            // Crea una tabella
            int index = worksheet.ListObjects.Add(0, 0, 2, 1, true);
            ListObject table = worksheet.ListObjects[index];
            
            // Ottieni lo stile della tabella dalla collezione di stili della cartella di lavoro
            TableStyleCollection tableStyles = workbook.Worksheets.TableStyles;
            TableStyle style = tableStyles[0];
            table.TableStyleName = style.Name;
            
            // Accedi all'intero elemento di stile della tabella
            TableStyleElement element = style.TableStyleElements[TableStyleElementType.WholeTable];
            
            // Ottieni lo stile dell'elemento
            Style tableStyle = element.GetElementStyle();
            
            // Modifica le proprietà dello stile
            tableStyle.Font.Name = "Arial";
            tableStyle.Font.Size = 12;
            tableStyle.Font.IsBold = true;
            tableStyle.Borders[BorderType.LeftBorder].LineStyle = CellBorderType.Thin;
            tableStyle.Borders[BorderType.RightBorder].LineStyle = CellBorderType.Thin;
            tableStyle.Borders[BorderType.TopBorder].LineStyle = CellBorderType.Thin;
            tableStyle.Borders[BorderType.BottomBorder].LineStyle = CellBorderType.Thin;
            
            // Reimposta lo stile modificato
            element.SetElementStyle(tableStyle);
            
            // Salva la cartella di lavoro
            workbook.Save("TableStyleElementDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Style](../../../aspose.cells/style/)
* class [TableStyleElement](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


