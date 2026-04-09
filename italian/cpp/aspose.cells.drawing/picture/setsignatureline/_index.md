---
title: Aspose::Cells::Drawing::Picture::SetSignatureLine method
linktitle: SetSignatureLine
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Drawing::Picture::SetSignatureLine method. Gets and sets the signature line in C++.'
type: docs
weight: 3500
url: /it/cpp/aspose.cells.drawing/picture/setsignatureline/
---
## Picture::SetSignatureLine method


Gets and sets the signature line.

```cpp
void Aspose::Cells::Drawing::Picture::SetSignatureLine(const SignatureLine &value)
```


## Examples


```cpp
Aspose::Cells::Startup();
//Istanziare un oggetto Workbook
Workbook workbook;
Worksheet worksheet = workbook.GetWorksheets().Get(0);
//Adding a picture at the location of a cell whose row and column indices are 1 in the worksheet. It is "B2" cell
int imgIndex = worksheet.GetPictures().Add(1, 1, u"example.jpeg");
//Get the inserted picture object
Picture pic = worksheet.GetPictures().Get(imgIndex);
// Crea oggetto linea di firma
SignatureLine s;
s.SetSigner(u"Simon Zhao");
s.SetTitle(u"Development Lead");
s.SetEmail(u"Simon.Zhao@aspose.com");
// Assign the signature line object to Picture.
pic.SetSignatureLine(s);

SignatureLine s2 = pic.GetSignatureLine();
if (s2.GetSigner() == s.GetSigner())
{
    //fai quello che vuoi
}
//Salva il file Excel.
workbook.Save(u"result.xlsx");
Aspose::Cells::Cleanup();
```

## See Also

* Class [Vector](../../../aspose.cells/vector/)
* Class [SignatureLine](../../signatureline/)
* Class [Picture](../)
* Namespace [Aspose::Cells::Drawing](../../)
* Library [Aspose.Cells for C++](../../../)
