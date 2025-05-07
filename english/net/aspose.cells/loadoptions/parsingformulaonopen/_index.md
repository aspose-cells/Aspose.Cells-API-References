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
// Called: options.ParsingFormulaOnOpen = false;
[Test]
        public void Property_ParsingFormulaOnOpen()
        {
            LoadOptions options = new LoadOptions();
            options.ParsingFormulaOnOpen = false;
            options.KeepUnparsedData = false;
            options.CheckDataValid = false;
            options.CheckExcelRestriction = false;

            String[] files = {"JAVA45489-1.xlsx", "JAVA45489-1.xlsx", "JAVA45489-1.xlsx"};

            foreach (String fileName in files)
            {
                Workbook wb = new Workbook(Constants.sourcePath + fileName, options);
                wb.Save(Constants.destPath + fileName.Substring(0, fileName.IndexOf(".")) + "_JAVA45489.xls");
            }
        }
```

### See Also

* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


