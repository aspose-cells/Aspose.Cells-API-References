---
title: Enum PasteOperationType
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.PasteOperationType enum. Represents operation type when pasting range
type: docs
url: /net/aspose.cells/pasteoperationtype/
---
## PasteOperationType enumeration

Represents operation type when pasting range.

```csharp
public enum PasteOperationType
```

### Values

| Name | Value | Description |
| --- | --- | --- |
| None | `0` | No operation. |
| Add | `1` | Add |
| Subtract | `2` | Subtract |
| Multiply | `3` | Multiply |
| Divide | `4` | Divide |

### Examples

```csharp
// Called: OperationType = PasteOperationType.None,
[Test]
        public void Type_PasteOperationType()
        {
            Workbook wbOrigin = new Workbook(Constants.sourcePath + &quot;CELLSNET53984.xlsx&quot;);
            var wbDestination = new Workbook(Path.Combine(Constants.sourcePath, &quot;CELLSNET53984_Destination.xlsx&quot;));
           
            var rangeOrigin = wbOrigin.Worksheets[0].Cells.CreateRange(&quot;A1:E150&quot;);
            var rangeDestination = wbDestination.Worksheets[0].Cells.CreateRange(&quot;A1:E150&quot;);
            var options = new PasteOptions
            {
                PasteType = PasteType.All,
                SkipBlanks = false,
                OnlyVisibleCells = false,
                Transpose = false,
                OperationType = PasteOperationType.None,
                IgnoreLinksToOriginalFile = false
            };
            rangeDestination.Copy(rangeOrigin, options);
            Cell b2 = wbDestination.Worksheets[0].Cells[&quot;B2&quot;];
            Style style = b2.GetStyle(false);
            Assert.AreEqual(CellBorderType.Thin, style.Borders[BorderType.BottomBorder].LineStyle);
            wbDestination.Save(Path.Combine(Constants.destPath, &quot;CellsNet53984.xlsx&quot;), SaveFormat.Xlsx);
        }
```

### See Also

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


