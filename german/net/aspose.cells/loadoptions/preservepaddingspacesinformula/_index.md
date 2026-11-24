---
title: "LoadOptions.PreservePaddingSpacesInFormula"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "LoadOptions-Eigenschaft. Gibt an, ob die zwischen Formeltoken eingefügten Leerzeichen und Zeilenumbrüche beim Abrufen und Setzen von Formeln beibehalten werden sollen. Der Standardwert ist false."
type: docs
url: /de/net/aspose.cells/loadoptions/preservepaddingspacesinformula/
---
## LoadOptions.PreservePaddingSpacesInFormula property

Gibt an, ob Leerzeichen und Zeilenumbrüche, die zwischen Formeltoken eingefügt sind, beim Lesen und Schreiben von Formeln erhalten bleiben sollen. Der Standardwert ist false.

```csharp
public bool PreservePaddingSpacesInFormula { get; set; }
```

### Hinweise

Nach dem Laden der Arbeitsmappe aus einer Vorlagendatei mit dieser Option wird [`PreservePaddingSpaces`](../../formulasettings/preservepaddingspaces/) auf denselben Wert wie diese Eigenschaft gesetzt.

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class LoadOptionsPropertyPreservePaddingSpacesInFormulaDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Aktiviere das Beibehalten von Auffüll-Leerzeichen in Formeln
            workbook.Settings.FormulaSettings.PreservePaddingSpaces = true;
            
            // Greife auf das erste Arbeitsblatt zu und setze eine Formel mit Auffüll-Leerzeichen
            Worksheet worksheet = workbook.Worksheets[0];
            Cell cell = worksheet.Cells["A1"];
            string formulaWithSpaces = "= IF(1 <>2, 2, 1)";
            cell.Formula = formulaWithSpaces;
            
            // Speichere die Arbeitsmappe und lade sie erneut mit der Option PreservePaddingSpacesInFormula
            string outputPath = "output.xlsx";
            workbook.Save(outputPath, SaveFormat.Xlsx);
            
            LoadOptions loadOptions = new LoadOptions(LoadFormat.Xlsx)
            {
                PreservePaddingSpacesInFormula = true
            };
            
            Workbook reloadedWorkbook = new Workbook(outputPath, loadOptions);
            Worksheet reloadedWorksheet = reloadedWorkbook.Worksheets[0];
            
            // Überprüfe, dass die Formel nach dem erneuten Laden die Leerzeichen beibehalten hat
            Console.WriteLine("Original formula: " + formulaWithSpaces);
            Console.WriteLine("Reloaded formula: " + reloadedWorksheet.Cells["A1"].Formula);
        }
    }
}
```

### Siehe auch

* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


