---
title: Aspose::Cells::Drawing::Picture::GetSignatureLine method
linktitle: GetSignatureLine
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Drawing::Picture::GetSignatureLine method. Gets and sets the signature line in C++.'
type: docs
weight: 3600
url: /ru/cpp/aspose.cells.drawing/picture/getsignatureline/
---
## Picture::GetSignatureLine method


Gets and sets the signature line.

```cpp
SignatureLine Aspose::Cells::Drawing::Picture::GetSignatureLine()
```


## Examples


```cpp
Aspose::Cells::Startup();
//Создание экземпляра объекта Workbook
Workbook workbook;
Worksheet worksheet = workbook.GetWorksheets().Get(0);
//Добавление изображения в ячейку, у которой индексы строки и столбца равны 1 в листе. Это ячейка "B2".
int imgIndex = worksheet.GetPictures().Add(1, 1, Vector<uint8_t>(0));
//Получить вставленный объект изображения
Picture pic = worksheet.GetPictures().Get(imgIndex);
// Создать объект строки подписи
SignatureLine s;
s.SetSigner(u"Simon Zhao");
s.SetTitle(u"Development Lead");
s.SetEmail(u"Simon.Zhao@aspose.com");
// Назначить объект подписи изображению.
pic.SetSignatureLine(s);

SignatureLine s2 = pic.GetSignatureLine();
if (s2.GetSigner() == s.GetSigner())
{
    //делайте, что хотите
}
//Сохранить файл Excel.
workbook.Save(u"result.xlsx");
Aspose::Cells::Cleanup();
```

## See Also

* Class [SignatureLine](../../signatureline/)
* Class [Picture](../)
* Namespace [Aspose::Cells::Drawing](../../)
* Library [Aspose.Cells for C++](../../../)
