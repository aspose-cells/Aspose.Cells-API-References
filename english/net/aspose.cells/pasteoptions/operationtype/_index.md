---
title: PasteOptions.OperationType
second_title: Aspose.Cells for .NET API Reference
description: PasteOptions property. Gets and sets the operation type when pasting range
type: docs
url: /net/aspose.cells/pasteoptions/operationtype/
---
## PasteOptions.OperationType property

Gets and sets the operation type when pasting range.

```csharp
public PasteOperationType OperationType { get; set; }
```

### Examples

```csharp
// Called: OperationType = PasteOperationType.None,
[Test]
        public void Property_OperationType()
        {
            Workbook wbOrigin = new Workbook(Constants.sourcePath + "CELLSNET53885.xlsx");
            var wbDestination = new Workbook();
            Console.WriteLine("");

            Console.WriteLine("Copy range from Origin to Destination");
            var rangeOrigin = wbOrigin.Worksheets[0].Cells.CreateRange("A1:E150");
            var rangeDestination = wbDestination.Worksheets[0].Cells.CreateRange("A1:E150");
            var options = new PasteOptions
            {
                PasteType = PasteType.All,
                //SkipBlanks = false,
                OnlyVisibleCells = false,
                Transpose = false,
                OperationType = PasteOperationType.None,
                IgnoreLinksToOriginalFile = false
            };
            rangeDestination.Copy(rangeOrigin, options);
            Cell b7 = wbDestination.Worksheets[0].Cells["B7"];
            Style style = b7.GetStyle(false);
            Assert.AreEqual(CellBorderType.Thin, style.Borders[BorderType.TopBorder].LineStyle);
        }
```

### See Also

* enum [PasteOperationType](../../pasteoperationtype/)
* class [PasteOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


