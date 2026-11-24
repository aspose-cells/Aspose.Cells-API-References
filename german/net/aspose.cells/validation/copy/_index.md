---
title: "Validation.Copy"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Validation-Methode. Kopiert die Validierung"
type: docs
url: /de/net/aspose.cells/validation/copy/
---
## Validation.Copy method

Validierung kopieren.

```csharp
public void Copy(Validation source, CopyOptions copyOption)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| source | Validierung | Die Quellvalidierung. |
| copyOption | CopyOptions | Die Kopieroption. |

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ValidationMethodCopyWithValidationCopyOptionsDemo
    {
        public static void Run()
        {
            // Erstellen Sie eine Quellarbeitsmappe mit Beispieldaten und Validierung
            Workbook sourceWorkbook = new Workbook();
            Worksheet sourceSheet = sourceWorkbook.Worksheets[0];
            
            // Fügen Sie eine Beispielvalidierung zum Quellblatt hinzu
            Validation sourceValidation = sourceSheet.Validations[sourceSheet.Validations.Add()];
            sourceValidation.Type = ValidationType.WholeNumber;
            sourceValidation.Operator = OperatorType.Between;
            sourceValidation.Formula1 = "10";
            sourceValidation.Formula2 = "20";
            
            // Erstelle CellArea mit StartRow, StartColumn, EndRow, EndColumn
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.StartColumn = 0;
            area.EndRow = 0;
            area.EndColumn = 0;
            sourceValidation.AddArea(area);

            // Erstelle eine Ziel-Arbeitsmappe.
            Workbook destWorkbook = new Workbook();
            Worksheet destSheet = destWorkbook.Worksheets[0];
            
            // Füge eine Validierung zum Zielblatt hinzu (wird durch Kopieren überschrieben)
            Validation destValidation = destSheet.Validations[destSheet.Validations.Add()];
            destValidation.AddArea(area); // Reuse the same area definition

            // Demonstriere die Copy-Methode mit CopyOptions
            CopyOptions options = new CopyOptions();
            destValidation.Copy(sourceValidation, options);

            // Überprüfe, ob die Validierung korrekt kopiert wurde
            Console.WriteLine("Validation Type: " + destValidation.Type);
            Console.WriteLine("Validation Formula1: " + destValidation.Formula1);
            Console.WriteLine("Validation Formula2: " + destValidation.Formula2);
        }
    }
}
```

### Siehe auch

* class [CopyOptions](../../copyoptions/)
* class [Validation](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


