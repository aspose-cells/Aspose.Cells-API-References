---
title: PageSetup.GetPicture
second_title: Aspose.Cells for .NET API Reference
description: PageSetup method. Gets the Picture object of the header / footer
type: docs
url: /net/aspose.cells/pagesetup/getpicture/
---
## GetPicture(bool, int) {#getpicture_1}

Gets the [`Picture`](../../../aspose.cells.drawing/picture/) object of the header / footer.

```csharp
public Picture GetPicture(bool isHeader, int section)
```

| Parameter | Type | Description |
| --- | --- | --- |
| isHeader | Boolean | Indicates whether it is in the header or footer. |
| section | Int32 | 0: Left Section, 1: Center Section, 2: Right Section. |

### Return Value

Returns [`Picture`](../../../aspose.cells.drawing/picture/) object. Returns null if there is no picture.

### Examples

```csharp
// Called: Assert.AreEqual(50, wb.Worksheets[0].PageSetup.GetPicture(true, 0).FormatPicture.Brightness);
public void PageSetup_Method_GetPicture()
{
    Workbook wb = new Workbook(Constants.sourcePath + "example.xlsx");
    Assert.AreEqual(50,wb.Worksheets[0].PageSetup.GetPicture(true, 0).FormatPicture.Brightness);
    wb.Combine(new Workbook(Constants.sourcePath + "example.xlsx"));
    wb = Util.ReSave(wb,SaveFormat.Xlsx);
    Assert.AreEqual(50, wb.Worksheets[0].PageSetup.GetPicture(true, 0).FormatPicture.Brightness);
}
```

### See Also

* class [Picture](../../../aspose.cells.drawing/picture/)
* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetPicture(bool, bool, bool, int) {#getpicture}

Gets the [`Picture`](../../../aspose.cells.drawing/picture/) object of the header / footer.

```csharp
public Picture GetPicture(bool isFirst, bool isEven, bool isHeader, int section)
```

| Parameter | Type | Description |
| --- | --- | --- |
| isFirst | Boolean | Indicates whether getting the picture of first page header/footer. |
| isEven | Boolean | Indicates whether getting the picture of even page header/footer. |
| isHeader | Boolean | Indicates whether getting the picture of header/footer. |
| section | Int32 | 0: Left Section, 1: Center Section, 2: Right Section. |

### Return Value

Returns [`Picture`](../../../aspose.cells.drawing/picture/) object.

### See Also

* class [Picture](../../../aspose.cells.drawing/picture/)
* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


