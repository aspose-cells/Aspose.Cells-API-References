---
title: Worksheet.Pictures
second_title: Aspose.Cells for .NET API Reference
description: Worksheet property. Gets a Picture collection
type: docs
url: /net/aspose.cells/worksheet/pictures/
---
## Worksheet.Pictures property

Gets a [`Picture`](../../../aspose.cells.drawing/picture/) collection.

```csharp
public PictureCollection Pictures { get; }
```

### Examples

```csharp
// Called: WorkbookCompare.PicturesTest.equals(sheetSrc.Pictures, sheetDest.Pictures, "worksheet.Pictures");
private void Property_Pictures(Workbook workbook)
        {
            Worksheet sheetSrc = workbook.Worksheets[0];
            Worksheet sheetDest = workbook.Worksheets["sheetDest"];
            WorkbookCompare.PicturesTest.equals(sheetSrc.Pictures, sheetDest.Pictures, "worksheet.Pictures");
        }
```

### See Also

* class [PictureCollection](../../../aspose.cells.drawing/picturecollection/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


