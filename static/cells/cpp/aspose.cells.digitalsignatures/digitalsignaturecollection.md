##Aspose::Cells::DigitalSignatures::DigitalSignatureCollection class
'Aspose::Cells::DigitalSignatures::DigitalSignatureCollection class. Provides a collection of digital signatures attached to a document in C++.'
## DigitalSignatureCollection class
Provides a collection of digital signatures attached to a document.
```cpp
class DigitalSignatureCollection
```
## Methods
| Method | Description |
| --- | --- |
| [Add(const DigitalSignature\& digitalSignature)](./add/) | Add one signature to [DigitalSignatureCollection](./). |
| [DigitalSignatureCollection()](./digitalsignaturecollection/) | The constructor of [DigitalSignatureCollection](./). |
| [DigitalSignatureCollection(DigitalSignatureCollection_Impl* impl)](./digitalsignaturecollection/) | Constructs from an implementation object. |
| [DigitalSignatureCollection(const DigitalSignatureCollection\& src)](./digitalsignaturecollection/) | Copy constructor. |
| [GetEnumerator()](./getenumerator/) | Get the enumerator for [DigitalSignatureCollection](./), this enumerator allows iteration over the collection. |
| [IsNull()](./isnull/) const | Checks whether the implementation object is nullptr. |
| explicit [operator bool()](./operator_bool/) const | operator bool() |
| [operator=(const DigitalSignatureCollection\& src)](./operator_asm/) | operator= |
| [~DigitalSignatureCollection()](./~digitalsignaturecollection/) | Destructor. |
## Fields
| Field | Description |
| --- | --- |
| [_impl](./_impl/) | The implementation object. |
## Examples
```cpp
Aspose::Cells::Startup();
//The following example shows how to validate digital signature.
//workbook from a signed source file
Workbook signedWorkbook(u"signedFile.xlsx");
//wb.IsDigitallySigned is true when the workbook is signed already.
std::cout<<signedWorkbook.IsDigitallySigned() << std::endl;
//get digitalSignature collection from workbook
DigitalSignatureCollection existingDsc = signedWorkbook.GetDigitalSignature();
Enumerator<DigitalSignature> en = existingDsc.GetEnumerator();
while (en.MoveNext())
{
DigitalSignature existingDs = (DigitalSignature)en.GetCurrent();
std::cout << "existingDs.Comments : " << existingDs.GetComments().ToUtf8() << std::endl;
Date dt = existingDs.GetSignTime();
std::cout << "existingDs.SignTime : " << dt.year << "-" << dt.month << "-" << dt.day << " " << dt.hour << ":" << dt.minute << ":" << dt.second << std::endl;
std::cout << "existingDs.IsValid = " << (existingDs.IsValid() ? "True" : "False") << std::endl;
}
Aspose::Cells::Cleanup();
```
## See Also
* Namespace [Aspose::Cells::DigitalSignatures](../)
* Library [Aspose.Cells for C++](../../)
