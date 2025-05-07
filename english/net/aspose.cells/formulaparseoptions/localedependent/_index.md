---
title: FormulaParseOptions.LocaleDependent
second_title: Aspose.Cells for .NET API Reference
description: FormulaParseOptions property. Whether the formula is locale formatted. Default is false
type: docs
url: /net/aspose.cells/formulaparseoptions/localedependent/
---
## FormulaParseOptions.LocaleDependent property

Whether the formula is locale formatted. Default is false.

```csharp
public bool LocaleDependent { get; set; }
```

### Examples

```csharp
// Called: LocaleDependent = true,
public static void Property_LocaleDependent()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Create an instance of FormulaParseOptions
            FormulaParseOptions options = new FormulaParseOptions
            {
                LocaleDependent = true,
                R1C1Style = false,
                CheckAddIn = true,
                Parse = true,
                CustomFunctionDefinition = null // Assuming no custom function definition for this example
            };

            // Add a formula to a cell using the options
            Cell cell = worksheet.Cells["A1"];
            cell.SetFormula("=SUM(B1:B10)", options);

            // Save the workbook
            workbook.Save("FormulaParseOptionsExample.xlsx");
            workbook.Save("FormulaParseOptionsExample.pdf");
            return;
        }
```

### See Also

* class [FormulaParseOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


