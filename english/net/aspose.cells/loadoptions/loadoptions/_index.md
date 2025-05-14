---
title: LoadOptions.LoadOptions
second_title: Aspose.Cells for .NET API Reference
description: LoadOptions constructor. Creates an options of loading the file
type: docs
url: /net/aspose.cells/loadoptions/loadoptions/
---
## LoadOptions() {#constructor}

Creates an options of loading the file.

```csharp
public LoadOptions()
```

### Examples

```csharp
// Called: LoadOptions options = new LoadOptions();
public void LoadOptions_Constructor()
{
    LoadOptions options = new LoadOptions();
    options.CheckDataValid = true;
    Workbook workbook = new Workbook(Constants.sourcePath + "example.xls", options);
    workbook.Save(Constants.destPath + "example.pdf");
}
```

### See Also

* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## LoadOptions(LoadFormat) {#constructor_1}

Creates an options of loading the file.

```csharp
public LoadOptions(LoadFormat loadFormat)
```

| Parameter | Type | Description |
| --- | --- | --- |
| loadFormat | LoadFormat | The loading format. |

### See Also

* enum [LoadFormat](../../loadformat/)
* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


