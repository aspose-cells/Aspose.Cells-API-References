---
title: "HtmlSaveOptions.OfficeMathOutputMode"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad HtmlSaveOptions. Indica cómo se exportan los objetos OfficeMath a HTML. El valor predeterminado es Image"
type: docs
url: /es/net/aspose.cells/htmlsaveoptions/officemathoutputmode/
---
## HtmlSaveOptions.OfficeMathOutputMode property

Indica cómo se exportan los objetos OfficeMath a HTML, el valor predeterminado es Image.

```csharp
public HtmlOfficeMathOutputType OfficeMathOutputMode { get; set; }
```

### Ejemplos

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
            
            // Agregar una forma de ecuación usando el método disponible
            TextBox equationTextBox = worksheet.Shapes.AddEquation(cell.Row, 0, cell.Column, 0, 100, 50);
            equationTextBox.Text = "1/2"; // Set equation text

            // Crear opciones de guardado HTML
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();

            // Mostrar y modificar OfficeMathOutputMode
            Console.WriteLine("Initial OfficeMathOutputMode: " + saveOptions.OfficeMathOutputMode);
            workbook.Save("OfficeMathDefault.html", saveOptions);

            saveOptions.OfficeMathOutputMode = HtmlOfficeMathOutputType.MathML;
            Console.WriteLine("Modified OfficeMathOutputMode: " + saveOptions.OfficeMathOutputMode);
            workbook.Save("OfficeMathMathML.html", saveOptions);
        }
    }
}
```

### Ver también

* enum [HtmlOfficeMathOutputType](../../htmlofficemathoutputtype/)
* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


