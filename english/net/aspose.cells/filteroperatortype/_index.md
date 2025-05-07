---
title: Enum FilterOperatorType
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.FilterOperatorType enum. Custom Filter operator type
type: docs
url: /net/aspose.cells/filteroperatortype/
---
## FilterOperatorType enumeration

Custom Filter operator type.

```csharp
public enum FilterOperatorType
```

### Values

| Name | Value | Description |
| --- | --- | --- |
| LessOrEqual | `0` | Represents LessOrEqual operator. |
| LessThan | `1` | Represents LessThan operator. |
| Equal | `2` | Represents Equal operator. |
| GreaterThan | `3` | Represents GreaterThan operator. |
| NotEqual | `4` | Represents NotEqual operator. |
| GreaterOrEqual | `5` | Represents GreaterOrEqual operator. |
| None | `6` | Represents no comparison. |
| BeginsWith | `7` | Begins with the text. |
| EndsWith | `8` | Ends with the text. |
| Contains | `9` | Contains the text. |
| NotContains | `10` | Not contains the text. |
| NotBeginsWith | `11` | Not begins with the text. |
| NotEndsWith | `12` | Not ends with the text. |

### Examples

```csharp
// Called: sheet.AutoFilter.Custom(1,FilterOperatorType.Equal, "R?C2");
[Test]
        public void Type_FilterOperatorType()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "AutoFilter/TestCustom_001.xls");
            Worksheet sheet = workbook.Worksheets[0];
            sheet.AutoFilter.SetRange(0, 0, 1);
            sheet.AutoFilter.Custom(1,FilterOperatorType.Equal, "R?C2");
            sheet.AutoFilter.Refresh();
            Util.ReSave(workbook, SaveFormat.Excel97To2003); //.Save(Constants.destPath + "TestCustom_001.xls");
            Assert.AreEqual(sheet.Cells.GetRowHeight(3), 0);
            Assert.AreEqual(sheet.Cells.GetRowHeight(4), 12.75);
        }
```

### See Also

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


