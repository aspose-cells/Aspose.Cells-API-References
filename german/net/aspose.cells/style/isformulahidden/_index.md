---
title: "Style.IsFormulaHidden"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Style-Eigenschaft. Gibt an, ob die Formel ausgeblendet wird, wenn das Arbeitsblatt geschützt ist."
type: docs
url: /de/net/aspose.cells/style/isformulahidden/
---
## Style.IsFormulaHidden property

Gibt an, ob die Formel verborgen wird, wenn das Arbeitsblatt geschützt ist.

```csharp
public bool IsFormulaHidden { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StylePropertyIsFormulaHiddenDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Erstelle einen Stil mit IsFormulaHidden auf true gesetzt
            Style style = workbook.CreateStyle();
            style.IsFormulaHidden = true;
            
            // Wende den Stil auf eine Zelle an
            cells["A1"].SetStyle(style);
            cells["A1"].Formula = "=1+1";

            // Erstelle einen weiteren Stil mit IsFormulaHidden auf false gesetzt
            Style style2 = workbook.CreateStyle();
            style2.IsFormulaHidden = false;
            
            // Wende den zweiten Stil auf eine andere Zelle an
            cells["B1"].SetStyle(style2);
            cells["B1"].Formula = "=2+2";

            // Schützen Sie das Arbeitsblatt, um die Wirkung zu sehen
            worksheet.Protect(ProtectionType.All, "password", null);

            // Speichere die Arbeitsmappe
            workbook.Save("IsFormulaHiddenDemo.xlsx");

            Console.WriteLine("Workbook saved with IsFormulaHidden examples.");
        }
    }
}
```

### Siehe auch

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


