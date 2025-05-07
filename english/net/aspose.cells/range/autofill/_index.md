---
title: Range.AutoFill
second_title: Aspose.Cells for .NET API Reference
description: Range method. Automaticall fill the target range
type: docs
url: /net/aspose.cells/range/autofill/
---
## AutoFill(Range) {#autofill}

Automaticall fill the target range.

```csharp
public void AutoFill(Range target)
```

| Parameter | Type | Description |
| --- | --- | --- |
| target | Range | the target range. |

### Examples

```csharp

[C#]

//Instantiating a Workbook object
Workbook workbook = new Workbook();
// Get the first Worksheet Cells.
Cells cells = workbook.Worksheets[0].Cells;
cells["A1"].PutValue(1);
cells["A2"].PutValue(2);
Aspose.Cells.Range source = cells.CreateRange("A1:A2");
Aspose.Cells.Range target = cells.CreateRange("A3:A10");
//fill 3,4,5....10 to the range A3:A10
source.AutoFill(target);
//Save the Excel file
workbook.Save("book1.xlsm");

 [Visual Basic]

'Instantiating a Workbook object
Dim workbook As Workbook = New Workbook("Book1.xlsx")
// Get the first Worksheet Cells.
Dim cells as Cells = workbook.Worksheets[0].Cells
cells("A1").PutValue(1)
cells("A2").PutValue(2)
Dim source as Aspose.Cells.Range = cells.CreateRange("A1:A2")
Dim target as Aspose.Cells.Range = cells.CreateRange("A3:A10")
'fill 3,4,5....10 to the range A3:A10
source.AutoFill(target)
'Save the Excel file
workbook.Save("book1.xlsm")
```

### See Also

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## AutoFill(Range, AutoFillType) {#autofill_1}

Automaticall fill the target range.

```csharp
public void AutoFill(Range target, AutoFillType autoFillType)
```

| Parameter | Type | Description |
| --- | --- | --- |
| target | Range | The targed range. |
| autoFillType | AutoFillType | The auto fill type. |

### Examples

```csharp
// Called: src.AutoFill(dest, AutoFillType.Series);
[Test]
        public void Method_AutoFillType_()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "CELLSNET49682.xlsx");
            Cells cells = workbook.Worksheets[0].Cells;
            Aspose.Cells.Range src = cells.CreateRange("C3:C4");
            Aspose.Cells.Range dest = cells.CreateRange("C5:C10");
            src.AutoFill(dest, AutoFillType.Series);
           Assert.AreEqual(1,workbook.Worksheets[0].ConditionalFormattings[0].RangeCount);
            workbook.Save(Constants.destPath + "CELLSNET49682.xlsx");
        }
```

### See Also

* enum [AutoFillType](../../autofilltype/)
* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


