---
title: AutoFilter.MatchBlanks
second_title: Aspose.Cells for .NET API Reference
description: AutoFilter method. Match all blank cell in the list
type: docs
url: /net/aspose.cells/autofilter/matchblanks/
---
## AutoFilter.MatchBlanks method

Match all blank cell in the list.

```csharp
public void MatchBlanks(int fieldIndex)
```

| Parameter | Type | Description |
| --- | --- | --- |
| fieldIndex | Int32 | The integer offset of the field on which you want to base the filter (from the left of the list; the leftmost field is field 0). |

### Examples

```csharp
// Called: worksheet.AutoFilter.MatchBlanks(0);
[Test]
        public void Method_Int32_()
        {
            var workbook = new Workbook(Constants.sourcePath + &quot;CELLSNET55716.xlsx&quot;);
            var worksheet = workbook.Worksheets[0];
            worksheet.AutoFilter.MatchBlanks(0);
            worksheet.AutoFilter.Refresh();
            Assert.IsFalse(worksheet.Cells.Rows[2].IsHidden);
        }
```

### See Also

* class [AutoFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


