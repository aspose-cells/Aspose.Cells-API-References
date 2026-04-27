---
title: Aspose::Cells::Drawing::Picture::Copy method
linktitle: Copy
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Drawing::Picture::Copy method. Copy the picture in C++.'
type: docs
weight: 600
url: /ar/cpp/aspose.cells.drawing/picture/copy/
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
//إنشاء كائن Workbook
Workbook workbook;
Worksheet worksheet = workbook.GetWorksheets().Get(0);
//إدراج الصورة الأولى
int imgIndex1 = worksheet.GetPictures().Add(1, 1, u"1.png");
//احصل على كائن الصورة المُدرَج
Picture pic1 = worksheet.GetPictures().Get(imgIndex1);
//إدراج الصورة الثانية
int imgIndex2 = worksheet.GetPictures().Add(1, 9, u"2.jpeg");
//احصل على كائن الصورة المُدرَج
Picture pic2 = worksheet.GetPictures().Get(imgIndex2);
//نسخ الصورة 1 إلى الصورة 2. ستحصل على كائنين من الصورة 1 مدمجين فوق بعضهما البعض.
CopyOptions opt;
pic2.Copy(pic1, opt);
//Save the excel file.
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
