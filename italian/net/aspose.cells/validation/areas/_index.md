---
title: "Validation.Areas"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà di convalida. Ottiene tutti i CellArea che contengono le impostazioni di convalida dei dati"
type: docs
url: /it/net/aspose.cells/validation/areas/
---
## Validation.Areas property

Ottiene tutti i [`CellArea`](../../cellarea/) che contengono le impostazioni di convalida dei dati.

```csharp
public CellArea[] Areas { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ValidationPropertyAreasDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets.Add("Areas & rent");

            // Crea una convalida per la colonna A
            Validation validation = worksheet.Validations[worksheet.Validations.Add()];
            validation.Type = ValidationType.WholeNumber;
            validation.Operator = OperatorType.Between;
            validation.Formula1 = "1";
            validation.Formula2 = "100";

            // Aggiungi aree di convalida in righe diverse
            validation.AddArea(new CellArea { StartRow = 46, StartColumn = 0, EndRow = 50, EndColumn = 0 });
            validation.AddArea(new CellArea { StartRow = 92, StartColumn = 0, EndRow = 96, EndColumn = 0 });
            validation.AddArea(new CellArea { StartRow = 138, StartColumn = 0, EndRow = 142, EndColumn = 0 });

            // Dimostra l'accesso alle aree di convalida
            CellArea area1 = (CellArea)validation.Areas[0];
            Console.WriteLine($"Area 1 StartRow: {area1.StartRow}"); // Output: 46
            
            CellArea area2 = (CellArea)validation.Areas[1];
            Console.WriteLine($"Area 2 StartRow: {area2.StartRow}"); // Output: 92
            
            CellArea area3 = (CellArea)validation.Areas[2];
            Console.WriteLine($"Area 3 StartRow: {area3.StartRow}"); // Output: 138
        }
    }
}
```

### Vedi anche

* struct [CellArea](../../cellarea/)
* class [Validation](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


