---
title: "FormulaSettings.PreservePaddingSpaces"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "FormulaSettings-Eigenschaft. Gibt an, ob die zwischen Formeltoken eingefügten Leerzeichen und Zeilenumbrüche beim Abrufen und Setzen von Formeln erhalten bleiben sollen. Der Standardwert ist false."
type: docs
url: /de/net/aspose.cells/formulasettings/preservepaddingspaces/
---
## FormulaSettings.PreservePaddingSpaces property

Gibt an, ob Leerzeichen und Zeilenumbrüche, die zwischen Formeltoken eingefügt werden, beim Abrufen und Setzen von Formeln erhalten bleiben sollen. Der Standardwert ist false.

```csharp
public bool PreservePaddingSpaces { get; set; }
```

### Hinweise

Im Allgemeinen dienen diese Leerzeichen und Zeilenumbrüche nur der visuellen Darstellung; das Beibehalten oder Entfernen beeinflusst das berechnete Ergebnis nicht. Aus Leistungsgründen ist es, sofern keine besonderen Anforderungen bestehen, besser, sie bei der Verarbeitung von Formeln nicht zu erhalten.

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FormulaSettingsPropertyPreservePaddingSpacesDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Zugriff auf das erste Arbeitsblatt
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Formel mit eingefügten Leerzeichen setzen.
            string formulaWithSpaces = "=SUM( IF( A1:A5 > 10, B1:B5, 0 ) )";
            worksheet.Cells["C1"].Formula = formulaWithSpaces;
            
            // Standardverhalten (PreservePaddingSpaces ist true).
            Console.WriteLine("Formula with spaces preserved: " + worksheet.Cells["C1"].Formula);
            
            // Einstellung ändern, um eingefügte Leerzeichen zu entfernen.
            workbook.Settings.FormulaSettings.PreservePaddingSpaces = false;
            worksheet.Cells["C2"].Formula = formulaWithSpaces;
            
            Console.WriteLine("Formula with spaces removed: " + worksheet.Cells["C2"].Formula);
            
            // Speichere die Arbeitsmappe
            workbook.Save("FormulaSpacesDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [FormulaSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


