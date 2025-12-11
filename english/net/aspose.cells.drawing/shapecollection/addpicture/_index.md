---
title: ShapeCollection.AddPicture
second_title: Aspose.Cells for .NET API Reference
description: ShapeCollection method. Adds a picture to the collection
type: docs
url: /net/aspose.cells.drawing/shapecollection/addpicture/
---
## AddPicture(int, int, int, int, Stream) {#addpicture}

Adds a picture to the collection.

```csharp
public Picture AddPicture(int topRow, int leftColumn, int bottomRow, int rightColumn, Stream stream)
```

| Parameter | Type | Description |
| --- | --- | --- |
| topRow | Int32 | Upper left row index. |
| leftColumn | Int32 | Upper left column index. |
| bottomRow | Int32 | Lower right row index |
| rightColumn | Int32 | Lower right column index |
| stream | Stream | Stream object which contains the image data. |

### Return Value

[`Picture`](../../picture/) Picture object.

### Examples

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeCollectionMethodAddPictureWithInt32Int32Int32Int32StreamDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Get the shapes collection
            ShapeCollection shapes = worksheet.Shapes;

            // Add a picture from a file stream
            using (FileStream fs = new FileStream("image.jpg", FileMode.Open))
            {
                Picture picture = shapes.AddPicture(1, 0, 1, 0, fs);
            }

            // Save the workbook
            workbook.Save("output.xlsx");
        }
    }
}
```

### See Also

* class [Picture](../../picture/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)

---

## AddPicture(int, int, Stream, int, int) {#addpicture_1}

Adds a picture to the collection.

```csharp
public Picture AddPicture(int topRow, int leftColumn, Stream stream, int widthScale, 
    int heightScale)
```

| Parameter | Type | Description |
| --- | --- | --- |
| topRow | Int32 | Upper left row index. |
| leftColumn | Int32 | Upper left column index. |
| stream | Stream | Stream object which contains the image data. |
| widthScale | Int32 | Scale of image width, a percentage. |
| heightScale | Int32 | Scale of image height, a percentage. |

### Return Value

[`Picture`](../../picture/) Picture object.

### Examples

```csharp

[C#]
//add a picture
using (FileStream fs = new FileStream("image.jpg", FileMode.Open))
{
    Picture picture = shapes.AddPicture(1, 1, fs, 50, 60);
}
```

### See Also

* class [Picture](../../picture/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


