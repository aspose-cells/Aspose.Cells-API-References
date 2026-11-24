---
title: "Font.IsBold"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Font-Eigenschaft. Gibt einen Wert zurück oder legt ihn fest, der angibt, ob die Schrift fett ist"
type: docs
url: /de/net/aspose.cells/font/isbold/
---
## Font.IsBold property

Ruft einen Wert ab oder legt ihn fest, der angibt, ob die Schrift fett ist.

```csharp
public bool IsBold { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FontPropertyIsBoldDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Zugriff auf das erste Arbeitsblatt
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Greife auf Zelle A1 zu und setze ihren Wert
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Bold Text Demo");
            
            // Rufen Sie den Zellenstil ab und setzen Sie die Schrift auf fett
            Style style = cell.GetStyle();
            style.Font.IsBold = true;
            cell.SetStyle(style);
            
            // Speichere die Arbeitsmappe
            workbook.Save("FontIsBoldDemo.xlsx");
            
            // Überprüfen Sie die Fett-Eigenschaft
            Workbook loadedWorkbook = new Workbook("FontIsBoldDemo.xlsx");
            Style loadedStyle = loadedWorkbook.Worksheets[0].Cells["A1"].GetStyle();
            Console.WriteLine("IsBold property: " + loadedStyle.Font.IsBold);
        }
    }
}
```

### Siehe auch

* class [Font](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


