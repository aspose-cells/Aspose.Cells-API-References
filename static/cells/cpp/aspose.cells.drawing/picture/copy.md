##Aspose::Cells::Drawing::Picture::Copy method
'Aspose::Cells::Drawing::Picture::Copy method. Copy the picture in C++.'
## Picture::Copy method
Copy the picture.
```cpp
void Aspose::Cells::Drawing::Picture::Copy(const Aspose::Cells::Drawing::Picture &source, const CopyOptions &options)
```
| Parameter | Type | Description |
| --- | --- | --- |
| source | const Aspose::Cells::Drawing::Picture\& | The source picture. |
| options | const CopyOptions\& | The copy options. |
## Examples
```cpp
Aspose::Cells::Startup();
//Instantiating a Workbook object
Workbook workbook;
Worksheet worksheet = workbook.GetWorksheets().Get(0);
//insert first picture
int imgIndex1 = worksheet.GetPictures().Add(1, 1, u"1.png");
//Get the inserted picture object
Picture pic1 = worksheet.GetPictures().Get(imgIndex1);
//insert second picture
int imgIndex2 = worksheet.GetPictures().Add(1, 9, u"2.jpeg");
//Get the inserted picture object
Picture pic2 = worksheet.GetPictures().Get(imgIndex2);
//Copy picture 1 to picture 2.You'll get two picture 1 objects that are superimposed on top of each other.
CopyOptions opt;
pic2.Copy(pic1, opt);
//Save the excel file.
workbook.Save(u"result.xlsx");
Aspose::Cells::Cleanup();
```
## See Also
* Class [Vector](../../../aspose.cells/vector/)
* Class [Picture](../)
* Class [CopyOptions](../../../aspose.cells/copyoptions/)
* Class [Picture](../)
* Namespace [Aspose::Cells::Drawing](../../)
* Library [Aspose.Cells for C++](../../../)
