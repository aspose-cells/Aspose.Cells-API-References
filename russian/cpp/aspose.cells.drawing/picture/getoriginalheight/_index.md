---
title: Aspose::Cells::Drawing::Picture::GetOriginalHeight method
linktitle: GetOriginalHeight
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Drawing::Picture::GetOriginalHeight method. Gets the original height of the picture in C++.'
type: docs
weight: 1100
url: /ru/cpp/aspose.cells.drawing/picture/getoriginalheight/
---
## Picture::GetOriginalHeight method


Gets the original height of the picture.

```cpp
int32_t Aspose::Cells::Drawing::Picture::GetOriginalHeight()
```


## Examples


```cpp
Aspose::Cells::Startup();
//Создание экземпляра объекта Workbook
Workbook workbook;
Worksheet worksheet = workbook.GetWorksheets().Get(0);
//Добавление изображения в ячейку, у которой индексы строки и столбца равны 1 в листе. Это ячейка "B2".
int imgIndex = worksheet.GetPictures().Add(1, 1, u"example.jpeg");
//Получить вставленный объект изображения
Picture pic = worksheet.GetPictures().Get(imgIndex);
//Получает исходную высоту изображения.
int picHeight = pic.GetOriginalHeight();
//Сохранить файл Excel.
workbook.Save(u"result.xlsx");
Aspose::Cells::Cleanup();
```

## See Also

* Class [Vector](../../../aspose.cells/vector/)
* Class [Picture](../)
* Namespace [Aspose::Cells::Drawing](../../)
* Library [Aspose.Cells for C++](../../../)
