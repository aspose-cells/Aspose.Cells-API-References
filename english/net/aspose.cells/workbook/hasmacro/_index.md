---
title: Workbook.HasMacro
second_title: Aspose.Cells for .NET API Reference
description: Workbook property. Indicates if this spreadsheet contains macro/VBA
type: docs
url: /net/aspose.cells/workbook/hasmacro/
---
## Workbook.HasMacro property

Indicates if this spreadsheet contains macro/VBA.

```csharp
public bool HasMacro { get; }
```

### Examples

```csharp
// Called: Assert.IsFalse(workbook.HasMacro);
[Test]
        public void Property_HasMacro()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;CELLSNET-47749.ods&quot;);
            workbook.RemoveMacro();
            Assert.IsFalse(workbook.HasMacro);
            workbook.Save(Constants.destPath + &quot;CellsNet47749.ods&quot;);
        }
```

### See Also

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


