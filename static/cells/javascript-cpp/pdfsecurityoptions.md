##PdfSecurityOptions
Options for encrypting and access permissions for a PDF document. PDFA does not allow security setting.
## PdfSecurityOptions class
Options for encrypting and access permissions for a PDF document. PDF/A does not allow security setting.
```javascript
class PdfSecurityOptions;
```
## Constructors
| Name | Description |
| --- | --- |
| [constructor()](#constructor--)| The constructor of PdfSecurityOptions |
## Properties
| Property | Type | Description |
| --- | --- | --- |
| [userPassword](#userPassword--)| string | Gets or sets the user password required for opening the encrypted PDF document. |
| [ownerPassword](#ownerPassword--)| string | Gets or sets the owner password for the encrypted PDF document. |
| [printPermission](#printPermission--)| boolean | Indicates whether to allow to print the document. |
| [modifyDocumentPermission](#modifyDocumentPermission--)| boolean | Indicates whether to allow to modify the contents of the document by operations other than those controlled by [AnnotationsPermission](../annotationspermission/), [FillFormsPermission](../fillformspermission/) and [AssembleDocumentPermission](../assembledocumentpermission/). |
| [annotationsPermission](#annotationsPermission--)| boolean | Indicates whether to allow to add or modify text annotations, fill in interactive form fields. |
| [fillFormsPermission](#fillFormsPermission--)| boolean | Indicates whether to allow to fill in existing interactive form fields (including signature fields), even if [ModifyDocumentPermission](../modifydocumentpermission/) is clear. |
| [extractContentPermission](#extractContentPermission--)| boolean | Indicates whether to allow to copy or otherwise extract text and graphics from the document by operations other than that controlled by [AccessibilityExtractContent](../accessibilityextractcontent/). |
| [accessibilityExtractContent](#accessibilityExtractContent--)| boolean | Indicates whether to allow to extract text and graphics (in support of accessibility to users with disabilities or for other purposes). |
| [assembleDocumentPermission](#assembleDocumentPermission--)| boolean | Indicates whether to allow to assemble the document (insert, rotate, or delete pages and create bookmarks or thumbnail images), even if [ModifyDocumentPermission](../modifydocumentpermission/) is clear. |
| [fullQualityPrintPermission](#fullQualityPrintPermission--)| boolean | Indicates whether to allow to print the document to a representation from which a faithful digital copy of the PDF content could be generated. |
### constructor() {#constructor--}
The constructor of PdfSecurityOptions
```javascript
constructor();
```
### userPassword {#userPassword--}
Gets or sets the user password required for opening the encrypted PDF document.
```javascript
userPassword : string;
```
**Remarks**
The owner password or user password will be required to open an encrypted PDF document for viewing.</p> <p>The user password can be null or empty string, in this case no password will be required from the user when opening the PDF document.</p> <p>Opening the document with the correct owner password allows full access to the document.</p> <p>Opening the document with the correct user password (or opening a document that does not have a user password) allows limited access as the permissions specified.
### ownerPassword {#ownerPassword--}
Gets or sets the owner password for the encrypted PDF document.
```javascript
ownerPassword : string;
```
**Remarks**
The owner password allows the user to open an encrypted PDF document without any access restrictions specified.
### printPermission {#printPermission--}
Indicates whether to allow to print the document.
```javascript
printPermission : boolean;
```
**Remarks**
Possibly not at the highest quality level, depending on whether [FullQualityPrintPermission](../fullqualityprintpermission/) is also set.
### modifyDocumentPermission {#modifyDocumentPermission--}
Indicates whether to allow to modify the contents of the document by operations other than those controlled by [AnnotationsPermission](../annotationspermission/), [FillFormsPermission](../fillformspermission/) and [AssembleDocumentPermission](../assembledocumentpermission/).
```javascript
modifyDocumentPermission : boolean;
```
### annotationsPermission {#annotationsPermission--}
Indicates whether to allow to add or modify text annotations, fill in interactive form fields.
```javascript
annotationsPermission : boolean;
```
**Remarks**
if [ModifyDocumentPermission](../modifydocumentpermission/) is also set, create or modify interactive form fields (including signature fields).
### fillFormsPermission {#fillFormsPermission--}
Indicates whether to allow to fill in existing interactive form fields (including signature fields), even if [ModifyDocumentPermission](../modifydocumentpermission/) is clear.
```javascript
fillFormsPermission : boolean;
```
### extractContentPermission {#extractContentPermission--}
Indicates whether to allow to copy or otherwise extract text and graphics from the document by operations other than that controlled by [AccessibilityExtractContent](../accessibilityextractcontent/).
```javascript
extractContentPermission : boolean;
```
### accessibilityExtractContent {#accessibilityExtractContent--}
Indicates whether to allow to extract text and graphics (in support of accessibility to users with disabilities or for other purposes).
```javascript
accessibilityExtractContent : boolean;
```
### assembleDocumentPermission {#assembleDocumentPermission--}
Indicates whether to allow to assemble the document (insert, rotate, or delete pages and create bookmarks or thumbnail images), even if [ModifyDocumentPermission](../modifydocumentpermission/) is clear.
```javascript
assembleDocumentPermission : boolean;
```
### fullQualityPrintPermission {#fullQualityPrintPermission--}
Indicates whether to allow to print the document to a representation from which a faithful digital copy of the PDF content could be generated.
```javascript
fullQualityPrintPermission : boolean;
```
**Remarks**
When it is clear (and [PrintPermission](../printpermission/) is set), printing is limited to a low level representation of the appearance, possibly of degraded quality.
