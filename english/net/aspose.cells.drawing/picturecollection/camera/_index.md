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
namespace AsposeCellsExamples
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

            // Access the first worksheet
            Worksheet worksheet = workbook.Worksheets[0];

            // Add some sample data to create a range
            worksheet.Cells["A1"].Value = "Sample Data";
            worksheet.Cells["B1"].Value = "More Data";
            worksheet.Cells["A2"].Value = "Row 2";
            worksheet.Cells["B2"].Value = "Row 2 Col 2";

            try
            {
                // Get the Pictures collection from the worksheet
                PictureCollection pictures = worksheet.Pictures;

                // Call the Camera method to create a camera picture
                // Parameters: row (top-left row), column (top-left column), range (source range)
                int pictureIndex = pictures.Camera(5, 1, "A1:B2");

                Console.WriteLine($"Camera picture added successfully at index: {pictureIndex}");

                // Save the workbook
                workbook.Save("CameraDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling Camera method: {ex.Message}");
            }
        }
    }
}
```

### See Also

* class [PictureCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


