---
title: Aspose::Cells::Drawing::Picture::GetSignatureLine method
linktitle: GetSignatureLine
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Drawing::Picture::GetSignatureLine method. Gets and sets the signature line in C++.'
type: docs
weight: 3400
url: /ar/cpp/aspose.cells.drawing/picture/getsignatureline/
---
## Picture::GetSignatureLine method


Gets and sets the signature line.

```cpp
SignatureLine Aspose::Cells::Drawing::Picture::GetSignatureLine()
```


## Examples


```cpp
Aspose::Cells::Startup();
//إنشاء كائن Workbook
Workbook workbook;
Worksheet worksheet = workbook.GetWorksheets().Get(0);
//إضافة صورة في موقع الخلية التي مؤشرات الصف والعمود لها 1 في ورقة العمل. إنها الخلية "B2"
int imgIndex = worksheet.GetPictures().Add(1, 1, Vector<uint8_t>(0));
//احصل على كائن الصورة المُدرَج
Picture pic = worksheet.GetPictures().Get(imgIndex);
// Create signature line object
SignatureLine s;
s.SetSigner(u"Simon Zhao");
s.SetTitle(u"Development Lead");
s.SetEmail(u"Simon.Zhao@aspose.com");
// تعيين كائن خط التوقيع إلى الصورة.
pic.SetSignatureLine(s);

SignatureLine s2 = pic.GetSignatureLine();
if (s2.GetSigner() == s.GetSigner())
{
    //افعل ما تريد
}
//Save the excel file.
workbook.Save(u"result.xlsx");
Aspose::Cells::Cleanup();
```

## See Also

* Class [SignatureLine](../../signatureline/)
* Class [Picture](../)
* Namespace [Aspose::Cells::Drawing](../../)
* Library [Aspose.Cells for C++](../../../)
