---
title: "Style.Font"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Style. Ottiene un oggetto Font"
type: docs
url: /it/net/aspose.cells/style/font/
---
## Style.Font property

Ottiene un oggetto `Font`.

```csharp
public Font Font { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class StylePropertyFontDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Accedi alla cella B4 e imposta il suo font in grassetto
            Cell b4 = cells["B4"];
            Style b4Style = b4.GetStyle();
            b4Style.Font.IsBold = true;
            b4.SetStyle(b4Style);

            // Accedi alla cella C4 e assicurati che il suo font non sia in grassetto
            Cell c4 = cells["C4"];
            Style c4Style = c4.GetStyle();
            c4Style.Font.IsBold = false;
            c4.SetStyle(c4Style);

            // Accedi alla cella D4 e imposta il suo font in grassetto con un colore diverso
            Cell d4 = cells["D4"];
            Style d4Style = d4.GetStyle();
            d4Style.Font.IsBold = true;
            d4Style.Font.Color = Color.Red;
            d4.SetStyle(d4Style);

            // Verifica le proprietà del font
            Console.WriteLine("B4 Font Bold: " + b4.GetStyle().Font.IsBold);
            Console.WriteLine("C4 Font Bold: " + c4.GetStyle().Font.IsBold);
            Console.WriteLine("D4 Font Bold: " + d4.GetStyle().Font.IsBold);
            Console.WriteLine("D4 Font Color: " + d4.GetStyle().Font.Color);

            // Salva la cartella di lavoro
            workbook.Save("FontPropertyDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Font](../../font/)
* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


