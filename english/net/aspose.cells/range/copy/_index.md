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
// Called: destinationRange.Copy(sourceRange, new PasteOptions { SkipBlanks = false, PasteType = PasteType.All });
[Test]
        public void Method_PasteOptions_()
        {
            Workbook sourceWorkbook = new Workbook(Constants.sourcePath + &quot;CellsNet44861_in.xlsx&quot;);

            Worksheet sourceworksheet = sourceWorkbook.Worksheets[0];

            Aspose.Cells.Range sourceRange = sourceworksheet.Cells.CreateRange(1, 7, 99999, 1);

            Workbook destinationWorkbook = new Workbook(Constants.sourcePath + &quot;CellsNet44861_out.xlsx&quot;);
            Worksheet destinationWorksheet = destinationWorkbook.Worksheets[0];

            Aspose.Cells.Range destinationRange = destinationWorksheet.
            Cells.CreateRange(0, 0, sourceRange.RowCount, sourceRange.ColumnCount);

            destinationRange.Copy(sourceRange, new PasteOptions { SkipBlanks = false, PasteType = PasteType.All });
            destinationWorkbook.Save(Constants.destPath + &quot;CellsNet44861.xlsx&quot;);
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


