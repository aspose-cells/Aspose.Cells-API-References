---
title: "FileFormatUtil 类"
linktitle: "FileFormatUtil"
second_title: "Aspose.Cells for Go via C++ API 参考"
description: "FileFormatUtil 类。封装了在 Go 中表示 fileformatutil 的对象。"
type: docs
weight: 200
url: /zh/go-cpp/fileformatutil/
---

## FileFormatUtil class

提供将文件格式枚举转换为字符串或文件扩展名以及反向转换的实用方法。

```go

type FileFormatUtil struct  {
	ptr unsafe.Pointer
}

```
## 构造函数

| 方法 | 描述 |
| --- | --- |

## 方法

| 方法 | 描述 |
| --- | --- |
| [FileFormatUtil_DetectFileFormat_Stream](./fileformatutil_detectfileformat_stream/) | 检测并返回存储在流中的 Excel 格式信息。 |
| [FileFormatUtil_DetectFileFormat_Stream_String](./fileformatutil_detectfileformat_stream_string/) | 检测并返回存储在流中的 Excel 格式信息。 |
| [FileFormatUtil_VerifyPassword](./fileformatutil_verifypassword/) | 检测并返回存储在流中的 Excel 格式信息。 |
| [FileFormatUtil_DetectFileFormat_String](./fileformatutil_detectfileformat_string/) | 检测并返回存储在文件中的 Excel 格式信息。 |
| [FileFormatUtil_DetectFileFormat_String_String](./fileformatutil_detectfileformat_string_string/) | 检测并返回存储在文件中的 Excel 格式信息。 |
| [FileFormatUtil_FileFormatToSaveFormat](./fileformatutil_fileformattosaveformat/) | 将文件格式转换为保存格式。 |
| [FileFormatUtil_ExtensionToSaveFormat](./fileformatutil_extensiontosaveformat/) | 将文件名扩展名转换为 SaveFormat 值。 |
| [FileFormatUtil_IsTemplateFormat](./fileformatutil_istemplateformat/) | 如果扩展名是 .xlt、.xltX、.xltm、.ots，则返回 true。 |
| [FileFormatUtil_LoadFormatToExtension](./fileformatutil_loadformattoextension/) | 将加载格式枚举值转换为文件扩展名。 |
| [FileFormatUtil_LoadFormatToSaveFormat](./fileformatutil_loadformattosaveformat/) | 如果可能，将 LoadFormat 值转换为 SaveFormat 值。 |
| [FileFormatUtil_SaveFormatToExtension](./fileformatutil_saveformattoextension/) | 将保存格式枚举值转换为文件扩展名。 |
| [FileFormatUtil_SaveFormatToLoadFormat](./fileformatutil_saveformattoloadformat/) | 如果可能，将 SaveFormat 值转换为 LoadFormat 值。 |
