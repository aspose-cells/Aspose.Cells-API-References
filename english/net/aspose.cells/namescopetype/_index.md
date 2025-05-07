---
title: Enum NameScopeType
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.NameScopeType enum. Represents the scope type of defined names
type: docs
url: /net/aspose.cells/namescopetype/
---
## NameScopeType enumeration

Represents the scope type of defined names.

```csharp
public enum NameScopeType
```

### Values

| Name | Value | Description |
| --- | --- | --- |
| All | `0` | All defined names. |
| Workbook | `1` | The defined names in the workbook. |
| Worksheet | `2` | The defined names in a worksheet or all worksheets. |

### Examples

```csharp
// Called: Assert.AreEqual(2, workbook.Worksheets.Names.Filter(NameScopeType.Worksheet, -1).Length);
[Test]
        public void Type_NameScopeType()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "CELLSNET50332.xlsx");

            Assert.AreEqual(1,workbook.Worksheets.Names.Filter(NameScopeType.Workbook, -1).Length);
            Assert.AreEqual(2, workbook.Worksheets.Names.Filter(NameScopeType.Worksheet, -1).Length);
            Assert.AreEqual(1, workbook.Worksheets.Names.Filter(NameScopeType.Worksheet, 1).Length);
            // Save the workbook
            workbook.Save(Constants.destPath + "dest.xlsx");
        }
```

### See Also

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


