---
title: Aspose::Cells::Drawing::Picture::GetOriginalWidthCM method
linktitle: GetOriginalWidthCM
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Drawing::Picture::GetOriginalWidthCM method. Gets the original width of picture, in unit of centimeters in C++.'
type: docs
weight: 3300
url: /ru/cpp/aspose.cells.drawing/picture/getoriginalwidthcm/
---
## Picture::GetOriginalWidthCM method


Gets the original width of picture, in unit of centimeters.

```cpp
double Aspose::Cells::Drawing::Picture::GetOriginalWidthCM()
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
//Получает исходную ширину изображения.
double picWidthCM = pic.GetOriginalWidthCM();
//Сохранить файл Excel.
workbook.Save(u"result.xlsx");
Aspose::Cells::Cleanup();
```

## See Also

* Class [Vector](../../../aspose.cells/vector/)
* Class [Picture](../)
* Namespace [Aspose::Cells::Drawing](../../)
* Library [Aspose.Cells for C++](../../../)
