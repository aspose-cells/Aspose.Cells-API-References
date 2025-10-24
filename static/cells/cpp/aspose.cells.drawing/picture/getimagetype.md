##Aspose::Cells::Drawing::Picture::GetImageType method
'Aspose::Cells::Drawing::Picture::GetImageType method. Gets the image format of the picture in C++.'
## Picture::GetImageType method
Gets the image format of the picture.
```cpp
Aspose::Cells::Drawing::ImageType Aspose::Cells::Drawing::Picture::GetImageType()
```
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
if (pic1.GetImageType() == ImageType::Png)
{
//The picture's type is png.";
}
//insert second picture
int imgIndex2 = worksheet.GetPictures().Add(1, 9, u"2.jpeg");
//Get the inserted picture object
Picture pic2 = worksheet.GetPictures().Get(imgIndex2);
if (pic2.GetImageType() == ImageType::Jpeg)
{
//The picture's type is jpg.";
}
Aspose::Cells::Cleanup();
```
## See Also
* Enum [ImageType](../../imagetype/)
* Class [Picture](../)
* Namespace [Aspose::Cells::Drawing](../../)
* Library [Aspose.Cells for C++](../../../)
