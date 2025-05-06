---
title: LoadOptions.ParsingFormulaOnOpen
second_title: Aspose.Cells for .NET API Reference
description: LoadOptions property. Indicates whether parsing the formula when reading the file
type: docs
url: /net/aspose.cells/loadoptions/parsingformulaonopen/
---
## LoadOptions.ParsingFormulaOnOpen property

Indicates whether parsing the formula when reading the file.

```csharp
public bool ParsingFormulaOnOpen { get; set; }
```

### Remarks

Only applies for Excel Xlsx, Xltx, Xltm and Xlsm file because the formulas in the files are stored with a string formula.

### Examples

```csharp
// Called: options.ParsingFormulaOnOpen = (false);
[Test]
        public void Property_ParsingFormulaOnOpen()
        {
            LoadOptions options = new LoadOptions();
            options.ParsingFormulaOnOpen = (false);
            options.KeepUnparsedData = (false);
            options.CheckDataValid = (false);
            options.CheckExcelRestriction = (false);
            Workbook wb = new Workbook(Constants.sourcePath + &quot;CELLSJAVA-45489.xlsx&quot;, options);
            wb.Save(Constants.destPath + &quot;CellsJava45489.xls&quot;);
        }
```

### See Also

* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


