---
title: PictureCollection.Camera
second_title: Aspose.Cells for .NET API Reference
description: PictureCollection method. Takes a photo of the range
type: docs
url: /net/aspose.cells.drawing/picturecollection/camera/
---
## PictureCollection.Camera method

Takes a photo of the range.

```csharp
public int Camera(int row, int column, string range)
```

| Parameter | Type | Description |
| --- | --- | --- |
| row | Int32 | The row index of this picture. |
| column | Int32 | The column index of this picture. |
| range | String | The area that requires photography |

### Examples

```csharp
namespace AsposeCellsExamples.PictureCollectionMethodCameraWithInt32Int32StringDemo
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class PictureCollectionMethodCameraWithInt32Int32StringDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add some data to cells that will be captured by the camera
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Price");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["B2"].PutValue(2.5);
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["B3"].PutValue(1.8);

            try
            {
                // Get the picture collection
                PictureCollection pictures = worksheet.Pictures;

                // Use Add method to create a picture from the cell range
                int index = pictures.Add(5, 1, "A1:B3");
                Picture cameraPicture = pictures[index];

                Console.WriteLine("Camera effect created successfully with parameters (Int32, Int32, String)");

                // Save the workbook to see the camera effect
                workbook.Save("CameraMethodDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error creating camera effect: {ex.Message}");
            }
        }
    }
}
```

### See Also

* class [PictureCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


