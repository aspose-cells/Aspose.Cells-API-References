---
title: Aspose::Cells::Drawing::Picture::SetSignatureLine method
linktitle: SetSignatureLine
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Drawing::Picture::SetSignatureLine method. Gets and sets the signature line in C++.'
type: docs
weight: 3500
url: /zh/cpp/aspose.cells.drawing/picture/setsignatureline/
---
## Picture::SetSignatureLine method


Gets and sets the signature line.

```cpp
void Aspose::Cells::Drawing::Picture::SetSignatureLine(const SignatureLine &value)
```


## Examples


```cpp
Aspose::Cells::Startup();
//实例化 Workbook 对象
Workbook workbook;
Worksheet worksheet = workbook.GetWorksheets().Get(0);
//在工作表中行列索引为 1 的单元格位置添加图片。该单元格为 "B2"。
int imgIndex = worksheet.GetPictures().Add(1, 1, u"example.jpeg");
//获取插入的图片对象
Picture pic = worksheet.GetPictures().Get(imgIndex);
// 创建签名行对象
SignatureLine s;
s.SetSigner(u"Simon Zhao");
s.SetTitle(u"Development Lead");
s.SetEmail(u"Simon.Zhao@aspose.com");
// 将签名线对象分配给 Picture。
pic.SetSignatureLine(s);

SignatureLine s2 = pic.GetSignatureLine();
if (s2.GetSigner() == s.GetSigner())
{
    //随意操作
}
//保存 Excel 文件。
workbook.Save(u"result.xlsx");
Aspose::Cells::Cleanup();
```

## See Also

* Class [Vector](../../../aspose.cells/vector/)
* Class [SignatureLine](../../signatureline/)
* Class [Picture](../)
* Namespace [Aspose::Cells::Drawing](../../)
* Library [Aspose.Cells for C++](../../../)
