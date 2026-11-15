---
title: Aspose::Cells::Drawing::Picture::GetData method
linktitle: GetData
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Drawing::Picture::GetData method. Gets the data of the picture in C++.'
type: docs
weight: 1700
url: /ru/cpp/aspose.cells.drawing/picture/getdata/
---
## Picture::GetData method


Gets the data of the picture.

```cpp
Vector<uint8_t> Aspose::Cells::Drawing::Picture::GetData()
```


## Examples


```cpp
Aspose::Cells::Startup();
//Создание экземпляра объекта Workbook
Workbook workbook;
Worksheet worksheet = workbook.GetWorksheets().Get(0);
//вставить первое изображение
int imgIndex1 = worksheet.GetPictures().Add(1, 1, u"example1.png");
//Получить вставленный объект изображения
Picture pic1 = worksheet.GetPictures().Get(imgIndex1);
//вставить второе изображение
int imgIndex2 = worksheet.GetPictures().Add(1, 9, u"example2.jpeg");
//Получить вставленный объект изображения
Picture pic2 = worksheet.GetPictures().Get(imgIndex2);
//Назначить байтовые данные первого изображения второму изображению
pic2.SetData(pic1.GetData());
//Сохранить файл Excel.
workbook.Save(u"result.xlsx");
Aspose::Cells::Cleanup();
```

## See Also

* Class [Vector](../../../aspose.cells/vector/)
* Class [Picture](../)
* Namespace [Aspose::Cells::Drawing](../../)
* Library [Aspose.Cells for C++](../../../)
