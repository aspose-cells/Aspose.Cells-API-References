##Aspose::Cells::Cells::LinkToXmlMap method
'Aspose::Cells::Cells::LinkToXmlMap method. Link to a xml map in C++.'
## Cells::LinkToXmlMap(const U16String\&, int32_t, int32_t, const U16String\&) method
Link to a xml map.
```cpp
void Aspose::Cells::Cells::LinkToXmlMap(const U16String &mapName, int32_t row, int32_t column, const U16String &path)
```
| Parameter | Type | Description |
| --- | --- | --- |
| mapName | const U16String\& | name of xml map |
| row | int32_t | row of the destination cell |
| column | int32_t | column of the destination cell |
| path | const U16String\& | path of xml element in xml map |
## Remarks
e.g. A xml map element structure: -RootElement |-Attribute1 |-SubElement |-Attribute2 |-Attribute3 To link "Attribute1", path is "/RootElement/Attribute1" To link "Attribute2", path is "/RootElement/SubElement/Attribute2" To link whole "SubElement", path is "/RootElement/SubElement"
## See Also
* Class [Vector](../../vector/)
* Class [U16String](../../u16string/)
* Class [Cells](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
## Cells::LinkToXmlMap(const char16_t*, int32_t, int32_t, const char16_t*) method
Link to a xml map.
```cpp
void Aspose::Cells::Cells::LinkToXmlMap(const char16_t *mapName, int32_t row, int32_t column, const char16_t *path)
```
| Parameter | Type | Description |
| --- | --- | --- |
| mapName | const char16_t* | name of xml map |
| row | int32_t | row of the destination cell |
| column | int32_t | column of the destination cell |
| path | const char16_t* | path of xml element in xml map |
## Remarks
e.g. A xml map element structure: -RootElement |-Attribute1 |-SubElement |-Attribute2 |-Attribute3 To link "Attribute1", path is "/RootElement/Attribute1" To link "Attribute2", path is "/RootElement/SubElement/Attribute2" To link whole "SubElement", path is "/RootElement/SubElement"
## See Also
* Class [Vector](../../vector/)
* Class [Cells](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
