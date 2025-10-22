##Aspose::Cells::Workbook::ExportXml method
'Aspose::Cells::Workbook::ExportXml method. Export XML data linked by the specified XML map in C++.'
## Workbook::ExportXml(const U16String\&, const U16String\&) method
Export XML data linked by the specified XML map.
```cpp
void Aspose::Cells::Workbook::ExportXml(const U16String &mapName, const U16String &path)
```
| Parameter | Type | Description |
| --- | --- | --- |
| mapName | const U16String\& | name of the XML map that need to be exported |
| path | const U16String\& | the export path |
## Examples
```cpp
Aspose::Cells::Startup();
//The following code exported the data linked by the first XmlMap.
Workbook wb(u"Book1.xlsx");
//Make sure that the source xlsx file contains a XmlMap.
XmlMap xmlMap = wb.GetWorksheets().GetXmlMaps().Get(0);
U16String val = u"output.xml";
wb.ExportXml(xmlMap.GetName(), val);
Aspose::Cells::Cleanup();
```
## See Also
* Class [Vector](../../vector/)
* Class [U16String](../../u16string/)
* Class [Workbook](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
## Workbook::ExportXml(const char16_t*, const char16_t*) method
Export XML data linked by the specified XML map.
```cpp
void Aspose::Cells::Workbook::ExportXml(const char16_t *mapName, const char16_t *path)
```
| Parameter | Type | Description |
| --- | --- | --- |
| mapName | const char16_t* | name of the XML map that need to be exported |
| path | const char16_t* | the export path |
## Examples
```cpp
Aspose::Cells::Startup();
//The following code exported the data linked by the first XmlMap.
Workbook wb(u"Book1.xlsx");
//Make sure that the source xlsx file contains a XmlMap.
wb.ExportXml(u"XmlMapName", u"output.xml");
Aspose::Cells::Cleanup();
```
## See Also
* Class [Vector](../../vector/)
* Class [Workbook](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
## Workbook::ExportXml(const U16String\&) method
Export XML data.
```cpp
Vector<uint8_t> Aspose::Cells::Workbook::ExportXml(const U16String &mapName)
```
| Parameter | Type | Description |
| --- | --- | --- |
| mapName | const U16String\& | name of the XML map that need to be exported |
## See Also
* Class [Vector](../../vector/)
* Class [U16String](../../u16string/)
* Class [Workbook](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
## Workbook::ExportXml(const char16_t*) method
Export XML data.
```cpp
Vector<uint8_t> Aspose::Cells::Workbook::ExportXml(const char16_t *mapName)
```
| Parameter | Type | Description |
| --- | --- | --- |
| mapName | const char16_t* | name of the XML map that need to be exported |
## See Also
* Class [Vector](../../vector/)
* Class [Workbook](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
