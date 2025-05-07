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
// Called: workbook.RemoveMacro();
[Test]
        public void Method_RemoveMacro()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "CELLSNET-47749.ods");
            workbook.RemoveMacro();
            Assert.IsFalse(workbook.HasMacro);
            workbook.Save(Constants.destPath + "CellsNet47749.ods");
        }
```

### See Also

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


