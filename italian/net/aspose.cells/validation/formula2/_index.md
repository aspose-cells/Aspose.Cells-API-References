---
title: "Validation.Formula2"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà di convalida. Rappresenta il valore o l'espressione associata alla convalida dei dati"
type: docs
url: /it/net/aspose.cells/validation/formula2/
---
## Validation.Formula2 property

Rappresenta il valore o l'espressione associati alla convalida dei dati.

```csharp
public string Formula2 { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ValidationPropertyFormula2Demo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet sheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio
            sheet.Cells["B3"].PutValue(100);
            sheet.Cells["B7"].PutValue(50);
            
            // Crea una convalida per la cella B7
            Validation validation = sheet.Cells["B7"].GetValidation();
            
            // Imposta il tipo di convalida e le formule
            validation.Type = ValidationType.WholeNumber;
            validation.Operator = OperatorType.Between;
            validation.Formula1 = "10";
            validation.Formula2 = "=B3";  // Demonstrating Formula2 usage
            
            // Applica la convalida
            CellArea area = new CellArea();
            area.StartRow = 6;
            area.StartColumn = 1;
            area.EndRow = 6;
            area.EndColumn = 1;
            validation.AddArea(area);
            
            // Salva la cartella di lavoro
            workbook.Save("ValidationFormula2Demo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Validation](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


