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
// Called: loadOptions.ParsingFormulaOnOpen = (false);
public void LoadOptions_Property_ParsingFormulaOnOpen()
{
            
    LoadOptions loadOptions = new LoadOptions();
    loadOptions.KeepUnparsedData = (false);
    loadOptions.ParsingFormulaOnOpen = (false);
    LoadFilter loadFilter = new LoadFilter(LoadDataFilterOptions.VBA);
    loadOptions.LoadFilter = (loadFilter);


    Workbook workbook = new Workbook(Constants.sourcePath + "example.xlsm", loadOptions);
    VbaModuleCollection modules = workbook.VbaProject.Modules;
    Assert.AreEqual(6,modules.Count);
}
```

### See Also

* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


