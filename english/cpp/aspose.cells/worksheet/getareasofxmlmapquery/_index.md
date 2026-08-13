---
title: Aspose::Cells::Worksheet::GetAreasOfXmlMapQuery method
linktitle: GetAreasOfXmlMapQuery
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Worksheet::GetAreasOfXmlMapQuery method. Query cell areas that mapped/linked to the specific path of xml map in C++.'
type: docs
weight: 12700
url: /cpp/aspose.cells/worksheet/getareasofxmlmapquery/
---
## Worksheet::GetAreasOfXmlMapQuery(const U16String\&, const XmlMap\&) method


Query cell areas that mapped/linked to the specific path of xml map.

```cpp
Vector<CellArea> Aspose::Cells::Worksheet::GetAreasOfXmlMapQuery(const U16String &path, const XmlMap &xmlMap)
```


| Parameter | Type | Description |
| --- | --- | --- |
| path | const U16String\& | xml element path |
| xmlMap | const XmlMap\& | Specify an xml map if you want to query for the specific path within a specific map |

## ReturnValue

[CellArea](../../cellarea/) list that mapped/linked to the specific path of xml map, an empty list is returned if nothing is mapped/linked.
## Remarks



e.g. A xml map element structure: -RootElement |-Attribute1 |-SubElement |-Attribute2 |-Attribute3 To query "Attribute1", path is "/RootElement/@Attribute1" To query "Attribute2", path is "/RootElement/SubElement/@Attribute2" To query whole "SubElement", path is "/RootElement/SubElement" 
## See Also

* Class [Vector](../../vector/)
* Class [CellArea](../../cellarea/)
* Class [U16String](../../u16string/)
* Class [XmlMap](../../xmlmap/)
* Class [Worksheet](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
## Worksheet::GetAreasOfXmlMapQuery(const char16_t*, const XmlMap\&) method


Query cell areas that mapped/linked to the specific path of xml map.

```cpp
Vector<CellArea> Aspose::Cells::Worksheet::GetAreasOfXmlMapQuery(const char16_t *path, const XmlMap &xmlMap)
```


| Parameter | Type | Description |
| --- | --- | --- |
| path | const char16_t* | xml element path |
| xmlMap | const XmlMap\& | Specify an xml map if you want to query for the specific path within a specific map |

## ReturnValue

[CellArea](../../cellarea/) list that mapped/linked to the specific path of xml map, an empty list is returned if nothing is mapped/linked.
## Remarks



e.g. A xml map element structure: -RootElement |-Attribute1 |-SubElement |-Attribute2 |-Attribute3 To query "Attribute1", path is "/RootElement/@Attribute1" To query "Attribute2", path is "/RootElement/SubElement/@Attribute2" To query whole "SubElement", path is "/RootElement/SubElement" 
## See Also

* Class [Vector](../../vector/)
* Class [CellArea](../../cellarea/)
* Class [XmlMap](../../xmlmap/)
* Class [Worksheet](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
