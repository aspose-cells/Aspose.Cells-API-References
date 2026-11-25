---
title: "ListColumn.Formula"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ListColumn. Ottiene e imposta la formula della colonna dell'elenco"
type: docs
url: /it/net/aspose.cells.tables/listcolumn/formula/
---
## ListColumn.Formula property

Ottiene e imposta la formula della colonna dell'elenco.

```csharp
public string Formula { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class ListColumnPropertyFormulaDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Crea dati di esempio e tabella
            sheet.Cells["A1"].PutValue("Numbers");
            sheet.Cells["A2"].PutValue(5);
            sheet.Cells["A3"].PutValue(10);
            sheet.Cells["A4"].PutValue(15);
            
            sheet.Cells["B1"].PutValue("Doubled");
            sheet.Cells["B2"].PutValue("=A2*2");
            
            int tableIndex = sheet.ListObjects.Add(0, 0, 3, 1, true);
            ListObject table = sheet.ListObjects[tableIndex];
            table.ShowTotals = true;
            
            // Aggiungi la formula alla colonna dell'elenco
            ListColumn column = table.ListColumns[0];
            column.Formula = "=A2*3"; // This will apply to all cells in the column
            
            // Salva la cartella di lavoro
            workbook.Save("ListColumnFormulaDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [ListColumn](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


