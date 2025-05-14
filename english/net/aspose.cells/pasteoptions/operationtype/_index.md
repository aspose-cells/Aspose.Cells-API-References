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
public void PasteOptions_Property_OperationType()
{
    Workbook wbOrigin = new Workbook(Constants.sourcePath + "example.xlsx");
    var wbDestination = new Workbook(Path.Combine(Constants.sourcePath, "example.xlsx"));
           
    var rangeOrigin = wbOrigin.Worksheets[0].Cells.CreateRange("A1:E150");
    var rangeDestination = wbDestination.Worksheets[0].Cells.CreateRange("A1:E150");
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
    Cell b2 = wbDestination.Worksheets[0].Cells["B2"];
    Style style = b2.GetStyle(false);
    Assert.AreEqual(CellBorderType.Thin, style.Borders[BorderType.BottomBorder].LineStyle);
    wbDestination.Save(Path.Combine(Constants.destPath, "example.xlsx"), SaveFormat.Xlsx);
}
```

### See Also

* enum [PasteOperationType](../../pasteoperationtype/)
* class [PasteOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


