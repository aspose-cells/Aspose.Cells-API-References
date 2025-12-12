---
title: ShapeCollection.AddLinkedPicture
second_title: Aspose.Cells for .NET API Reference
description: ShapeCollection method. Add a linked picture
type: docs
url: /net/aspose.cells.drawing/shapecollection/addlinkedpicture/
---
## ShapeCollection.AddLinkedPicture method

Add a linked picture.

```csharp
public Picture AddLinkedPicture(int topRow, int leftColumn, int height, int width, 
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
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ShapeCollectionMethodAddLinkedPictureWithInt32Int32Int32Int32StringDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            
            // Access the first worksheet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Add sample text to cell A1
            worksheet.Cells["A1"].PutValue("Image will be linked below:");
            
            // Add linked picture to the worksheet
            string imageUrl = "https://example.com/sample.jpg";
            worksheet.Shapes.AddLinkedPicture(1, 1, 100, 100, imageUrl);
            
            // Save the workbook
            workbook.Save("output_with_linked_picture.xlsx");
            
            Console.WriteLine("Workbook saved with linked picture.");
        }
    }
}
```

### See Also

* class [Picture](../../picture/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


