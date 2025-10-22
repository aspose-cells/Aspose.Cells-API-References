##Aspose::Cells::Rendering::PdfSecurity::PdfSecurityOptions::GetUserPassword method
'Aspose::Cells::Rendering::PdfSecurity::PdfSecurityOptions::GetUserPassword method. Gets or sets the user password required for opening the encrypted PDF document in C++.'
## PdfSecurityOptions::GetUserPassword method
Gets or sets the user password required for opening the encrypted PDF document.
```cpp
U16String Aspose::Cells::Rendering::PdfSecurity::PdfSecurityOptions::GetUserPassword()
```
## Remarks
The owner password or user password will be required to open an encrypted PDF document for viewing.
The user password can be null or empty string, in this case no password will be required from the user when opening the PDF document.
Opening the document with the correct owner password allows full access to the document.
Opening the document with the correct user password (or opening a document that does not have a user password) allows limited access as the permissions specified.
## See Also
* Class [U16String](../../../aspose.cells/u16string/)
* Class [PdfSecurityOptions](../)
* Namespace [Aspose::Cells::Rendering::PdfSecurity](../../)
* Library [Aspose.Cells for C++](../../../)
