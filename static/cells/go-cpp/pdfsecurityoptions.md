##PdfSecurityOptions Class
'PdfSecurityOptions class. Encapsulates the object that represents pdfsecurityoptions in Go.'
## PdfSecurityOptions class
Options for encrypting and access permissions for a PDF document.PDF/A does not allow security setting.
```go
type PdfSecurityOptions struct  {
ptr unsafe.Pointer
}
```
## Constructors
| Method | Description |
| --- | --- |
|[NewPdfSecurityOptions](./newpdfsecurityoptions/) | The constructor of PdfSecurityOptions |
## Methods
| Method | Description |
| --- | --- |
|[IsNull](./isnull/) | Checks whether the implementation object is nullptr. |
|[GetUserPassword](./getuserpassword/) | Gets or sets the user password required for opening the encrypted PDF document. |
|[SetUserPassword](./setuserpassword/) | Gets or sets the user password required for opening the encrypted PDF document. |
|[GetOwnerPassword](./getownerpassword/) | Gets or sets the owner password for the encrypted PDF document. |
|[SetOwnerPassword](./setownerpassword/) | Gets or sets the owner password for the encrypted PDF document. |
|[GetPrintPermission](./getprintpermission/) | Indicates whether to allow to print the document. |
|[SetPrintPermission](./setprintpermission/) | Indicates whether to allow to print the document. |
|[GetModifyDocumentPermission](./getmodifydocumentpermission/) | Indicates whether to allow to modify the contents of the document by operations other than those controlledby AnnotationsPermission, FillFormsPermission and AssembleDocumentPermission. |
|[SetModifyDocumentPermission](./setmodifydocumentpermission/) | Indicates whether to allow to modify the contents of the document by operations other than those controlledby AnnotationsPermission, FillFormsPermission and AssembleDocumentPermission. |
|[GetAnnotationsPermission](./getannotationspermission/) | Indicates whether to allow to add or modify text annotations, fill in interactive form fields. |
|[SetAnnotationsPermission](./setannotationspermission/) | Indicates whether to allow to add or modify text annotations, fill in interactive form fields. |
|[GetFillFormsPermission](./getfillformspermission/) | Indicates whether to allow to fill in existing interactive form fields (including signature fields),even if ModifyDocumentPermission is clear. |
|[SetFillFormsPermission](./setfillformspermission/) | Indicates whether to allow to fill in existing interactive form fields (including signature fields),even if ModifyDocumentPermission is clear. |
|[GetExtractContentPermission](./getextractcontentpermission/) | Indicates whether to allow to copy or otherwise extract text and graphics from the documentby operations other than that controlled by AccessibilityExtractContent. |
|[SetExtractContentPermission](./setextractcontentpermission/) | Indicates whether to allow to copy or otherwise extract text and graphics from the documentby operations other than that controlled by AccessibilityExtractContent. |
|[GetAccessibilityExtractContent](./getaccessibilityextractcontent/) | Indicates whether to allow to extract text and graphics (in support of accessibility to users with disabilities or for other purposes). |
|[SetAccessibilityExtractContent](./setaccessibilityextractcontent/) | Indicates whether to allow to extract text and graphics (in support of accessibility to users with disabilities or for other purposes). |
|[GetAssembleDocumentPermission](./getassembledocumentpermission/) | Indicates whether to allow to assemble the document (insert, rotate, or delete pages and create bookmarks or thumbnail images),even if ModifyDocumentPermission is clear. |
|[SetAssembleDocumentPermission](./setassembledocumentpermission/) | Indicates whether to allow to assemble the document (insert, rotate, or delete pages and create bookmarks or thumbnail images),even if ModifyDocumentPermission is clear. |
|[GetFullQualityPrintPermission](./getfullqualityprintpermission/) | Indicates whether to allow to print the document to a representation fromwhich a faithful digital copy of the PDF content could be generated. |
|[SetFullQualityPrintPermission](./setfullqualityprintpermission/) | Indicates whether to allow to print the document to a representation fromwhich a faithful digital copy of the PDF content could be generated. |
