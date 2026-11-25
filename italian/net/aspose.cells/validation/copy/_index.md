---
title: "Validation.Copy"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Validation. Copia la convalida"
type: docs
url: /it/net/aspose.cells/validation/copy/
---
## Validation.Copy method

Copia la convalida.

```csharp
public void Copy(Validation source, CopyOptions copyOption)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| origine | Validation | La validation di origine. |
| copyOption | CopyOptions | L'opzione di copia. |

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ValidationMethodCopyWithValidationCopyOptionsDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro di origine con dati di esempio e convalida
            Workbook sourceWorkbook = new Workbook();
            Worksheet sourceSheet = sourceWorkbook.Worksheets[0];
            
            // Aggiungi una convalida di esempio al foglio di origine
            Validation sourceValidation = sourceSheet.Validations[sourceSheet.Validations.Add()];
            sourceValidation.Type = ValidationType.WholeNumber;
            sourceValidation.Operator = OperatorType.Between;
            sourceValidation.Formula1 = "10";
            sourceValidation.Formula2 = "20";
            
            // Crea CellArea con StartRow, StartColumn, EndRow, EndColumn
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.StartColumn = 0;
            area.EndRow = 0;
            area.EndColumn = 0;
            sourceValidation.AddArea(area);

            // Crea una cartella di lavoro di destinazione
            Workbook destWorkbook = new Workbook();
            Worksheet destSheet = destWorkbook.Worksheets[0];
            
            // Aggiungi una convalida al foglio di destinazione (verrà sovrascritta dalla copia)
            Validation destValidation = destSheet.Validations[destSheet.Validations.Add()];
            destValidation.AddArea(area); // Reuse the same area definition

            // Dimostra il metodo Copy con CopyOptions
            CopyOptions options = new CopyOptions();
            destValidation.Copy(sourceValidation, options);

            // Verifica che la convalida sia stata copiata correttamente
            Console.WriteLine("Validation Type: " + destValidation.Type);
            Console.WriteLine("Validation Formula1: " + destValidation.Formula1);
            Console.WriteLine("Validation Formula2: " + destValidation.Formula2);
        }
    }
}
```

### Vedi anche

* class [CopyOptions](../../copyoptions/)
* class [Validation](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


