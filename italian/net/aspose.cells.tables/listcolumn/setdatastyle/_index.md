---
title: "ListColumn.SetDataStyle"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo ListColumn. Imposta lo stile dei dati in questa colonna della tabella"
type: docs
url: /it/net/aspose.cells.tables/listcolumn/setdatastyle/
---
## ListColumn.SetDataStyle method

Imposta lo stile dei dati in questa colonna della tabella.

```csharp
public void SetDataStyle(Style style)
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ListColumnMethodSetDataStyleWithStyleDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio
            worksheet.Cells["A1"].PutValue("Header");
            worksheet.Cells["A2"].PutValue("Data1");
            worksheet.Cells["A3"].PutValue("Data2");
            
            // Crea un oggetto lista (tabella)
            int index = worksheet.ListObjects.Add(0, 0, 2, 0, true);
            Aspose.Cells.Tables.ListObject table = worksheet.ListObjects[index];
            
            // Ottieni lo stile della prima colonna
            Style style = table.ListColumns[0].GetDataStyle();
            
            // Modifica lo stile
            style.Pattern = BackgroundType.Solid;
            style.BackgroundColor = System.Drawing.Color.Red;
            
            // Applica lo stile modificato alla colonna
            table.ListColumns[0].SetDataStyle(style);
            
            // Salva la cartella di lavoro
            workbook.Save("output.xlsx");
        }
    }
}
```

### Vedi anche

* class [Style](../../../aspose.cells/style/)
* class [ListColumn](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


