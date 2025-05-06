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
            Workbook wbOrigin = new Workbook(Constants.sourcePath + &quot;CELLSNET53885.xlsx&quot;);
            var wbDestination = new Workbook();
            Console.WriteLine(&quot;&quot;);

            Console.WriteLine(&quot;Copy range from Origin to Destination&quot;);
            var rangeOrigin = wbOrigin.Worksheets[0].Cells.CreateRange(&quot;A1:E150&quot;);
            var rangeDestination = wbDestination.Worksheets[0].Cells.CreateRange(&quot;A1:E150&quot;);
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
            Cell b7 = wbDestination.Worksheets[0].Cells[&quot;B7&quot;];
            Style style = b7.GetStyle(false);
            Assert.AreEqual(CellBorderType.Thin, style.Borders[BorderType.TopBorder].LineStyle);
        }
```

### See Also

* enum [PasteOperationType](../../pasteoperationtype/)
* class [PasteOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


