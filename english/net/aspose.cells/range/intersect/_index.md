---
title: Range.Intersect
second_title: Aspose.Cells for .NET API Reference
description: Range method. Returns a Range object that represents the rectangular intersection of two ranges
type: docs
url: /net/aspose.cells/range/intersect/
---
## Range.Intersect method

Returns a [`Range`](../) object that represents the rectangular intersection of two ranges.

```csharp
public Range Intersect(Range range)
```

| Parameter | Type | Description |
| --- | --- | --- |
| range | Range | The intersecting range. |

### Return Value

Returns a [`Range`](../) object

### Remarks

If the two ranges are not intersected, returns null.

### Examples

```csharp

[C#]

//Instantiating a Workbook object
Workbook workbook = new Workbook();
// Get the first Worksheet Cells.
Cells cells = workbook.Worksheets[0].Cells;
Range range1 = cells.CreateRange("A1:A5");
Range range2 = cells.CreateRange("A3:A10");
//Get intersected range of the two ranges.
Range intersectRange = range1.Intersect(range2);
//Save the Excel file
workbook.Save("book1.xlsm");

 [Visual Basic]

'Instantiating a Workbook object
Dim workbook As Workbook = New Workbook()
'Get the first Worksheet Cells.
Dim cells as Cells = workbook.Worksheets[0].Cells
Range range1 = cells.CreateRange("A1:A5")
Range range2 = cells.CreateRange("A3:A10")
'Get intersected range of the two ranges.
Range intersectRange = range1.Intersect(range2)
'Save the Excel file
workbook.Save("book1.xlsm")
```

### See Also

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


