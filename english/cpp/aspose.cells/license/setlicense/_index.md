---
title: Aspose::Cells::License::SetLicense method
linktitle: SetLicense
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::License::SetLicense method. Licenses the component in C++.'
type: docs
weight: 600
url: /cpp/aspose.cells/license/setlicense/
---
## License::SetLicense(const U16String\&) method


Licenses the component.

```cpp
void Aspose::Cells::License::SetLicense(const U16String &licenseName)
```


| Parameter | Type | Description |
| --- | --- | --- |
| licenseName | const U16String\& | The license file path. |
## Examples

```cpp
Aspose::Cells::Startup();
//In this example, an attempt will be made to find a license file named MyLicense.lic
//in the folder that contains
U16String val = u"License.lic";//your license file
License license;
license.SetLicense(val);//your license file
Aspose::Cells::Cleanup();
```

## See Also

* Class [Vector](../../vector/)
* Class [U16String](../../u16string/)
* Class [License](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
## License::SetLicense(const char16_t*) method


Licenses the component.

```cpp
void Aspose::Cells::License::SetLicense(const char16_t *licenseName)
```


| Parameter | Type | Description |
| --- | --- | --- |
| licenseName | const char16_t* | The license file path. |


## Examples


```cpp
Aspose::Cells::Startup();
//In this example, an attempt will be made to find a license file named MyLicense.lic
//in the folder that contains
License license;
license.SetLicense(u"License.lic");//your license file
Aspose::Cells::Cleanup();
```

## See Also

* Class [Vector](../../vector/)
* Class [License](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
## License::SetLicense(const Vector \<uint8_t\>\&) method


Licenses the component.

```cpp
void Aspose::Cells::License::SetLicense(const Vector<uint8_t> &stream)
```


| Parameter | Type | Description |
| --- | --- | --- |
| stream | const Vector \<uint8_t\>\& | A Vector<uint8_t> that contains the license. |

## Examples


```cpp
Aspose::Cells::Startup();
//In this example, an attempt will be made to find a license file named MyLicense.lic
//in the folder that contains
Vector<uint8_t> licData = { 0 };//Gets data from license file into 'licData'(Note: You need to read the data into this variable.).
License license;
license.SetLicense(licData);

Aspose::Cells::Cleanup();
```
## See Also

* Class [Vector](../../vector/)
* Class [License](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
