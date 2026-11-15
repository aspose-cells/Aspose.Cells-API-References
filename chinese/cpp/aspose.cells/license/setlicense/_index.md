---
title: Aspose::Cells::License::SetLicense method
linktitle: SetLicense
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::License::SetLicense method. Licenses the component in C++.'
type: docs
weight: 600
url: /zh/cpp/aspose.cells/license/setlicense/
---
## License::SetLicense(const U16String\&) method


Licenses the component.

```cpp
void Aspose::Cells::License::SetLicense(const U16String &licenseName)
```


| Parameter | Type | Description |
| --- | --- | --- |
| licenseName | const U16String\& | The license file path. |

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
//在此示例中，将尝试查找名为 MyLicense.lic 的许可证文件
//在包含的文件夹中
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

## See Also

* Class [Vector](../../vector/)
* Class [License](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
