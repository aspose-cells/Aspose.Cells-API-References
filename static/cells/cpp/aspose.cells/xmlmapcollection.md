##Aspose::Cells::XmlMapCollection class
'Aspose::Cells::XmlMapCollection class. A collection of XmlMap objects that represent XmlMap information in C++.'
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
//The following code adds two XmlMaps by a xsd file and a xml file.
Workbook wb;
XmlMapCollection xmlMapCollection = wb.GetWorksheets().GetXmlMaps();
//Add a XmlMap by a xsd file.
xmlMapCollection.Add(u"schema.xsd");
//Add a XmlMap by a xml file.
xmlMapCollection.Add(u"xml.xml");
wb.Save(u"twoXmlMaps.xlsx");
Aspose::Cells::Cleanup();
```
## See Also
* Namespace [Aspose::Cells](../)
* Library [Aspose.Cells for C++](../../)
