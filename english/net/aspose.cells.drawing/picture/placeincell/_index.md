---
title: Picture.PlaceInCell
second_title: Aspose.Cells for .NET API Reference
description: Picture method. Place this picture in the cell
type: docs
url: /net/aspose.cells.drawing/picture/placeincell/
---
## Picture.PlaceInCell method

Place this picture in the cell

```csharp
public void PlaceInCell()
```

### Examples

```csharp
// Called: picture.PlaceInCell();
public void Picture_Method_PlaceInCell()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "example.xlsm");
    Worksheet worksheet = workbook.Worksheets[0];
    foreach (Picture picture in worksheet.Pictures.Reverse())
    {
        int row = picture.UpperLeftRow;
        int column = picture.UpperLeftColumn;

        // Convert row and column to an Excel cell name
        string cellName = CellsHelper.CellIndexToName(row, column);

        if (cellName == "H13")
        {

            picture.PlaceInCell();
            // worksheet.Cells.UnMerge(161, 0, 11, 4);
                    
            break;

        }
    }
    Cell cell = worksheet.Cells["H13"];
    byte[] data = cell.EmbeddedImage;
    Assert.AreEqual(0x89, data[0]);
          
}
```

### See Also

* class [Picture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


