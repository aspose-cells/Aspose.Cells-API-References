---
title: ConditionalFormattingIcon.GetImageData
second_title: Aspose.Cells for .NET API Reference
description: ConditionalFormattingIcon method. Gets the image data with the setting of cell
type: docs
url: /net/aspose.cells/conditionalformattingicon/getimagedata/
---
## ConditionalFormattingIcon.GetImageData method

Gets the image data with the setting of cell.

```csharp
public byte[] GetImageData(Cell cell)
```

| Parameter | Type | Description |
| --- | --- | --- |
| cell | Cell | The setting of cell. |

### Return Value

Returns the image data of icon.

### Examples

```csharp
// Called: byte[] d = icon.GetImageData(wb.Worksheets[0].Cells["E1"]);
public void ConditionalFormattingIcon_Method_GetImageData()
{
    Workbook wb = new Workbook(Constants.sourcePath + "example.xlsx");
    ConditionalFormattingIcon icon = wb.Worksheets[0].ConditionalFormattings[0][0].IconSet.CfIcons[0];
    byte[] d = icon.GetImageData(wb.Worksheets[0].Cells["E1"]);
    Assert.AreEqual(13,Image.FromStream(new MemoryStream(d)).Width);
    //d = icon.GetImageData(wb.Worksheets[0].Cells["F1"]);
    //File.WriteAllBytes(dir + "F1.png", d);
    d = icon.GetImageData(wb.Worksheets[0].Cells["G1"]);
    Assert.AreEqual(24,Image.FromStream(new MemoryStream(d)).Width);
}
```

### See Also

* class [Cell](../../cell/)
* class [ConditionalFormattingIcon](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


