---
title: "PictureCollection.Add"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод PictureCollection. Добавляет изображение в коллекцию"
type: docs
url: /ru/net/aspose.cells.drawing/picturecollection/add/
---
## Add(int, int, int, int, Stream) {#add}

Добавляет изображение в коллекцию.

```csharp
public int Add(int topRow, int leftColumn, int bottomRow, int rightColumn, Stream stream)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| topRow | Int32 | Индекс строки в верхнем левом углу. |
| leftColumn | Int32 | Индекс столбца в верхнем левом углу. |
| bottomRow | Int32 | Индекс строки нижнего правого угла |
| rightColumn | Int32 | Индекс столбца нижнего правого угла |
| поток | Stream | Объект Stream, содержащий данные изображения. |

### Возвращаемое значение

[`Picture`](../../picture/) object index.

### Примеры

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
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить изображение из потока
            using (FileStream fs = new FileStream("image.jpg", FileMode.Open))
            {
                worksheet.Pictures.Add(10, 10, 200, 200, fs);
            }

            // Сохраните книгу
            workbook.Save("output.xlsx");
        }
    }
}
```

### См. также

* class [PictureCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)

---

## Add(int, int, int, int, string) {#add_1}

Добавляет изображение в коллекцию.

```csharp
public int Add(int topRow, int leftColumn, int bottomRow, int rightColumn, string fileName)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| topRow | Int32 | Индекс строки в верхнем левом углу. |
| leftColumn | Int32 | Индекс столбца в верхнем левом углу. |
| bottomRow | Int32 | Индекс строки нижнего правого угла |
| rightColumn | Int32 | Индекс столбца нижнего правого угла |
| fileName | String | Имя файла изображения. |

### Возвращаемое значение

[`Picture`](../../picture/) object index.

### Примеры

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

### См. также

* class [PictureCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)

---

## Add(int, int, Stream) {#add_2}

Добавляет изображение в коллекцию.

```csharp
public int Add(int topRow, int leftColumn, Stream stream)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| topRow | Int32 | Индекс строки в верхнем левом углу. |
| leftColumn | Int32 | Индекс столбца в верхнем левом углу. |
| поток | Stream | Объект Stream, содержащий данные изображения. |

### Возвращаемое значение

[`Picture`](../../picture/) object index.

### Примеры

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
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить изображение из потока
            using (FileStream fs = new FileStream("image.jpg", FileMode.Open))
            {
                worksheet.Pictures.Add(1, 1, fs);
            }

            // Сохраните книгу
            workbook.Save("output.xlsx");
        }
    }
}
```

### См. также

* class [PictureCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)

---

## Add(int, int, string) {#add_4}

Добавляет изображение в коллекцию.

```csharp
public int Add(int topRow, int leftColumn, string fileName)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| topRow | Int32 | Индекс строки в верхнем левом углу. |
| leftColumn | Int32 | Индекс столбца в верхнем левом углу. |
| fileName | String | Имя файла изображения. |

### Возвращаемое значение

[`Picture`](../../picture/) object index.

### Примеры

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

### См. также

* class [PictureCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)

---

## Add(int, int, Stream, int, int) {#add_3}

Добавляет изображение в коллекцию.

```csharp
public int Add(int topRow, int leftColumn, Stream stream, int widthScale, int heightScale)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| topRow | Int32 | Индекс строки в верхнем левом углу. |
| leftColumn | Int32 | Индекс столбца в верхнем левом углу. |
| поток | Stream | Объект Stream, содержащий данные изображения. |
| widthScale | Int32 | Масштаб ширины изображения, в процентах. |
| heightScale | Int32 | Масштаб высоты изображения, в процентах. |

### Возвращаемое значение

[`Picture`](../../picture/) object index.

### Примеры

```csharp

[C#]
//добавить изображение
using (FileStream fs = new FileStream("image.jpg", FileMode.Open))
{
    pictures.Add(1, 1, fs, 50, 50);
}
```

### См. также

* class [PictureCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)

---

## Add(int, int, string, int, int) {#add_5}

Добавляет изображение в коллекцию.

```csharp
public int Add(int topRow, int leftColumn, string fileName, int widthScale, int heightScale)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| topRow | Int32 | Индекс строки в верхнем левом углу. |
| leftColumn | Int32 | Индекс столбца в верхнем левом углу. |
| fileName | String | Имя файла изображения. |
| widthScale | Int32 | Масштаб ширины изображения, в процентах. |
| heightScale | Int32 | Масштаб высоты изображения, в процентах. |

### Возвращаемое значение

[`Picture`](../../picture/) object index.

### Примеры

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

### См. также

* class [PictureCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


