---
title: Workbook.RemoveMacro
second_title: Aspose.Cells for .NET API Reference
description: Workbook method. Removes VBA/macro from this spreadsheet
type: docs
url: /net/aspose.cells/workbook/removemacro/
---
## Workbook.RemoveMacro method

Removes VBA/macro from this spreadsheet.

```csharp
public void RemoveMacro()
```

### Examples

```csharp
// Called: wb1.RemoveMacro(); //This doesn't fix either
public void Workbook_Method_RemoveMacro()
{
    Workbook wb1 = new Workbook(Constants.sourcePath + "example.xlsm");
    Workbook wb2 = new Workbook(Constants.sourcePath + "example.xlsm");

    wb1.RemoveMacro(); //This doesn't fix either 

    wb2.Combine(wb1);
    wb2.Save(Constants.destPath + "example.xlsm");
}
```

### See Also

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


