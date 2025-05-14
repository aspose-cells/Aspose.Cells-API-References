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
// Called: worksheet.AutoFilter.Custom(0, FilterOperatorType.BeginsWith, "Bo");
public void Cells_Type_FilterOperatorType()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "example.xlsx");
    // Accessing the first worksheet in the Excel file
    Worksheet worksheet = workbook.Worksheets[0];
    // Creating AutoFilter by giving the cells range
    worksheet.AutoFilter.Range = "A1:A18";
    // Initialize filter for rows containing string "Ba"
    worksheet.AutoFilter.Custom(0, FilterOperatorType.BeginsWith, "Bo");
    //Refresh the filter to show/hide filtered rows
    worksheet.AutoFilter.Refresh();
    Assert.IsFalse(worksheet.Cells.IsRowHidden(10));
    // Saving the modified Excel file
    Util.ReSave(workbook, SaveFormat.Xlsx);//.Save(Constants.destPath + "example.xlsx");
}
```

### See Also

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


