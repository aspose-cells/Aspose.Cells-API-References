---
title: OriginalWidthCM
second_title: Справочник по Aspose.Cells для .NET API
description: Получает исходную ширину изображения в сантиметрах.
type: docs
weight: 140
url: /ru/net/aspose.cells.drawing/picture/originalwidthcm/
---
## Picture.OriginalWidthCM property

Получает исходную ширину изображения в сантиметрах.

```csharp
public double OriginalWidthCM { get; }
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
  //Получает исходную ширину изображения.
double picWidthCM = pic.OriginalWidthCM;
  // Сохраняем файл Excel.
workbook.Save("result.xlsx");
```

### Смотрите также

* class [Picture](../../picture)
* пространство имен [Aspose.Cells.Drawing](../../picture)
* сборка [Aspose.Cells](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
