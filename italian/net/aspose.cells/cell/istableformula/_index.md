---
title: "Cell.IsTableFormula"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Cell. Indica se questa cella fa parte della formula della tabella"
type: docs
url: /it/net/aspose.cells/cell/istableformula/
---
## Cell.IsTableFormula property

Indica se questa cella fa parte di una formula di tabella.

```csharp
public bool IsTableFormula { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class CellPropertyIsTableFormulaDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Crea una tabella
            int index = worksheet.ListObjects.Add(0, 0, 5, 3, true);
            ListObject table = worksheet.ListObjects[index];
            
            // Aggiungi la formula tabella alla cella D2
            Cell cell = worksheet.Cells["D2"];
            cell.Formula = "=SUM(Table1[[#This Row],[Column1]:[Column3]])";
            
            // Verifica se la cella contiene una formula tabella
            Console.WriteLine("Is table formula: " + cell.IsTableFormula);
            
            // Salva la cartella di lavoro
            workbook.Save("output.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Vedi anche

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


