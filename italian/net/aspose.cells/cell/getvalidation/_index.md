---
title: "Cell.GetValidation"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Cell. Restituisce la convalida applicata a questa cella"
type: docs
url: /it/net/aspose.cells/cell/getvalidation/
---
## Cell.GetValidation method

Ottiene la convalida applicata a questa cella.

```csharp
public Validation GetValidation()
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodGetValidationDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Accedi alla cella B5 e aggiungi la convalida
            Cell cell = worksheet.Cells["B5"];
            Validation validation = cell.GetValidation();
            
            // Imposta il tipo di convalida e mostra il messaggio
            validation.Type = ValidationType.WholeNumber;
            validation.Operator = OperatorType.Between;
            validation.Formula1 = "10";
            validation.Formula2 = "20";
            validation.ShowError = true;
            validation.ErrorMessage = "Enter value between 10 and 20";
            
            // Salva la cartella di lavoro
            workbook.Save("ValidationDemo.xlsx");
            
            // Verifica la convalida
            Validation retrievedValidation = cell.GetValidation();
            Console.WriteLine("Validation Type: " + retrievedValidation.Type);
            Console.WriteLine("Validation Message: " + retrievedValidation.ErrorMessage);
        }
    }
}
```

### Vedi anche

* class [Validation](../../validation/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


