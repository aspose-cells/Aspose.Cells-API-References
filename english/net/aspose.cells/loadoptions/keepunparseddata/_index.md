---
title: LoadOptions.KeepUnparsedData
second_title: Aspose.Cells for .NET API Reference
description: LoadOptions property. Whether keep the unparsed data in memory for the Workbook when it is loaded from template file. Default is true
type: docs
url: /net/aspose.cells/loadoptions/keepunparseddata/
---
## LoadOptions.KeepUnparsedData property

Whether keep the unparsed data in memory for the Workbook when it is loaded from template file. Default is true.

```csharp
public bool KeepUnparsedData { get; set; }
```

### Remarks

For scenarios that user only needs to read some contents from template file and does not need to save the workbook back, set this property as false may improve performance, especially when using it together with some kind of LoadFilter,

### Examples

```csharp
// Called: options.KeepUnparsedData = (false);
[Test]
        public void Property_KeepUnparsedData()
        {
            LoadOptions options = new LoadOptions();
            options.ParsingFormulaOnOpen = (false);
            options.KeepUnparsedData = (false);
            options.CheckDataValid = (false);
            options.CheckExcelRestriction = (false);
            Workbook wb = new Workbook(Constants.sourcePath + "CELLSJAVA-45489.xlsx", options);
            wb.Save(Constants.destPath + "CellsJava45489.xls");
        }
```

### See Also

* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


