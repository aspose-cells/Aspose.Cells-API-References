---
title: "Worksheet.Validations"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Worksheet. Ottiene la raccolta delle impostazioni di convalida dei dati nel foglio di lavoro"
type: docs
url: /it/net/aspose.cells/worksheet/validations/
---
## Worksheet.Validations property

Ottiene la collezione delle impostazioni di convalida dei dati nel foglio di lavoro.

```csharp
public ValidationCollection Validations { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyValidationsDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi la convalida dei dati alla cella A1
            Validation validation = worksheet.Validations[worksheet.Validations.Add()];
            validation.Type = ValidationType.List;
            validation.Formula1 = "Option1,Option2,Option3";
            
            // Correzione: crea CellArea con StartRow, StartColumn, EndRow, EndColumn
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.StartColumn = 0;
            area.EndRow = 0;
            area.EndColumn = 0;
            validation.AddArea(area);

            // Ottieni la convalida dalla cella A1
            Validation cellValidation = worksheet.Validations.GetValidationInCell(0, 0);
            
            // Restituisci il tipo di convalida
            Console.WriteLine("Validation type in A1: " + cellValidation.Type);
            
            // Salva la cartella di lavoro
            workbook.Save("ValidationDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [ValidationCollection](../../validationcollection/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


