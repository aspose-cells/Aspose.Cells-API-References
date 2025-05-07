---
title: Cells.GetCellsWithPlaceInCellPicture
second_title: Aspose.Cells for .NET API Reference
description: Cells method. Gets all cells that contain embedded picture
type: docs
url: /net/aspose.cells/cells/getcellswithplaceincellpicture/
---
## Cells.GetCellsWithPlaceInCellPicture method

Gets all cells that contain embedded picture.

```csharp
public IEnumerator GetCellsWithPlaceInCellPicture()
```

### Return Value

Enumerator to enumerate all Cell objects that contain embedded picture

### Remarks

If there is no picture which is set as "Place in Cell" in this worksheet, null will be returned.

### Examples

```csharp
// Called: for (IEnumerator ie = cells.GetCellsWithPlaceInCellPicture(); ie.MoveNext();)
[Test]
        public void Method_GetCellsWithPlaceInCellPicture()
        {
            Workbook workbook = new Workbook();
            workbook.Worksheets[0].Pictures.Add(0, 0, Constants.sourcePath + "2.png");
            workbook.Worksheets[0].Cells["B3"].EmbeddedImage = File.ReadAllBytes(Constants.sourcePath + "1.png");
            workbook.Worksheets[0].Pictures.RemoveAt(0);
            Assert.IsTrue(workbook.Worksheets[0].Cells["B3"].EmbeddedImage != null);


            //CELLSNET56093
            Cells cells = workbook.Worksheets[0].Cells;
            int count = 0;
            for (IEnumerator ie = cells.GetCellsWithPlaceInCellPicture(); ie.MoveNext();)
            {
                Cell cell = (Cell)ie.Current;
                byte[] data = cell.EmbeddedImage;
                Assert.IsTrue(data != null);
                count++;
            }
            Assert.AreEqual(1, count);


            workbook.Save(Constants.destPath + "CELLSNET56093.xlsx");
            workbook = new Workbook(Constants.destPath + "CELLSNET56093.xlsx");
             cells = workbook.Worksheets[0].Cells;
             count = 0;
            for (IEnumerator ie = cells.GetCellsWithPlaceInCellPicture(); ie.MoveNext();)
            {
                Cell cell = (Cell)ie.Current;
                byte[] data = cell.EmbeddedImage;
                Assert.IsTrue(data != null);
                count++;
            }
            Assert.AreEqual(1, count);
        }
```

### See Also

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


