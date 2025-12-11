---
title: HtmlSaveOptions.OfficeMathOutputMode
second_title: Aspose.Cells for .NET API Reference
description: HtmlSaveOptions property. Indicates how OfficeMath objects are exported to HTML Default value is Image
type: docs
url: /net/aspose.cells/htmlsaveoptions/officemathoutputmode/
---
## HtmlSaveOptions.OfficeMathOutputMode property

Indicates how OfficeMath objects are exported to HTML, Default value is Image.

```csharp
public HtmlOfficeMathOutputType OfficeMathOutputMode { get; set; }
```

### Examples

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
            
            // Add an equation shape using the available method
            TextBox equationTextBox = worksheet.Shapes.AddEquation(cell.Row, 0, cell.Column, 0, 100, 50);
            equationTextBox.Text = "1/2"; // Set equation text

            // Create HTML save options
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();

            // Display and modify OfficeMathOutputMode
            Console.WriteLine("Initial OfficeMathOutputMode: " + saveOptions.OfficeMathOutputMode);
            workbook.Save("OfficeMathDefault.html", saveOptions);

            saveOptions.OfficeMathOutputMode = HtmlOfficeMathOutputType.MathML;
            Console.WriteLine("Modified OfficeMathOutputMode: " + saveOptions.OfficeMathOutputMode);
            workbook.Save("OfficeMathMathML.html", saveOptions);
        }
    }
}
```

### See Also

* enum [HtmlOfficeMathOutputType](../../htmlofficemathoutputtype/)
* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


