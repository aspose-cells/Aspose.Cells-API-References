---
title: Aspose::Cells::XmlMapCollection class
linktitle: XmlMapCollection
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::XmlMapCollection class. A collection of XmlMap objects that represent XmlMap information in C++.'
type: docs
weight: 17400
url: /zh/cpp/aspose.cells/xmlmapcollection/
---
## XmlMapCollection class


A collection of [XmlMap](../xmlmap/) objects that represent [XmlMap](../xmlmap/) information.

```cpp
class XmlMapCollection
```

## Methods

| Method | Description |
| --- | --- |
| [Add(const U16String\& url)](./add/) | Add a [XmlMap](../xmlmap/) by the url/path of a xml/xsd file. |
| [Add(const char16_t* url)](./add/) | Add a [XmlMap](../xmlmap/) by the url/path of a xml/xsd file. |
| [Clear()](./clear/) | Removes all XmlMaps. |
| [Get(int32_t index)](./get/) | Gets the xml map by the specific index. |
| [GetCount()](./getcount/) |  |
| [IsNull()](./isnull/) const | Checks whether the implementation object is nullptr. |
| explicit [operator bool()](./operator_bool/) const | operator bool() |
| [operator=(const XmlMapCollection\& src)](./operator_asm/) | operator= |
| [XmlMapCollection(XmlMapCollection_Impl* impl)](./xmlmapcollection/) | Constructs from an implementation object. |
| [XmlMapCollection(const XmlMapCollection\& src)](./xmlmapcollection/) | Copy constructor. |
| [~XmlMapCollection()](./~xmlmapcollection/) | Destructor. |
## Fields

| Field | Description |
| --- | --- |
| [_impl](./_impl/) | The implementation object. |

## Examples


```cpp
Aspose::Cells::Startup();
//以下代码通过 XSD 文件和 XML 文件添加了两个 XmlMap。
Workbook wb;

XmlMapCollection xmlMapCollection = wb.GetWorksheets().GetXmlMaps();

//通过 XSD 文件添加一个 XmlMap。
xmlMapCollection.Add(u"schema.xsd");

//通过 XML 文件添加一个 XmlMap。
xmlMapCollection.Add(u"xml.xml");

wb.Save(u"twoXmlMaps.xlsx");
Aspose::Cells::Cleanup();
```

## See Also

* Namespace [Aspose::Cells](../)
* Library [Aspose.Cells for C++](../../)
