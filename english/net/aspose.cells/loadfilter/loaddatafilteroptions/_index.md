---
title: LoadFilter.LoadDataFilterOptions
second_title: Aspose.Cells for .NET API Reference
description: LoadFilter property. The filter options to denote what data should be loaded
type: docs
url: /net/aspose.cells/loadfilter/loaddatafilteroptions/
---
## LoadFilter.LoadDataFilterOptions property

The filter options to denote what data should be loaded.

```csharp
public LoadDataFilterOptions LoadDataFilterOptions { get; set; }
```

### Examples

```csharp
// Called: option.LoadFilter.LoadDataFilterOptions = LoadDataFilterOptions.CellData | LoadDataFilterOptions.DefinedNames;
public void LoadFilter_Property_LoadDataFilterOptions()
{
    LoadOptions option = new LoadOptions();
    option.LoadFilter.LoadDataFilterOptions = LoadDataFilterOptions.CellData | LoadDataFilterOptions.DefinedNames;
    Workbook workbook = new Workbook(Constants.sourcePath + "example.xls", option);
    //workbook.LoadData(Constants.sourcePath + "example.xls");
    workbook.Save(Constants.destPath + "example.xls");
}
```

### See Also

* enum [LoadDataFilterOptions](../../loaddatafilteroptions/)
* class [LoadFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


