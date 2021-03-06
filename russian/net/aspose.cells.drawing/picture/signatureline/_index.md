---
title: SignatureLine
second_title: Справочник по Aspose.Cells для .NET API
description: Получает и устанавливает строку подписи
type: docs
weight: 160
url: /ru/net/aspose.cells.drawing/picture/signatureline/
---
## Picture.SignatureLine property

Получает и устанавливает строку подписи

```csharp
public SignatureLine SignatureLine { get; set; }
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
  // Создаем строку подписи object
SignatureLine s = new SignatureLine();
s.Signer = "Simon Zhao";
s.Title = "Development Lead";
s.Email = "Simon.Zhao@aspose.com";
  // Назначаем объект линии подписи Picture.
pic.SignatureLine = s;
  // Сохраняем файл Excel.
workbook.Save("result.xlsx");
```

### Смотрите также

* class [SignatureLine](../../signatureline)
* class [Picture](../../picture)
* пространство имен [Aspose.Cells.Drawing](../../picture)
* сборка [Aspose.Cells](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
