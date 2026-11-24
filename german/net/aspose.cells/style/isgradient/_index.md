---
title: "Style.IsGradient"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Style-Eigenschaft. Gibt an, ob die Zellenbeschattung ein Farbverlaufsmuster ist"
type: docs
url: /de/net/aspose.cells/style/isgradient/
---
## Style.IsGradient property

Gibt an, ob die Zellen Schattierung ein Farbverlaufsmuster ist.

```csharp
public bool IsGradient { get; set; }
```

### Beispiele

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class StylePropertyIsGradientDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Erstellen Sie einen Stil
            Style style = workbook.CreateStyle();
            
            // Verlaufshintergrund festlegen
            style.SetTwoColorGradient(Color.LightBlue, Color.DarkBlue, GradientStyleType.Horizontal, 1);
            
            // Wende den Stil auf eine Zelle an
            worksheet.Cells["A1"].SetStyle(style);
            
            // Prüfen, ob der Stil einen Verlauf hat
            bool isGradient = worksheet.Cells["A1"].GetStyle().IsGradient;
            
            // Gib das Ergebnis aus
            Console.WriteLine("Cell A1 style has gradient: " + isGradient);
            
            // Speichere die Arbeitsmappe
            workbook.Save("GradientStyleDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


