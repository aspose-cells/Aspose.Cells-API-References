---
title: StyleFlag.HideFormula
second_title: Aspose.Cells for .NET API Reference
description: StyleFlag property. Hide formula setting will be applied
type: docs
url: /net/aspose.cells/styleflag/hideformula/
---
## StyleFlag.HideFormula property

Hide formula setting will be applied.

```csharp
public bool HideFormula { get; set; }
```

### Examples

```csharp
namespace AsposeCellsExamples.StyleFlagPropertyHideFormulaDemo
{
    using Aspose.Cells;
    using System;

    public class StyleFlagPropertyHideFormulaDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add a formula to cell A1
            worksheet.Cells["A1"].Formula = "=1+2";
            worksheet.Cells["A1"].Value = 3; // Display value

            // Create a style flag with HideFormula set to true
            StyleFlag styleFlag = new StyleFlag();
            styleFlag.HideFormula = true;

            // Create a style and set IsFormulaHidden to true
            Style style = workbook.CreateStyle();
            style.IsFormulaHidden = true;

            // Apply the style to cell A1 with the style flag
            worksheet.Cells["A1"].SetStyle(style, styleFlag);

            // Protect the worksheet to see the effect of HideFormula
            worksheet.Protection.AllowEditingObject = true;
            worksheet.Protection.AllowEditingContent = false;
            worksheet.Protection.Password = "password";

            // Save the workbook
            workbook.Save("PropertyHideFormulaDemo.xlsx");

            // Verify the formula is hidden
            Console.WriteLine("Formula in A1: " + worksheet.Cells["A1"].Formula);
            Console.WriteLine("Is formula hidden? " + style.IsFormulaHidden);
        }
    }
}
```

### See Also

* class [StyleFlag](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


