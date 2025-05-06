---
title: Cells.GetViewColumnWidthPixel
second_title: Aspose.Cells for .NET API Reference
description: Cells method. Get the width in different view type
type: docs
url: /net/aspose.cells/cells/getviewcolumnwidthpixel/
---
## Cells.GetViewColumnWidthPixel method

Get the width in different view type.

```csharp
public int GetViewColumnWidthPixel(int column)
```

| Parameter | Type | Description |
| --- | --- | --- |
| column | Int32 | The column index. |

### Return Value

the column width in unit of pixels

### Examples

```csharp
// Called: Assert.AreEqual(sheetLayout.Cells.GetViewColumnWidthPixel(0), 67);
[Test]
        public void Method_Int32_()
        {
            FileStream imageStream = File.OpenRead(Constants.sourcePath + &quot;image1.png&quot;);
            Workbook workbook = new Workbook();       // Add map image to sheet with NormalView.     
            // The image will have 100% width and height scaling, but this    
            // does not print the image accurately.  
            Worksheet sheetNormal = workbook.Worksheets.Add(&quot;Map Image Normal View&quot;);
            sheetNormal.ViewType = ViewType.NormalView;
            sheetNormal.Pictures.Add(0, 0, imageStream);
            // Here I try to insert the image to a worksheet that is in    
            // PageLayout view.  However, the image will have 105% width     
            // when viewed in Page Layout view.  It will not print accurately either.  
            Worksheet sheetLayout = workbook.Worksheets.Add(&quot;Map Image Layout View&quot;);
            sheetLayout.ViewType = ViewType.PageLayoutView;
            Assert.AreEqual(sheetLayout.Cells.GetViewColumnWidthPixel(0), 67);
            int index = sheetLayout.Pictures.Add(0, 0, imageStream);
            var mapPicture = sheetLayout.Pictures[index];
            // The following lines make no difference.  The image properties will show     
            // the width being 105% in Page Layout view.
            mapPicture.Placement = PlacementType.Move;
            //mapPicture.HeightScale = 100;    
            //mapPicture.WidthScale = 90;//100/105
            String outputPath = Constants.destPath +&quot;MapImageTest.xlsx&quot;;
            workbook.Save(outputPath, SaveFormat.Xlsx);
        }
```

### See Also

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


