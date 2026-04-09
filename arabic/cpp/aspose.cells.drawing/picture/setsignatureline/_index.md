---
title: Aspose::Cells::Drawing::Picture::SetSignatureLine method
linktitle: SetSignatureLine
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Drawing::Picture::SetSignatureLine method. Gets and sets the signature line in C++.'
type: docs
weight: 3500
url: /ar/cpp/aspose.cells.drawing/picture/setsignatureline/
---
## Picture::SetSignatureLine method


Gets and sets the signature line.

```cpp
void Aspose::Cells::Drawing::Picture::SetSignatureLine(const SignatureLine &value)
```


## Examples


```cpp
Aspose::Cells::Startup();
//إنشاء كائن Workbook
Workbook workbook;
Worksheet worksheet = workbook.GetWorksheets().Get(0);
//إضافة صورة في موقع الخلية التي مؤشرات الصف والعمود لها 1 في ورقة العمل. إنها الخلية "B2"
int imgIndex = worksheet.GetPictures().Add(1, 1, u"example.jpeg");
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

* Class [Vector](../../../aspose.cells/vector/)
* Class [SignatureLine](../../signatureline/)
* Class [Picture](../)
* Namespace [Aspose::Cells::Drawing](../../)
* Library [Aspose.Cells for C++](../../../)
