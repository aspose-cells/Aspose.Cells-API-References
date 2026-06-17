---
title: Aspose::Cells::DigitalSignatures::DigitalSignature::DigitalSignature constructor
linktitle: DigitalSignature
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::DigitalSignatures::DigitalSignature::DigitalSignature constructor. Constructor of DigitalSignature in C++.'
type: docs
weight: 100
url: /zh/cpp/aspose.cells.digitalsignatures/digitalsignature/digitalsignature/
---
## DigitalSignature::DigitalSignature(const Vector \<uint8_t\>\&, const U16String\&, const U16String\&, const Date\&) constructor


Constructor of [DigitalSignature](../).

```cpp
Aspose::Cells::DigitalSignatures::DigitalSignature::DigitalSignature(const Vector<uint8_t> &rawData, const U16String &password, const U16String &comments, const Date &signTime)
```


| Parameter | Type | Description |
| --- | --- | --- |
| rawData | const Vector \<uint8_t\>\& | A byte array containing data from an X.509 certificate. |
| password | const U16String\& | The password required to access the X.509 certificate data. |
| comments | const U16String\& | The purpose to signature. |
| signTime | const Date\& | The utc time when the document was signed. |


## Examples


```cpp
Aspose::Cells::Startup();
//以下示例展示了如何创建数字签名。

//签名集合包含一个或多个用于签名的签名
DigitalSignatureCollection dsc;

//包含 X.509 证书数据的字节数组。
Vector<uint8_t> data{ 0 };//Note: You need to read the data into this variable.
U16String pwd = "123456";//The password required to access the X.509 certificate data.
U16String comment = "test for sign";//The purpose to signature.
Date dtUtc{ 2023,10,10,5,30,12 };//The utc time when the document was signed.
DigitalSignature ds(data, pwd, comment, dtUtc);

dsc.Add(ds);
Workbook wb;
//将所有签名设置到工作簿
wb.SetDigitalSignature(dsc);
wb.Save(u"newfile.xlsx");
Aspose::Cells::Cleanup();
```

## See Also

* Class [Vector](../../../aspose.cells/vector/)
* Class [U16String](../../../aspose.cells/u16string/)
* Class [DigitalSignature](../)
* Namespace [Aspose::Cells::DigitalSignatures](../../)
* Library [Aspose.Cells for C++](../../../)
## DigitalSignature::DigitalSignature(const Vector \<uint8_t\>\&, const char16_t*, const char16_t*, const Date\&) constructor


Constructor of [DigitalSignature](../).

```cpp
Aspose::Cells::DigitalSignatures::DigitalSignature::DigitalSignature(const Vector<uint8_t> &rawData, const char16_t *password, const char16_t *comments, const Date &signTime)
```


| Parameter | Type | Description |
| --- | --- | --- |
| rawData | const Vector \<uint8_t\>\& | A byte array containing data from an X.509 certificate. |
| password | const char16_t* | The password required to access the X.509 certificate data. |
| comments | const char16_t* | The purpose to signature. |
| signTime | const Date\& | The utc time when the document was signed. |


## Examples


```cpp
Aspose::Cells::Startup();
//以下示例展示了如何创建数字签名。

//签名集合包含一个或多个用于签名的签名
DigitalSignatureCollection dsc;

//包含 X.509 证书数据的字节数组。
Vector<uint8_t> data{0};//Note: You need to read the data into this variable.
Date dtUtc{2023,10,10,5,30,12};//The utc time when the document was signed.
DigitalSignature ds(data,"123456", "test for sign", dtUtc); //123456 is password of cert

dsc.Add(ds);
Workbook wb;
//将所有签名设置到工作簿
wb.SetDigitalSignature(dsc);
wb.Save(u"newfile.xlsx");


Aspose::Cells::Cleanup();
```

## See Also

* Class [Vector](../../../aspose.cells/vector/)
* Class [DigitalSignature](../)
* Namespace [Aspose::Cells::DigitalSignatures](../../)
* Library [Aspose.Cells for C++](../../../)
## DigitalSignature::DigitalSignature(const U16String\&, const U16String\&, const U16String\&, const Date\&) constructor


Constructor of [DigitalSignature](../).

```cpp
Aspose::Cells::DigitalSignatures::DigitalSignature::DigitalSignature(const U16String &fileName, const U16String &password, const U16String &comments, const Date &signTime)
```


| Parameter | Type | Description |
| --- | --- | --- |
| fileName | const U16String\& | The name of a certificate file. |
| password | const U16String\& | The password required to access the X.509 certificate data. |
| comments | const U16String\& | The purpose to signature. |
| signTime | const Date\& | The utc time when the document was signed. |

## See Also

* Class [Vector](../../../aspose.cells/vector/)
* Class [U16String](../../../aspose.cells/u16string/)
* Class [DigitalSignature](../)
* Namespace [Aspose::Cells::DigitalSignatures](../../)
* Library [Aspose.Cells for C++](../../../)
## DigitalSignature::DigitalSignature(const char16_t*, const char16_t*, const char16_t*, const Date\&) constructor


Constructor of [DigitalSignature](../).

```cpp
Aspose::Cells::DigitalSignatures::DigitalSignature::DigitalSignature(const char16_t *fileName, const char16_t *password, const char16_t *comments, const Date &signTime)
```


| Parameter | Type | Description |
| --- | --- | --- |
| fileName | const char16_t* | The name of a certificate file. |
| password | const char16_t* | The password required to access the X.509 certificate data. |
| comments | const char16_t* | The purpose to signature. |
| signTime | const Date\& | The utc time when the document was signed. |

## See Also

* Class [Vector](../../../aspose.cells/vector/)
* Class [DigitalSignature](../)
* Namespace [Aspose::Cells::DigitalSignatures](../../)
* Library [Aspose.Cells for C++](../../../)
## DigitalSignature::DigitalSignature(DigitalSignature_Impl*) constructor


Constructs from an implementation object.

```cpp
Aspose::Cells::DigitalSignatures::DigitalSignature::DigitalSignature(DigitalSignature_Impl *impl)
```

## See Also

* Class [Vector](../../../aspose.cells/vector/)
* Class [DigitalSignature](../)
* Namespace [Aspose::Cells::DigitalSignatures](../../)
* Library [Aspose.Cells for C++](../../../)
## DigitalSignature::DigitalSignature(const DigitalSignature\&) constructor


Copy constructor.

```cpp
Aspose::Cells::DigitalSignatures::DigitalSignature::DigitalSignature(const DigitalSignature &src)
```

## See Also

* Class [Vector](../../../aspose.cells/vector/)
* Class [DigitalSignature](../)
* Class [DigitalSignature](../)
* Namespace [Aspose::Cells::DigitalSignatures](../../)
* Library [Aspose.Cells for C++](../../../)
