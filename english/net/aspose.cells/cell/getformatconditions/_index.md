---
title: Cell.GetFormatConditions
second_title: Aspose.Cells for .NET API Reference
description: Cell method. Gets format conditions which applies to this cell
type: docs
url: /net/aspose.cells/cell/getformatconditions/
---
## Cell.GetFormatConditions method

Gets format conditions which applies to this cell.

```csharp
public FormatConditionCollection[] GetFormatConditions()
```

### Return Value

Returns [`FormatConditionCollection`](../../formatconditioncollection/) object

### Examples

```csharp
// Called: Assert.IsTrue(cells[&amp;quot;E2&amp;quot;].GetFormatConditions() != null);
[Test]
        public void Method_GetFormatConditions()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;CellsNet43650.xlsx&quot;);
         

            Worksheet worksheet = workbook.Worksheets[0];


            Cells cells = worksheet.Cells;


            //Copy columns does not copy conditional formatting 

            cells.CopyColumns(cells, 1, 4, 2);

            Assert.IsTrue(cells[&quot;E2&quot;].GetFormatConditions() != null);


        }
```

### See Also

* class [FormatConditionCollection](../../formatconditioncollection/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


