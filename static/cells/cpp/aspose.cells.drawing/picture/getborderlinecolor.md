##Aspose::Cells::Drawing::Picture::GetBorderLineColor method
'Aspose::Cells::Drawing::Picture::GetBorderLineColor method. Represents the Color of the border line of a picture in C++.'
## Picture::GetBorderLineColor method
Represents the [Color](../../../aspose.cells/color/) of the border line of a picture.
```cpp
Aspose::Cells::Color Aspose::Cells::Drawing::Picture::GetBorderLineColor()
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
//Set the border color of the picture
if (pic.GetBorderLineColor() == Color{ 0xff, 0, 0, 0xff })//Blue
{
pic.SetBorderLineColor(Color{ 0xff, 0xff, 0, 0 });//Red
}
//Save the excel file.
workbook.Save(u"result.xlsx");
Aspose::Cells::Cleanup();
```
## See Also
* Class [Picture](../)
* Namespace [Aspose::Cells::Drawing](../../)
* Library [Aspose.Cells for C++](../../../)
