---
title: OriginalHeight
second_title: Справочник по Aspose.Cells для .NET API
description: Получает исходную высоту изображения.
type: docs
weight: 100
url: /ru/net/aspose.cells.drawing/picture/originalheight/
---
## Picture.OriginalHeight property

Получает исходную высоту изображения.

```csharp
public int OriginalHeight { get; }
```

### Примеры

```csharp

[C#]
  //Создание экземпляра рабочей книги object
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
  //Добавление изображения в ячейку, индексы строки и столбца которой равны 1 на рабочем листе. Это "B2" cell
int imgIndex = worksheet.Pictures.Add(1, 1, "example.jpeg");
  //Получить вставленную картинку object
Picture pic = worksheet.Pictures[imgIndex];
  //Получает исходную высоту изображения.
int picHeight = pic.OriginalHeight;
  // Сохраняем файл Excel.
workbook.Save("result.xlsx");
```

### Смотрите также

* class [Picture](../../picture)
* пространство имен [Aspose.Cells.Drawing](../../picture)
* сборка [Aspose.Cells](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->