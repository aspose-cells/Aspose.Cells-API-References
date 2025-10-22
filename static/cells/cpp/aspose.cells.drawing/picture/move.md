##Aspose::Cells::Drawing::Picture::Move method
'Aspose::Cells::Drawing::Picture::Move method. Moves the picture to a specified location in C++.'
## Picture::Move method
Moves the picture to a specified location.
```cpp
void Aspose::Cells::Drawing::Picture::Move(int32_t upperLeftRow, int32_t upperLeftColumn)
```
| Parameter | Type | Description |
| --- | --- | --- |
| upperLeftRow | int32_t | Upper left row index. |
| upperLeftColumn | int32_t | Upper left column index. |
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
//Set the new location of the picture
pic.Move(2, 4);
//Save the excel file.
workbook.Save(u"result.xlsx");
Aspose::Cells::Cleanup();
```
## See Also
* Class [Vector](../../../aspose.cells/vector/)
* Class [Picture](../)
* Namespace [Aspose::Cells::Drawing](../../)
* Library [Aspose.Cells for C++](../../../)
