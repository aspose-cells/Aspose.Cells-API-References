---
title: Aspose::Cells::Drawing::Picture::GetOriginalHeightInch method
linktitle: GetOriginalHeightInch
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Drawing::Picture::GetOriginalHeightInch method. Gets the original height of picture, in unit of inches in C++.'
type: docs
weight: 3100
url: /cpp/aspose.cells.drawing/picture/getoriginalheightinch/
---
## Picture::GetOriginalHeightInch method


Gets the original height of picture, in unit of inches.

```cpp
double Aspose::Cells::Drawing::Picture::GetOriginalHeightInch()
```


## Examples


```cpp
Aspose::Cells::Startup();
//Instantiating a Workbook object
Workbook workbook;
Worksheet worksheet = workbook.GetWorksheets().Get(0);
//Adding a picture at the location of a cell whose row and column indices are 1 in the worksheet. It is "B2" cell
int imgIndex = worksheet.GetPictures().Add(1, 1, u"example.jpeg");
//Get the inserted picture object
Picture pic = worksheet.GetPictures().Get(imgIndex);
//Gets the original height of the picture.
double picHeightInch = pic.GetOriginalHeightInch();
//Save the excel file.
workbook.Save(u"result.xlsx");
Aspose::Cells::Cleanup();
```

## See Also

* Class [Vector](../../../aspose.cells/vector/)
* Class [Picture](../)
* Namespace [Aspose::Cells::Drawing](../../)
* Library [Aspose.Cells for C++](../../../)
