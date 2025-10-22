##Aspose::Cells::Drawing::Picture::SetBorderWeight method
'Aspose::Cells::Drawing::Picture::SetBorderWeight method. Gets or sets the weight of the border line of a picture in units of pt in C++.'
## Picture::SetBorderWeight method
Gets or sets the weight of the border line of a picture in units of pt.
```cpp
void Aspose::Cells::Drawing::Picture::SetBorderWeight(double value)
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
pic.SetBorderLineColor(Color{ 0xff, 0xff, 0, 0 });//Red
//Set the border width of the picture
if (pic.GetBorderWeight() == 3)
{
pic.SetBorderWeight(3);
}
//Save the excel file.
workbook.Save(u"result.xlsx");
Aspose::Cells::Cleanup();
```
## See Also
* Class [Vector](../../../aspose.cells/vector/)
* Class [Picture](../)
* Namespace [Aspose::Cells::Drawing](../../)
* Library [Aspose.Cells for C++](../../../)
