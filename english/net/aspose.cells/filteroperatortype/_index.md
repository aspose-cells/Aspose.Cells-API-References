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
// Called: worksheet.AutoFilter.Custom(5, FilterOperatorType.Equal, &amp;quot;&amp;quot;, false, FilterOperatorType.GreaterThan, 500);
[Test]
        public void Type_FilterOperatorType()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;AutoFilter/CellsNet46029.xlsx&quot;);
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.AutoFilter.Range = &quot;B6:K6&quot;;
            worksheet.AutoFilter.Custom(4, FilterOperatorType.GreaterThan, 500);
            worksheet.AutoFilter.Refresh();
            Assert.IsTrue(worksheet.Cells.IsRowHidden(7));
            workbook = new Workbook(Constants.sourcePath + &quot;AutoFilter/CellsNet46029.xlsx&quot;);
            worksheet = workbook.Worksheets[0];
            worksheet.AutoFilter.Range = &quot;B6:K6&quot;;
            worksheet.AutoFilter.Custom(5, FilterOperatorType.Equal, &quot;&quot;, false, FilterOperatorType.GreaterThan, 500); 
            worksheet.AutoFilter.Refresh();
            Assert.IsFalse(worksheet.Cells.IsRowHidden(13));
            workbook = new Workbook(Constants.sourcePath + &quot;AutoFilter/CellsNet46029.xlsx&quot;);
            worksheet = workbook.Worksheets[0];
            worksheet.AutoFilter.Range = &quot;B6:K6&quot;;
            worksheet.AutoFilter.FilterTop10(5, false, false, 5); 
            worksheet.AutoFilter.Refresh();
            Assert.IsTrue(worksheet.Cells.IsRowHidden(13));
            workbook = new Workbook(Constants.sourcePath + &quot;AutoFilter/CellsNet46029.xlsx&quot;);
            worksheet = workbook.Worksheets[0];
            worksheet.AutoFilter.Range = &quot;B6:K6&quot;;
            worksheet.AutoFilter.FilterTop10(5, true, false, 5);
            worksheet.AutoFilter.Refresh();
            Assert.IsTrue(worksheet.Cells.IsRowHidden(13));
        }
```

### See Also

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


