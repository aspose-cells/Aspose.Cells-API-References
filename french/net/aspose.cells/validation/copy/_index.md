---
title: "Validation.Copy"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Validation. Copier la validation"
type: docs
url: /fr/net/aspose.cells/validation/copy/
---
## Validation.Copy method

Copier la validation.

```csharp
public void Copy(Validation source, CopyOptions copyOption)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| source | Validation | La validation source. |
| copyOption | CopyOptions | L'option de copie. |

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ValidationMethodCopyWithValidationCopyOptionsDemo
    {
        public static void Run()
        {
            // Créer un classeur source avec des données d'exemple et une validation
            Workbook sourceWorkbook = new Workbook();
            Worksheet sourceSheet = sourceWorkbook.Worksheets[0];
            
            // Ajouter une validation d'exemple à la feuille source
            Validation sourceValidation = sourceSheet.Validations[sourceSheet.Validations.Add()];
            sourceValidation.Type = ValidationType.WholeNumber;
            sourceValidation.Operator = OperatorType.Between;
            sourceValidation.Formula1 = "10";
            sourceValidation.Formula2 = "20";
            
            // Créer un CellArea avec StartRow, StartColumn, EndRow, EndColumn
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.StartColumn = 0;
            area.EndRow = 0;
            area.EndColumn = 0;
            sourceValidation.AddArea(area);

            // Créer un classeur de destination
            Workbook destWorkbook = new Workbook();
            Worksheet destSheet = destWorkbook.Worksheets[0];
            
            // Ajouter une validation à la feuille de destination (sera écrasée par la copie)
            Validation destValidation = destSheet.Validations[destSheet.Validations.Add()];
            destValidation.AddArea(area); // Reuse the same area definition

            // Démontrer la méthode Copy avec CopyOptions
            CopyOptions options = new CopyOptions();
            destValidation.Copy(sourceValidation, options);

            // Vérifier que la validation a été copiée correctement
            Console.WriteLine("Validation Type: " + destValidation.Type);
            Console.WriteLine("Validation Formula1: " + destValidation.Formula1);
            Console.WriteLine("Validation Formula2: " + destValidation.Formula2);
        }
    }
}
```

### Voir aussi

* class [CopyOptions](../../copyoptions/)
* class [Validation](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


