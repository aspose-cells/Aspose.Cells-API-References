---
title: Range.Copy
second_title: Aspose.Cells for .NET API Reference
description: Range method. Copying the range with paste special options
type: docs
url: /net/aspose.cells/range/copy/
---
## Copy(Range, PasteOptions) {#copy_1}

Copying the range with paste special options.

```csharp
public void Copy(Range range, PasteOptions options)
```

| Parameter | Type | Description |
| --- | --- | --- |
| range | Range | The source range. |
| options | PasteOptions | The paste special options. |

### Examples

```csharp
// Called: range.Copy(source, options);
public void Range_Method_Copy()
{
    Workbook wb = new Workbook(Constants.sourcePath + "example.xlsx");

    Cells cells = wb.Worksheets[0].Cells;
    cells.InsertRows(32, 24, true);


    Aspose.Cells.Range range = cells.CreateRange(32, 1, 24, 18);
    Aspose.Cells.Range source = cells.CreateRange(8, 1, 24, 18);

    PasteOptions options = new PasteOptions();
    options.PasteType = (PasteType.All);
    range.Copy(source, options);

    Assert.AreEqual(1, cells["G52"].GetFormatConditions().Length);
    Assert.AreEqual(1, cells["G52"].GetFormatConditions()[0].Count);

    wb.Save(Constants.destPath + "example.xlsx");
}
```

### See Also

* class [PasteOptions](../../pasteoptions/)
* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Copy(Range) {#copy}

Copies data (including formulas), formatting, drawing objects etc. from a source range.

```csharp
public void Copy(Range range)
```

| Parameter | Type | Description |
| --- | --- | --- |
| range | Range | Source [`Range`](../) object. |

### Examples

```csharp

[C#]

//Instantiating a Workbook object
Workbook workbook = new Workbook();
// Get the first Worksheet Cells.
Cells cells = workbook.Worksheets[0].Cells;
Range range1 = cells.CreateRange("A1:A5");
Range range2 = cells.CreateRange("A6:A10");
//Copy the range.
range1.Copy(range2);
//Save the Excel file
workbook.Save("book1.xlsm");

 [Visual Basic]

'Instantiating a Workbook object
Dim workbook As Workbook = New Workbook()
'Get the first Worksheet Cells.
Dim cells as Cells = workbook.Worksheets[0].Cells
Range range1 = cells.CreateRange("A1:A5")
Range range2 = cells.CreateRange("A6:A10")
//Copy the range
range1.Copy(range2)
'Save the Excel file
workbook.Save("book1.xlsm")
```

### See Also

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


