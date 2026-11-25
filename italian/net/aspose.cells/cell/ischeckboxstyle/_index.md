---
title: "Cell.IsCheckBoxStyle"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Cell. Indica se questa cella è impostata come casella di controllo"
type: docs
url: /it/net/aspose.cells/cell/ischeckboxstyle/
---
## Cell.IsCheckBoxStyle property

Indica se impostare questa cella come casella di controllo.

```csharp
public bool IsCheckBoxStyle { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellPropertyIsCheckBoxStyleDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Accedi alla cella B1 e impostala in stile casella di controllo
            Cell cell = worksheet.Cells["B1"];
            cell.IsCheckBoxStyle = true;
            cell.PutValue(true);
            
            // Accedi alla cella A1 e impostala in stile casella di controllo con un valore
            cell = worksheet.Cells["A1"];
            cell.IsCheckBoxStyle = true;
            cell.PutValue(false);
            
            // Salva la cartella di lavoro
            workbook.Save("CheckBoxStyleDemo.xlsx");
            
            // Carica la cartella di lavoro salvata per verificare le proprietà
            Workbook loadedWorkbook = new Workbook("CheckBoxStyleDemo.xlsx");
            worksheet = loadedWorkbook.Worksheets[0];
            
            // Verifica che B1 sia in stile casella di controllo
            cell = worksheet.Cells["B1"];
            Console.WriteLine("Cell B1 IsCheckBoxStyle: " + cell.IsCheckBoxStyle);
            
            // Cambia B1 a stile non casella di controllo e salva
            cell.IsCheckBoxStyle = false;
            loadedWorkbook.Save("CheckBoxStyleDemo_Modified.xlsx");
        }
    }
}
```

### Vedi anche

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


