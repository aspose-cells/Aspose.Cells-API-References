---
title: Aspose::Cells::FileFormatUtil::DetectFileFormat method
linktitle: DetectFileFormat
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::FileFormatUtil::DetectFileFormat method. Detects and returns the information about a format of an excel stored in a stream in C++.'
type: docs
weight: 100
url: /cpp/aspose.cells/fileformatutil/detectfileformat/
---
## FileFormatUtil::DetectFileFormat(const Vector \<uint8_t\>\&) method


Detects and returns the information about a format of an excel stored in a stream.

```cpp
static FileFormatInfo Aspose::Cells::FileFormatUtil::DetectFileFormat(const Vector<uint8_t> &stream)
```


| Parameter | Type | Description |
| --- | --- | --- |
| stream | const Vector \<uint8_t\>\& |  |

## ReturnValue

A [FileFormatInfo](../../fileformatinfo/) object that contains the detected information.

## See Also

* Class [FileFormatInfo](../../fileformatinfo/)
* Class [Vector](../../vector/)
* Class [FileFormatUtil](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
## FileFormatUtil::DetectFileFormat(const Vector \<uint8_t\>\&, const U16String\&) method


Detects and returns the information about a format of an excel stored in a stream.

```cpp
static FileFormatInfo Aspose::Cells::FileFormatUtil::DetectFileFormat(const Vector<uint8_t> &stream, const U16String &password)
```


| Parameter | Type | Description |
| --- | --- | --- |
| stream | const Vector \<uint8_t\>\& |  |
| password | const U16String\& | The password for encrypted ooxml files. |

## ReturnValue

A [FileFormatInfo](../../fileformatinfo/) object that contains the detected information.

## See Also

* Class [FileFormatInfo](../../fileformatinfo/)
* Class [Vector](../../vector/)
* Class [U16String](../../u16string/)
* Class [FileFormatUtil](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
## FileFormatUtil::DetectFileFormat(const Vector \<uint8_t\>\&, const char16_t*) method


Detects and returns the information about a format of an excel stored in a stream.

```cpp
static FileFormatInfo Aspose::Cells::FileFormatUtil::DetectFileFormat(const Vector<uint8_t> &stream, const char16_t *password)
```


| Parameter | Type | Description |
| --- | --- | --- |
| stream | const Vector \<uint8_t\>\& |  |
| password | const char16_t* | The password for encrypted ooxml files. |

## ReturnValue

A [FileFormatInfo](../../fileformatinfo/) object that contains the detected information.

## See Also

* Class [FileFormatInfo](../../fileformatinfo/)
* Class [Vector](../../vector/)
* Class [FileFormatUtil](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
## FileFormatUtil::DetectFileFormat(const U16String\&) method


Detects and returns the information about a format of an excel stored in a file.

```cpp
static FileFormatInfo Aspose::Cells::FileFormatUtil::DetectFileFormat(const U16String &filePath)
```


| Parameter | Type | Description |
| --- | --- | --- |
| filePath | const U16String\& | The file path. |

## ReturnValue

A [FileFormatInfo](../../fileformatinfo/) object that contains the detected information.
## Remarks



Only supports checking some files with magic signature. If there is no magic signature, we can not precisely detect the file format. 
## See Also

* Class [FileFormatInfo](../../fileformatinfo/)
* Class [Vector](../../vector/)
* Class [U16String](../../u16string/)
* Class [FileFormatUtil](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
## FileFormatUtil::DetectFileFormat(const char16_t*) method


Detects and returns the information about a format of an excel stored in a file.

```cpp
static FileFormatInfo Aspose::Cells::FileFormatUtil::DetectFileFormat(const char16_t *filePath)
```


| Parameter | Type | Description |
| --- | --- | --- |
| filePath | const char16_t* | The file path. |

## ReturnValue

A [FileFormatInfo](../../fileformatinfo/) object that contains the detected information.
## Remarks



Only supports checking some files with magic signature. If there is no magic signature, we can not precisely detect the file format. 
## See Also

* Class [FileFormatInfo](../../fileformatinfo/)
* Class [Vector](../../vector/)
* Class [FileFormatUtil](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
## FileFormatUtil::DetectFileFormat(const U16String\&, const U16String\&) method


Detects and returns the information about a format of an excel stored in a file.

```cpp
static FileFormatInfo Aspose::Cells::FileFormatUtil::DetectFileFormat(const U16String &filePath, const U16String &password)
```


| Parameter | Type | Description |
| --- | --- | --- |
| filePath | const U16String\& | The file path. |
| password | const U16String\& | The password for encrypted ooxml files. |

## ReturnValue

A [FileFormatInfo](../../fileformatinfo/) object that contains the detected information.
## Remarks



Only supports checking some files with magic signature. If there is no magic signature, we can not precisely detect the file format. 
## See Also

* Class [FileFormatInfo](../../fileformatinfo/)
* Class [Vector](../../vector/)
* Class [U16String](../../u16string/)
* Class [FileFormatUtil](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
## FileFormatUtil::DetectFileFormat(const char16_t*, const char16_t*) method


Detects and returns the information about a format of an excel stored in a file.

```cpp
static FileFormatInfo Aspose::Cells::FileFormatUtil::DetectFileFormat(const char16_t *filePath, const char16_t *password)
```


| Parameter | Type | Description |
| --- | --- | --- |
| filePath | const char16_t* | The file path. |
| password | const char16_t* | The password for encrypted ooxml files. |

## ReturnValue

A [FileFormatInfo](../../fileformatinfo/) object that contains the detected information.
## Remarks



Only supports checking some files with magic signature. If there is no magic signature, we can not precisely detect the file format. 
## See Also

* Class [FileFormatInfo](../../fileformatinfo/)
* Class [Vector](../../vector/)
* Class [FileFormatUtil](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
