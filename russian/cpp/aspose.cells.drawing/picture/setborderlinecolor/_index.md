---
title: Aspose::Cells::Drawing::Picture::SetBorderLineColor method
linktitle: SetBorderLineColor
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Drawing::Picture::SetBorderLineColor method. Represents the Color of the border line of a picture in C++.'
type: docs
weight: 1400
url: /ru/cpp/aspose.cells.drawing/picture/setborderlinecolor/
---
## Picture::SetBorderLineColor method


Represents the [Color](../../../aspose.cells/color/) of the border line of a picture.

```cpp
void Aspose::Cells::Drawing::Picture::SetBorderLineColor(const Aspose::Cells::Color &value)
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
//Установить цвет границы изображения
if (pic.GetBorderLineColor() == Color{ 0xff, 0, 0, 0xff })//Blue
{
    pic.SetBorderLineColor(Color{ 0xff, 0xff, 0, 0 });//Red
}
//Сохранить файл Excel.
workbook.Save(u"result.xlsx");
Aspose::Cells::Cleanup();
```

## See Also

* Class [Vector](../../../aspose.cells/vector/)
* Class [Picture](../)
* Namespace [Aspose::Cells::Drawing](../../)
* Library [Aspose.Cells for C++](../../../)
