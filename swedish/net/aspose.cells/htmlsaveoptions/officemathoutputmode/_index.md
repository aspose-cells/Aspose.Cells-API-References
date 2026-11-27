---
title: "HtmlSaveOptions.OfficeMathOutputMode"
second_title: "Aspose.Cells för .NET API‑referens"
description: "HtmlSaveOptions egenskap. Anger hur OfficeMath-objekt exporteras till HTML. Standardvärdet är Image"
type: docs
url: /sv/net/aspose.cells/htmlsaveoptions/officemathoutputmode/
---
## HtmlSaveOptions.OfficeMathOutputMode property

Anger hur OfficeMath-objekt exporteras till HTML, standardvärdet är Image.

```csharp
public HtmlOfficeMathOutputType OfficeMathOutputMode { get; set; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class HtmlSaveOptionsPropertyOfficeMathOutputModeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            var cell = worksheet.Cells["A1"];
            
            // Lägg till en ekvationsform med den tillgängliga metoden
            TextBox equationTextBox = worksheet.Shapes.AddEquation(cell.Row, 0, cell.Column, 0, 100, 50);
            equationTextBox.Text = "1/2"; // Set equation text

            // Skapa HTML-sparalternativ
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();

            // Visa och ändra OfficeMathOutputMode
            Console.WriteLine("Initial OfficeMathOutputMode: " + saveOptions.OfficeMathOutputMode);
            workbook.Save("OfficeMathDefault.html", saveOptions);

            saveOptions.OfficeMathOutputMode = HtmlOfficeMathOutputType.MathML;
            Console.WriteLine("Modified OfficeMathOutputMode: " + saveOptions.OfficeMathOutputMode);
            workbook.Save("OfficeMathMathML.html", saveOptions);
        }
    }
}
```

### Se även

* enum [HtmlOfficeMathOutputType](../../htmlofficemathoutputtype/)
* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


