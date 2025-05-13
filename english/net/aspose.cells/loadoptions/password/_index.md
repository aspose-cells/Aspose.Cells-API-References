---
title: LoadOptions.Password
second_title: Aspose.Cells for .NET API Reference
description: LoadOptions property. Gets and set the password of the workbook
type: docs
url: /net/aspose.cells/loadoptions/password/
---
## LoadOptions.Password property

Gets and set the password of the workbook.

```csharp
public string Password { get; set; }
```

### Examples

```csharp
// Called: options.Password = "test";
public void LoadOptions_Property_Password()
{
    LoadOptions options = new LoadOptions();
    options.Password = "test";

    Workbook workbook = new Workbook(Constants.sourcePath + "example.xlsx", options);
    workbook.Settings.Password = null;

    Util.SaveForViewer(workbook, "13", "CellsNet46972.XLSx");
}
```

### See Also

* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


