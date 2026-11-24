---
title: "FormulaParseOptions.CheckAddIn"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "FormulaParseOptions-Eigenschaft. Gibt an, ob Add-Ins in bestehenden externen Links der aktuellen Arbeitsmappe für benutzerdefinierte Funktionen ohne externen Link geprüft werden. Standard ist true. Wenn die benutzerdefinierte Funktion mit einem Add-In in bestehenden externen Links übereinstimmt, wird sie als Add-In übernommen."
type: docs
url: /de/net/aspose.cells/formulaparseoptions/checkaddin/
---
## FormulaParseOptions.CheckAddIn property

Ob Add‑Ins in bestehenden externen Links der aktuellen Arbeitsmappe für benutzerdefinierte Funktionen ohne externen Link überprüft werden sollen. Standard ist true (wenn die benutzerdefinierte Funktion mit einem Add‑In in bestehenden externen Links übereinstimmt, wird sie als dieses Add‑In betrachtet).

```csharp
public bool CheckAddIn { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FormulaParseOptionsPropertyCheckAddInDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Cells cells = wb.Worksheets[0].Cells;
            
            // Add-In-Funktion registrieren
            wb.Worksheets.RegisterAddInFunction("Test.xlam", "TEST_UDF", false);

            // Ohne CheckAddIn=false – Formel wird in das Add-In-Format konvertiert
            cells["A1"].SetFormula("=TEST_UDF()", new FormulaParseOptions());
            Console.WriteLine("A1 Formula (CheckAddIn=true): " + cells["A1"].Formula);

            // Mit CheckAddIn=false – Formel bleibt unverändert
            cells["A2"].SetFormula("=TEST_UDF()", new FormulaParseOptions() { CheckAddIn = false });
            Console.WriteLine("A2 Formula (CheckAddIn=false): " + cells["A2"].Formula);
        }
    }
}
```

### Siehe auch

* class [FormulaParseOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


