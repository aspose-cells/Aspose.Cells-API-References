---
title: LoadOptions.CheckDataValid
second_title: Aspose.Cells for .NET API Reference
description: LoadOptions property. Check whether data is valid in the template file
type: docs
url: /net/aspose.cells/loadoptions/checkdatavalid/
---
## LoadOptions.CheckDataValid property

Check whether data is valid in the template file.

```csharp
public bool CheckDataValid { get; set; }
```

### Examples

```csharp
// Called: options.CheckDataValid = false;
public void LoadOptions_Property_CheckDataValid()
{
    LoadOptions options = new LoadOptions();
    options.ParsingFormulaOnOpen = false;
    options.KeepUnparsedData = false;
    options.CheckDataValid = false;
    options.CheckExcelRestriction = false;

    String[] files = {"example.xlsx", "example.xlsx", "example.xlsx"};

    foreach (String fileName in files)
    {
        Workbook wb = new Workbook(Constants.sourcePath + fileName, options);
        wb.Save(Constants.destPath + fileName.Substring(0, fileName.IndexOf(".")) + "example.xls");
    }
}
```

### See Also

* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


