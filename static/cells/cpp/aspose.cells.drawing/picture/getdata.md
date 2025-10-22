##Aspose::Cells::Drawing::Picture::GetData method
'Aspose::Cells::Drawing::Picture::GetData method. Gets the data of the picture in C++.'
## Picture::GetData method
Gets the data of the picture.
```cpp
Vector<uint8_t> Aspose::Cells::Drawing::Picture::GetData()
```
## Examples
```cpp
Aspose::Cells::Startup();
//Instantiating a Workbook object
Workbook workbook;
Worksheet worksheet = workbook.GetWorksheets().Get(0);
//insert first picture
int imgIndex1 = worksheet.GetPictures().Add(1, 1, u"example1.png");
//Get the inserted picture object
Picture pic1 = worksheet.GetPictures().Get(imgIndex1);
//insert second picture
int imgIndex2 = worksheet.GetPictures().Add(1, 9, u"example2.jpeg");
//Get the inserted picture object
Picture pic2 = worksheet.GetPictures().Get(imgIndex2);
//Assign the byte data of the first image to the second image
pic2.SetData(pic1.GetData());
//Save the excel file.
workbook.Save(u"result.xlsx");
Aspose::Cells::Cleanup();
```
## See Also
* Class [Vector](../../../aspose.cells/vector/)
* Class [Picture](../)
* Namespace [Aspose::Cells::Drawing](../../)
* Library [Aspose.Cells for C++](../../../)
