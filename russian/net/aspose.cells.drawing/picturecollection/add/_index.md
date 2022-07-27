---
title: Add
second_title: Справочник по Aspose.Cells для .NET API
description: Добавляет картинку в коллекцию.
type: docs
weight: 20
url: /ru/net/aspose.cells.drawing/picturecollection/add/
---
## Add(int, int, int, int, Stream) {#add}

Добавляет картинку в коллекцию.

```csharp
public int Add(int upperLeftRow, int upperLeftColumn, int lowerRightRow, int lowerRightColumn, 
    Stream stream)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| upperLeftRow | Int32 | Индекс верхней левой строки. |
| upperLeftColumn | Int32 | Индекс левого верхнего столбца. |
| lowerRightRow | Int32 | Нижний индекс правой строки |
| lowerRightColumn | Int32 | Индекс нижнего правого столбца |
| stream | Stream | Потоковый объект, содержащий данные изображения. |

### Возвращаемое значение

[`Picture`](../../picture) индекс объекта.

### Примеры

```csharp

[C#]
//добавляем картинку
using (FileStream fs = new FileStream("image.jpg", FileMode.Open))
{
    pictures.Add(1, 1, 5, 5, fs);
}
```

### Смотрите также

* class [PictureCollection](../../picturecollection)
* пространство имен [Aspose.Cells.Drawing](../../picturecollection)
* сборка [Aspose.Cells](../../../)

---

## Add(int, int, int, int, string) {#add_1}

Добавляет картинку в коллекцию.

```csharp
public int Add(int upperLeftRow, int upperLeftColumn, int lowerRightRow, int lowerRightColumn, 
    string fileName)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| upperLeftRow | Int32 | Индекс верхней левой строки. |
| upperLeftColumn | Int32 | Индекс левого верхнего столбца. |
| lowerRightRow | Int32 | Нижний индекс правой строки |
| lowerRightColumn | Int32 | Индекс нижнего правого столбца |
| fileName | String | Имя файла изображения. |

### Возвращаемое значение

[`Picture`](../../picture) индекс объекта.

### Примеры

```csharp

[C#]
//добавляем картинку
pictures.Add(1, 1, 5, 5, "image.jpg");
```

### Смотрите также

* class [PictureCollection](../../picturecollection)
* пространство имен [Aspose.Cells.Drawing](../../picturecollection)
* сборка [Aspose.Cells](../../../)

---

## Add(int, int, Stream) {#add_2}

Добавляет картинку в коллекцию.

```csharp
public int Add(int upperLeftRow, int upperLeftColumn, Stream stream)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| upperLeftRow | Int32 | Индекс верхней левой строки. |
| upperLeftColumn | Int32 | Индекс левого верхнего столбца. |
| stream | Stream | Потоковый объект, содержащий данные изображения. |

### Возвращаемое значение

[`Picture`](../../picture) индекс объекта.

### Примеры

```csharp

[C#]
//добавляем картинку
using (FileStream fs = new FileStream("image.jpg", FileMode.Open))
{
    pictures.Add(1, 1, fs);
}
```

### Смотрите также

* class [PictureCollection](../../picturecollection)
* пространство имен [Aspose.Cells.Drawing](../../picturecollection)
* сборка [Aspose.Cells](../../../)

---

## Add(int, int, string) {#add_4}

Добавляет картинку в коллекцию.

```csharp
public int Add(int upperLeftRow, int upperLeftColumn, string fileName)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| upperLeftRow | Int32 | Индекс верхней левой строки. |
| upperLeftColumn | Int32 | Индекс левого верхнего столбца. |
| fileName | String | Имя файла изображения. |

### Возвращаемое значение

[`Picture`](../../picture) индекс объекта.

### Примеры

```csharp

[C#]
//добавляем картинку
pictures.Add(1, 1, "image.jpg");
```

### Смотрите также

* class [PictureCollection](../../picturecollection)
* пространство имен [Aspose.Cells.Drawing](../../picturecollection)
* сборка [Aspose.Cells](../../../)

---

## Add(int, int, Stream, int, int) {#add_3}

Добавляет картинку в коллекцию.

```csharp
public int Add(int upperLeftRow, int upperLeftColumn, Stream stream, int widthScale, 
    int heightScale)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| upperLeftRow | Int32 | Индекс верхней левой строки. |
| upperLeftColumn | Int32 | Индекс левого верхнего столбца. |
| stream | Stream | Потоковый объект, содержащий данные изображения. |
| widthScale | Int32 | Масштаб ширины изображения в процентах. |
| heightScale | Int32 | Масштаб высоты изображения в процентах. |

### Возвращаемое значение

[`Picture`](../../picture) индекс объекта.

### Примеры

```csharp

[C#]
//добавляем картинку
using (FileStream fs = new FileStream("image.jpg", FileMode.Open))
{
    pictures.Add(1, 1, fs, 50, 50);
}
```

### Смотрите также

* class [PictureCollection](../../picturecollection)
* пространство имен [Aspose.Cells.Drawing](../../picturecollection)
* сборка [Aspose.Cells](../../../)

---

## Add(int, int, string, int, int) {#add_5}

Добавляет картинку в коллекцию.

```csharp
public int Add(int upperLeftRow, int upperLeftColumn, string fileName, int widthScale, 
    int heightScale)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| upperLeftRow | Int32 | Индекс верхней левой строки. |
| upperLeftColumn | Int32 | Индекс левого верхнего столбца. |
| fileName | String | Имя файла изображения. |
| widthScale | Int32 | Масштаб ширины изображения в процентах. |
| heightScale | Int32 | Масштаб высоты изображения в процентах. |

### Возвращаемое значение

[`Picture`](../../picture) индекс объекта.

### Примеры

```csharp

[C#]
//добавляем картинку
pictures.Add(1, 1, "image.jpg", 50, 50);
```

### Смотрите также

* class [PictureCollection](../../picturecollection)
* пространство имен [Aspose.Cells.Drawing](../../picturecollection)
* сборка [Aspose.Cells](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
