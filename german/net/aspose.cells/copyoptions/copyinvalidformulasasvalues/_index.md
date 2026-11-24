---
title: "CopyOptions.CopyInvalidFormulasAsValues"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "CopyOptions-Eigenschaft. Wenn die Formel für das Ziel nicht gültig ist, werden nur Werte kopiert."
type: docs
url: /de/net/aspose.cells/copyoptions/copyinvalidformulasasvalues/
---
## CopyOptions.CopyInvalidFormulasAsValues property

Wenn die Formel für das Ziel nicht gültig ist, werden nur Werte kopiert.

```csharp
public bool CopyInvalidFormulasAsValues { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CopyOptionsPropertyCopyInvalidFormulasAsValuesDemo
    {
        public static void Run()
        {
            // Erstelle eine Quell-Arbeitsmappe mit einem Beispiel-Arbeitsblatt.
            Workbook srcWorkbook = new Workbook();
            Worksheet srcSheet = srcWorkbook.Worksheets[0];
            
            // Füge eine Formel hinzu, die in manchen Kontexten ungültig sein könnte.
            srcSheet.Cells["A1"].Formula = "=1/0"; // Division by zero - invalid formula
            srcSheet.Cells["A2"].Value = "Valid Data";

            // Erstelle eine Ziel-Arbeitsmappe.
            Workbook destWorkbook = new Workbook();
            
            // Setze Kopieroptionen, um ungültige Formeln in Werte zu konvertieren.
            CopyOptions copyOptions = new CopyOptions();
            copyOptions.CopyInvalidFormulasAsValues = true;

            // Kopiere das Arbeitsblatt mit den Optionen.
            destWorkbook.Worksheets[0].Copy(srcSheet, copyOptions);

            // Ergebnisse überprüfen.
            Console.WriteLine("A1 (invalid formula copied as value): " + 
                destWorkbook.Worksheets[0].Cells["A1"].Value); // Should show #DIV/0! as value
            Console.WriteLine("A2 (valid data): " + 
                destWorkbook.Worksheets[0].Cells["A2"].Value); // Should show "Valid Data"
        }
    }
}
```

### Siehe auch

* class [CopyOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


