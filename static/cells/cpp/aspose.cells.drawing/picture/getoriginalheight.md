##Aspose::Cells::Drawing::Picture::GetOriginalHeight method
'Aspose::Cells::Drawing::Picture::GetOriginalHeight method. Gets the original height of the picture in C++.'
## Picture::GetOriginalHeight method
Gets the original height of the picture.
```cpp
int32_t Aspose::Cells::Drawing::Picture::GetOriginalHeight()
```
## Examples
```cpp
Aspose::Cells::Startup();
//Instantiating a Workbook object
Workbook workbook;
Worksheet worksheet = workbook.GetWorksheets().Get(0);
//Adding a picture at the location of a cell whose row and column indices are 1 in the worksheet. It is "B2" cell
int imgIndex = worksheet.GetPictures().Add(1, 1, u"example.jpeg");
//Get the inserted picture object
Picture pic = worksheet.GetPictures().Get(imgIndex);
//Gets the original height of the picture.
int picHeight = pic.GetOriginalHeight();
//Save the excel file.
workbook.Save(u"result.xlsx");
Aspose::Cells::Cleanup();
```
## See Also
* Class [Vector](../../../aspose.cells/vector/)
* Class [Picture](../)
* Namespace [Aspose::Cells::Drawing](../../)
* Library [Aspose.Cells for C++](../../../)
