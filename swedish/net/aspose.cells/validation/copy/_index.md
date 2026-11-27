---
title: "Validation.Copy"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Valideringsmetod. Kopiera validering"
type: docs
url: /sv/net/aspose.cells/validation/copy/
---
## Validation.Copy method

Kopiera validering.

```csharp
public void Copy(Validation source, CopyOptions copyOption)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| källa | Validering | Källvalideringen. |
| copyOption | CopyOptions | Kopieringsalternativet. |

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ValidationMethodCopyWithValidationCopyOptionsDemo
    {
        public static void Run()
        {
            // Skapa en källarbok med exempeldata och validering
            Workbook sourceWorkbook = new Workbook();
            Worksheet sourceSheet = sourceWorkbook.Worksheets[0];
            
            // Lägg till exempelvalidering i källbladet
            Validation sourceValidation = sourceSheet.Validations[sourceSheet.Validations.Add()];
            sourceValidation.Type = ValidationType.WholeNumber;
            sourceValidation.Operator = OperatorType.Between;
            sourceValidation.Formula1 = "10";
            sourceValidation.Formula2 = "20";
            
            // Skapa CellArea med StartRow, StartColumn, EndRow, EndColumn
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.StartColumn = 0;
            area.EndRow = 0;
            area.EndColumn = 0;
            sourceValidation.AddArea(area);

            // Skapa en målarbetsbok
            Workbook destWorkbook = new Workbook();
            Worksheet destSheet = destWorkbook.Worksheets[0];
            
            // Lägg till en validering i destinationsbladet (kommer att skrivas över av kopiering)
            Validation destValidation = destSheet.Validations[destSheet.Validations.Add()];
            destValidation.AddArea(area); // Reuse the same area definition

            // Demonstrera Copy-metoden med CopyOptions
            CopyOptions options = new CopyOptions();
            destValidation.Copy(sourceValidation, options);

            // Verifiera att valideringen kopierades korrekt
            Console.WriteLine("Validation Type: " + destValidation.Type);
            Console.WriteLine("Validation Formula1: " + destValidation.Formula1);
            Console.WriteLine("Validation Formula2: " + destValidation.Formula2);
        }
    }
}
```

### Se även

* class [CopyOptions](../../copyoptions/)
* class [Validation](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


