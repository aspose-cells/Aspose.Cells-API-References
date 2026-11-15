---
title: Aspose::Cells::Drawing::Picture::SetBorderWeight method
linktitle: SetBorderWeight
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Drawing::Picture::SetBorderWeight method. Gets or sets the weight of the border line of a picture in units of pt in C++.'
type: docs
weight: 1600
url: /ru/cpp/aspose.cells.drawing/picture/setborderweight/
---
## Picture::SetBorderWeight method


Gets or sets the weight of the border line of a picture in units of pt.

```cpp
void Aspose::Cells::Drawing::Picture::SetBorderWeight(double value)
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
pic.SetBorderLineColor(Color{ 0xff, 0xff, 0, 0 });//Red
//Установить ширину границы изображения
if (pic.GetBorderWeight() == 3)
{
    pic.SetBorderWeight(3);
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
