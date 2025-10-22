##Aspose::Cells::Drawing::Picture::GetSignatureLine method
'Aspose::Cells::Drawing::Picture::GetSignatureLine method. Gets and sets the signature line in C++.'
## Picture::GetSignatureLine method
Gets and sets the signature line.
```cpp
SignatureLine Aspose::Cells::Drawing::Picture::GetSignatureLine()
```
## Examples
```cpp
Aspose::Cells::Startup();
//Instantiating a Workbook object
Workbook workbook;
Worksheet worksheet = workbook.GetWorksheets().Get(0);
//Adding a picture at the location of a cell whose row and column indices are 1 in the worksheet. It is "B2" cell
int imgIndex = worksheet.GetPictures().Add(1, 1, Vector<uint8_t>(0));
//Get the inserted picture object
Picture pic = worksheet.GetPictures().Get(imgIndex);
// Create signature line object
SignatureLine s;
s.SetSigner(u"Simon Zhao");
s.SetTitle(u"Development Lead");
s.SetEmail(u"Simon.Zhao@aspose.com");
// Assign the signature line object to Picture.
pic.SetSignatureLine(s);
SignatureLine s2 = pic.GetSignatureLine();
if (s2.GetSigner() == s.GetSigner())
{
//do what you want
}
//Save the excel file.
workbook.Save(u"result.xlsx");
Aspose::Cells::Cleanup();
```
## See Also
* Class [SignatureLine](../../signatureline/)
* Class [Picture](../)
* Namespace [Aspose::Cells::Drawing](../../)
* Library [Aspose.Cells for C++](../../../)
