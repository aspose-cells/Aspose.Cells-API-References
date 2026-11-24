---
title: "StyleFlag.HideFormula"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "StyleFlag-Eigenschaft. Hide-Formel-Einstellung wird angewendet"
type: docs
url: /de/net/aspose.cells/styleflag/hideformula/
---
## StyleFlag.HideFormula property

Die Einstellung zum Ausblenden von Formeln wird angewendet.

```csharp
public bool HideFormula { get; set; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class StyleFlagPropertyHideFormulaDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cell a1 = worksheet.Cells["A1"];
            // Fügen Sie eine Formel zu Zelle A1 hinzu
            a1.Formula = "=1+2";
            a1.Value = 3; // Display value

            // Erstellen Sie ein Style-Flag mit HideFormula auf true gesetzt
            StyleFlag styleFlag = new StyleFlag();
            styleFlag.HideFormula = true;

            // Erstellen Sie einen Stil und setzen Sie IsFormulaHidden auf true
            Style style = workbook.CreateStyle();
            style.IsFormulaHidden = true;

            // Wenden Sie den Stil auf Zelle A1 mit dem Style-Flag an
            a1.SetStyle(style, styleFlag);

            // Schützen Sie das Arbeitsblatt, um die Wirkung von HideFormula zu sehen
            worksheet.Protection.AllowEditingObject = true;
            worksheet.Protection.AllowEditingContent = false;
            worksheet.Protection.Password = "password";

            // Speichere die Arbeitsmappe
            workbook.Save("PropertyHideFormulaDemo.xlsx");

            // Überprüfen Sie, ob die Formel verborgen ist
            Console.WriteLine("Formula in A1: " + a1.Formula);
            Console.WriteLine("Is formula hidden? " + a1.GetStyle().IsFormulaHidden);
        }
    }
}
```

### Siehe auch

* class [StyleFlag](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


