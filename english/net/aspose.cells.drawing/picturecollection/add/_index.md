---
title: PictureCollection.Add
second_title: Aspose.Cells for .NET API Reference
description: PictureCollection method. Adds a picture to the collection
type: docs
url: /net/aspose.cells.drawing/picturecollection/add/
---
## Add(int, int, int, int, Stream) {#add}

Adds a picture to the collection.

```csharp
public int Add(int topRow, int leftColumn, int bottomRow, int rightColumn, Stream stream)
```

| Parameter | Type | Description |
| --- | --- | --- |
| topRow | Int32 | Upper left row index. |
| leftColumn | Int32 | Upper left column index. |
| bottomRow | Int32 | Lower right row index |
| rightColumn | Int32 | Lower right column index |
| stream | Stream | Stream object which contains the image data. |

### Return Value

[`Picture`](../../picture/) object index.

### Examples

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PictureCollectionMethodAddWithInt32Int32Int32Int32StreamDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add a picture from stream
            using (FileStream fs = new FileStream("image.jpg", FileMode.Open))
            {
                worksheet.Pictures.Add(10, 10, 200, 200, fs);
            }

            // Save the workbook
            workbook.Save("output.xlsx");
        }
    }
}
```

### See Also

* class [PictureCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)

---

## Add(int, int, int, int, string) {#add_1}

Adds a picture to the collection.

```csharp
public int Add(int topRow, int leftColumn, int bottomRow, int rightColumn, string fileName)
```

| Parameter | Type | Description |
| --- | --- | --- |
| topRow | Int32 | Upper left row index. |
| leftColumn | Int32 | Upper left column index. |
| bottomRow | Int32 | Lower right row index |
| rightColumn | Int32 | Lower right column index |
| fileName | String | Image filename. |

### Return Value

[`Picture`](../../picture/) object index.

### Examples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class PictureCollectionMethodAddWithInt32Int32Int32Int32StringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            PictureCollection pictures = worksheet.Pictures;
            pictures.Add(1, 1, 5, 5, "image.jpg");

            workbook.Save("output.xlsx");
        }
    }
}
```

### See Also

* class [PictureCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)

---

## Add(int, int, Stream) {#add_2}

Adds a picture to the collection.

```csharp
public int Add(int topRow, int leftColumn, Stream stream)
```

| Parameter | Type | Description |
| --- | --- | --- |
| topRow | Int32 | Upper left row index. |
| leftColumn | Int32 | Upper left column index. |
| stream | Stream | Stream object which contains the image data. |

### Return Value

[`Picture`](../../picture/) object index.

### Examples

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PictureCollectionMethodAddWithInt32Int32StreamDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add a picture from stream
            using (FileStream fs = new FileStream("image.jpg", FileMode.Open))
            {
                worksheet.Pictures.Add(1, 1, fs);
            }

            // Save the workbook
            workbook.Save("output.xlsx");
        }
    }
}
```

### See Also

* class [PictureCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)

---

## Add(int, int, string) {#add_4}

Adds a picture to the collection.

```csharp
public int Add(int topRow, int leftColumn, string fileName)
```

| Parameter | Type | Description |
| --- | --- | --- |
| topRow | Int32 | Upper left row index. |
| leftColumn | Int32 | Upper left column index. |
| fileName | String | Image filename. |

### Return Value

[`Picture`](../../picture/) object index.

### Examples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PictureCollectionMethodAddWithInt32Int32StringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            Aspose.Cells.Drawing.PictureCollection pictures = worksheet.Pictures;
            pictures.Add(1, 1, "image.jpg");

            workbook.Save("output.xlsx");
        }
    }
}
```

### See Also

* class [PictureCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)

---

## Add(int, int, Stream, int, int) {#add_3}

Adds a picture to the collection.

```csharp
public int Add(int topRow, int leftColumn, Stream stream, int widthScale, int heightScale)
```

| Parameter | Type | Description |
| --- | --- | --- |
| topRow | Int32 | Upper left row index. |
| leftColumn | Int32 | Upper left column index. |
| stream | Stream | Stream object which contains the image data. |
| widthScale | Int32 | Scale of image width, a percentage. |
| heightScale | Int32 | Scale of image height, a percentage. |

### Return Value

[`Picture`](../../picture/) object index.

### Examples

```csharp

[C#]
//add a picture
using (FileStream fs = new FileStream("image.jpg", FileMode.Open))
{
    pictures.Add(1, 1, fs, 50, 50);
}
```

### See Also

* class [PictureCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)

---

## Add(int, int, string, int, int) {#add_5}

Adds a picture to the collection.

```csharp
public int Add(int topRow, int leftColumn, string fileName, int widthScale, int heightScale)
```

| Parameter | Type | Description |
| --- | --- | --- |
| topRow | Int32 | Upper left row index. |
| leftColumn | Int32 | Upper left column index. |
| fileName | String | Image filename. |
| widthScale | Int32 | Scale of image width, a percentage. |
| heightScale | Int32 | Scale of image height, a percentage. |

### Return Value

[`Picture`](../../picture/) object index.

### Examples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class PictureCollectionMethodAddWithInt32Int32StringInt32Int32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            PictureCollection pictures = worksheet.Pictures;
            pictures.Add(1, 1, "image.jpg", 50, 50);

            workbook.Save("output.xlsx");
        }
    }
}
```

### See Also

* class [PictureCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


