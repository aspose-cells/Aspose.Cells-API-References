---
title: "HtmlSaveOptions.OfficeMathOutputMode"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété HtmlSaveOptions. Indique comment les objets OfficeMath sont exportés vers HTML. La valeur par défaut est Image"
type: docs
url: /fr/net/aspose.cells/htmlsaveoptions/officemathoutputmode/
---
## HtmlSaveOptions.OfficeMathOutputMode property

Indique comment les objets OfficeMath sont exportés en HTML, la valeur par défaut est Image.

```csharp
public HtmlOfficeMathOutputType OfficeMathOutputMode { get; set; }
```

### Exemples

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
            
            // Ajoutez une forme d'équation en utilisant la méthode disponible
            TextBox equationTextBox = worksheet.Shapes.AddEquation(cell.Row, 0, cell.Column, 0, 100, 50);
            equationTextBox.Text = "1/2"; // Set equation text

            // Créer des options d'enregistrement HTML
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();

            // Affichez et modifiez OfficeMathOutputMode
            Console.WriteLine("Initial OfficeMathOutputMode: " + saveOptions.OfficeMathOutputMode);
            workbook.Save("OfficeMathDefault.html", saveOptions);

            saveOptions.OfficeMathOutputMode = HtmlOfficeMathOutputType.MathML;
            Console.WriteLine("Modified OfficeMathOutputMode: " + saveOptions.OfficeMathOutputMode);
            workbook.Save("OfficeMathMathML.html", saveOptions);
        }
    }
}
```

### Voir aussi

* enum [HtmlOfficeMathOutputType](../../htmlofficemathoutputtype/)
* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


