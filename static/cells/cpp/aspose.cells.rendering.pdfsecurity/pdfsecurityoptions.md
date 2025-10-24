##Aspose::Cells::Rendering::PdfSecurity::PdfSecurityOptions class
'Aspose::Cells::Rendering::PdfSecurity::PdfSecurityOptions class. Options for encrypting and access permissions for a PDF document. PDF/A does not allow security setting in C++.'
## PdfSecurityOptions class
Options for encrypting and access permissions for a PDF document. PDF/A does not allow security setting.
```cpp
class PdfSecurityOptions
```
## Methods
| Method | Description |
| --- | --- |
| [GetAccessibilityExtractContent()](./getaccessibilityextractcontent/) | Indicates whether to allow to extract text and graphics (in support of accessibility to users with disabilities or for other purposes). |
| [GetAnnotationsPermission()](./getannotationspermission/) | Indicates whether to allow to add or modify text annotations, fill in interactive form fields. |
| [GetAssembleDocumentPermission()](./getassembledocumentpermission/) | Indicates whether to allow to assemble the document (insert, rotate, or delete pages and create bookmarks or thumbnail images), even if ModifyDocumentPermission is clear. |
| [GetExtractContentPermission()](./getextractcontentpermission/) | Indicates whether to allow to copy or otherwise extract text and graphics from the document by operations other than that controlled by AccessibilityExtractContent. |
| [GetFillFormsPermission()](./getfillformspermission/) | Indicates whether to allow to fill in existing interactive form fields (including signature fields), even if ModifyDocumentPermission is clear. |
| [GetFullQualityPrintPermission()](./getfullqualityprintpermission/) | Indicates whether to allow to print the document to a representation from which a faithful digital copy of the PDF content could be generated. |
| [GetModifyDocumentPermission()](./getmodifydocumentpermission/) | Indicates whether to allow to modify the contents of the document by operations other than those controlled by AnnotationsPermission, FillFormsPermission and AssembleDocumentPermission. |
| [GetOwnerPassword()](./getownerpassword/) | Gets or sets the owner password for the encrypted PDF document. |
| [GetPrintPermission()](./getprintpermission/) | Indicates whether to allow to print the document. |
| [GetUserPassword()](./getuserpassword/) | Gets or sets the user password required for opening the encrypted PDF document. |
| [IsNull()](./isnull/) const | Checks whether the implementation object is nullptr. |
| explicit [operator bool()](./operator_bool/) const | operator bool() |
| [operator=(const PdfSecurityOptions\& src)](./operator_asm/) | operator= |
| [PdfSecurityOptions()](./pdfsecurityoptions/) | The constructor of [PdfSecurityOptions](./). |
| [PdfSecurityOptions(PdfSecurityOptions_Impl* impl)](./pdfsecurityoptions/) | Constructs from an implementation object. |
| [PdfSecurityOptions(const PdfSecurityOptions\& src)](./pdfsecurityoptions/) | Copy constructor. |
| [SetAccessibilityExtractContent(bool value)](./setaccessibilityextractcontent/) | Indicates whether to allow to extract text and graphics (in support of accessibility to users with disabilities or for other purposes). |
| [SetAnnotationsPermission(bool value)](./setannotationspermission/) | Indicates whether to allow to add or modify text annotations, fill in interactive form fields. |
| [SetAssembleDocumentPermission(bool value)](./setassembledocumentpermission/) | Indicates whether to allow to assemble the document (insert, rotate, or delete pages and create bookmarks or thumbnail images), even if ModifyDocumentPermission is clear. |
| [SetExtractContentPermission(bool value)](./setextractcontentpermission/) | Indicates whether to allow to copy or otherwise extract text and graphics from the document by operations other than that controlled by AccessibilityExtractContent. |
| [SetFillFormsPermission(bool value)](./setfillformspermission/) | Indicates whether to allow to fill in existing interactive form fields (including signature fields), even if ModifyDocumentPermission is clear. |
| [SetFullQualityPrintPermission(bool value)](./setfullqualityprintpermission/) | Indicates whether to allow to print the document to a representation from which a faithful digital copy of the PDF content could be generated. |
| [SetModifyDocumentPermission(bool value)](./setmodifydocumentpermission/) | Indicates whether to allow to modify the contents of the document by operations other than those controlled by AnnotationsPermission, FillFormsPermission and AssembleDocumentPermission. |
| [SetOwnerPassword(const U16String\& value)](./setownerpassword/) | Gets or sets the owner password for the encrypted PDF document. |
| [SetOwnerPassword(const char16_t* value)](./setownerpassword/) | Gets or sets the owner password for the encrypted PDF document. |
| [SetPrintPermission(bool value)](./setprintpermission/) | Indicates whether to allow to print the document. |
| [SetUserPassword(const U16String\& value)](./setuserpassword/) | Gets or sets the user password required for opening the encrypted PDF document. |
| [SetUserPassword(const char16_t* value)](./setuserpassword/) | Gets or sets the user password required for opening the encrypted PDF document. |
| [~PdfSecurityOptions()](./~pdfsecurityoptions/) | Destructor. |
## Fields
| Field | Description |
| --- | --- |
| [_impl](./_impl/) | The implementation object. |
## See Also
* Namespace [Aspose::Cells::Rendering::PdfSecurity](../)
* Library [Aspose.Cells for C++](../../)
