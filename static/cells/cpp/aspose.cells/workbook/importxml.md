##Aspose::Cells::Workbook::ImportXml method
'Aspose::Cells::Workbook::ImportXml method. Imports/Updates an XML data file into the workbook in C++.'
## Workbook::ImportXml(const U16String\&, const U16String\&, int32_t, int32_t) method
Imports/Updates an XML data file into the workbook.
```cpp
void Aspose::Cells::Workbook::ImportXml(const U16String &url, const U16String &sheetName, int32_t row, int32_t col)
```
| Parameter | Type | Description |
| --- | --- | --- |
| url | const U16String\& | the url/path of the xml file. |
| sheetName | const U16String\& | the destination sheet name. |
| row | int32_t | the destination row |
| col | int32_t | the destination column |
## Examples
```cpp
Aspose::Cells::Startup();
//The following code imports xml data into worksheet 'Sheet 1' at Cell A1.
Workbook wb(u"Book1.xlsx");
U16String val_1 = u"xml.xml";
U16String val_2 = u"Sheet1";
wb.ImportXml(val_1, val_2, 0, 0);
wb.Save(u"output.xlsx");
Aspose::Cells::Cleanup();
```
## See Also
* Class [Vector](../../vector/)
* Class [U16String](../../u16string/)
* Class [Workbook](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
## Workbook::ImportXml(const char16_t*, const char16_t*, int32_t, int32_t) method
Imports/Updates an XML data file into the workbook.
```cpp
void Aspose::Cells::Workbook::ImportXml(const char16_t *url, const char16_t *sheetName, int32_t row, int32_t col)
```
| Parameter | Type | Description |
| --- | --- | --- |
| url | const char16_t* | the url/path of the xml file. |
| sheetName | const char16_t* | the destination sheet name. |
| row | int32_t | the destination row |
| col | int32_t | the destination column |
## Examples
```cpp
Aspose::Cells::Startup();
//The following code imports xml data into worksheet 'Sheet 1' at Cell A1.
Workbook wb(u"Book1.xlsx");
wb.ImportXml(u"xml.xml", u"Sheet1", 0, 0);
wb.Save(u"output.xlsx");
Aspose::Cells::Cleanup();
```
## See Also
* Class [Vector](../../vector/)
* Class [Workbook](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
## Workbook::ImportXml(const Vector \<uint8_t\>\&, const U16String\&, int32_t, int32_t) method
Imports/Updates an XML data file into the workbook.
```cpp
void Aspose::Cells::Workbook::ImportXml(const Vector<uint8_t> &stream, const U16String &sheetName, int32_t row, int32_t col)
```
| Parameter | Type | Description |
| --- | --- | --- |
| stream | const Vector \<uint8_t\>\& | the xml file stream. |
| sheetName | const U16String\& | the destination sheet name. |
| row | int32_t | the destination row. |
| col | int32_t | the destination column. |
## See Also
* Class [Vector](../../vector/)
* Class [U16String](../../u16string/)
* Class [Workbook](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
## Workbook::ImportXml(const Vector \<uint8_t\>\&, const char16_t*, int32_t, int32_t) method
Imports/Updates an XML data file into the workbook.
```cpp
void Aspose::Cells::Workbook::ImportXml(const Vector<uint8_t> &stream, const char16_t *sheetName, int32_t row, int32_t col)
```
| Parameter | Type | Description |
| --- | --- | --- |
| stream | const Vector \<uint8_t\>\& | the xml file stream. |
| sheetName | const char16_t* | the destination sheet name. |
| row | int32_t | the destination row. |
| col | int32_t | the destination column. |
## See Also
* Class [Vector](../../vector/)
* Class [Workbook](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
