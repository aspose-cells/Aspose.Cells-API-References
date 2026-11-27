---
title: "TextBoxOptions.AllowTextToOverflow"
second_title: "Aspose.Cells för .NET API‑referens"
description: "TextBoxOptions-egenskap. Huruvida text får flöda över formen"
type: docs
url: /sv/net/aspose.cells.drawing.texts/textboxoptions/allowtexttooverflow/
---
## TextBoxOptions.AllowTextToOverflow property

Om text får flöda över formen.

```csharp
public bool AllowTextToOverflow { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class TextBoxOptionsPropertyAllowTextToOverflowDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en textruta i kalkylbladet
            TextBox textBox = worksheet.Shapes.AddTextBox(0, 0, 100, 100, 200, 50);

            // Ange text som kan flöda över
            textBox.Text = "This is a long text that might overflow the text box boundaries if AllowTextToOverflow is false";

            // Aktivera textöverspill
            textBox.TextBoxOptions.AllowTextToOverflow = true;

            // Spara arbetsboken
            workbook.Save("TextBoxAllowTextToOverflowDemo.xlsx");
        }
    }
}
```

### Se även

* class [TextBoxOptions](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


