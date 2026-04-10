---
title: Aspose::Cells::Drawing::Picture::Copy method
linktitle: Copy
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Drawing::Picture::Copy method. Copy the picture in C++.'
type: docs
weight: 600
url: /sv/cpp/aspose.cells.drawing/picture/copy/
---
## Picture::Copy method


Copy the picture.

```cpp
void Aspose::Cells::Drawing::Picture::Copy(const Aspose::Cells::Drawing::Picture &source, const CopyOptions &options)
```


| Parameter | Type | Description |
| --- | --- | --- |
| source | const Aspose::Cells::Drawing::Picture\& | The source picture. |
| options | const CopyOptions\& | The copy options. |


## Examples


```cpp
Aspose::Cells::Startup();
//Instansierar ett Workbook‑objekt
Workbook workbook;
Worksheet worksheet = workbook.GetWorksheets().Get(0);
//infoga första bilden
int imgIndex1 = worksheet.GetPictures().Add(1, 1, u"1.png");
//Hämta det infogade bildobjektet
Picture pic1 = worksheet.GetPictures().Get(imgIndex1);
//infoga andra bilden
int imgIndex2 = worksheet.GetPictures().Add(1, 9, u"2.jpeg");
//Hämta det infogade bildobjektet
Picture pic2 = worksheet.GetPictures().Get(imgIndex2);
//Kopiera bild 1 till bild 2. Du får två bild 1-objekt som är överlagrade på varandra.
CopyOptions opt;
pic2.Copy(pic1, opt);
//Spara Excel-filen.
workbook.Save(u"result.xlsx");
Aspose::Cells::Cleanup();
```

## See Also

* Class [Vector](../../../aspose.cells/vector/)
* Class [Picture](../)
* Class [CopyOptions](../../../aspose.cells/copyoptions/)
* Class [Picture](../)
* Namespace [Aspose::Cells::Drawing](../../)
* Library [Aspose.Cells for C++](../../../)
