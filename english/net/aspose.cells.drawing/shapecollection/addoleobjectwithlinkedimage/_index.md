---
title: ShapeCollection.AddOleObjectWithLinkedImage
second_title: Aspose.Cells for .NET API Reference
description: ShapeCollection method. Add a linked picture
type: docs
url: /net/aspose.cells.drawing/shapecollection/addoleobjectwithlinkedimage/
---
## ShapeCollection.AddOleObjectWithLinkedImage method

Add a linked picture.

```csharp
public OleObject AddOleObjectWithLinkedImage(int topRow, int leftColumn, int height, int width, 
    string sourceFullName)
```

| Parameter | Type | Description |
| --- | --- | --- |
| topRow | Int32 | Upper left row index. |
| leftColumn | Int32 | Upper left column index. |
| height | Int32 | The height of the shape. In unit of pixels |
| width | Int32 | The width of the shape. In unit of pixels |
| sourceFullName | String | The path and name of the source file for the linked image |

### Return Value

[`Picture`](../../picture/) Picture object.

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ShapeCollectionMethodAddOleObjectWithLinkedImageWithInt32Int32Int32Int32StringDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Path to the image file to be linked
            string imagePath = "example.jpg";

            try
            {
                // Call the AddOleObjectWithLinkedImage method with specific parameters
                OleObject oleObject = worksheet.Shapes.AddOleObjectWithLinkedImage(
                    1,  // upperLeftRow
                    1,  // upperLeftColumn
                    200, // height
                    300, // width
                    imagePath); // sourceFullName

                // Set additional properties for the OleObject
                oleObject.DisplayAsIcon = false;
                oleObject.IsAutoSize = true;

                Console.WriteLine("OLE object with linked image added successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing AddOleObjectWithLinkedImage method: {ex.Message}");
            }

            // Save the workbook
            workbook.Save("AddOleObjectWithLinkedImageDemo.xlsx");
        }
    }
}
```

### See Also

* class [OleObject](../../oleobject/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


