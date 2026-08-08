---
title: "PdfSecurityOptions"
linktitle: "PdfSecurityOptions"
second_title: "Aspose.Cells for Node.js via Java API Reference"
description: "Options for encrypting and access permissions for a PDF document."
type: docs
weight: 2600
url: /nodejs/aspose.cells/pdfsecurityoptions/
---

## PdfSecurityOptions class

Options for encrypting and access permissions for a PDF document. PDF/A does not allow security setting.

```js
new PdfSecurityOptions()
```

The constructor of PdfSecurityOptions

## Methods

| Name | Description |
| --- | --- |
| [getAccessibilityExtractContent()](#getaccessibilityextractcontent) | Indicates whether to allow to extract text and graphics (in support of accessibility to users with disabilities or for o |
| [getAnnotationsPermission()](#getannotationspermission) | Indicates whether to allow to add or modify text annotations, fill in interactive form fields. if ModifyDocumentPermissi |
| [getAssembleDocumentPermission()](#getassembledocumentpermission) | Indicates whether to allow to assemble the document (insert, rotate, or delete pages and create bookmarks or thumbnail i |
| [getExtractContentPermission()](#getextractcontentpermission) | Indicates whether to allow to copy or otherwise extract text and graphics from the document by operations other than tha |
| [getExtractContentPermissionObsolete()](#getextractcontentpermissionobsolete) | Permission to copy or extract content Obsoleted according to PDF reference. NOTE: This member is now obsolete. Instead,  |
| [getFillFormsPermission()](#getfillformspermission) | Indicates whether to allow to fill in existing interactive form fields (including signature fields), even if ModifyDocum |
| [getFullQualityPrintPermission()](#getfullqualityprintpermission) | Indicates whether to allow to print the document to a representation from which a faithful digital copy of the PDF conte |
| [getModifyDocumentPermission()](#getmodifydocumentpermission) | Indicates whether to allow to modify the contents of the document by operations other than those controlled by Annotatio |
| [getOwnerPassword()](#getownerpassword) | Gets or sets the owner password for the encrypted PDF document. The owner password allows the user to open an encrypted  |
| [getPrintPermission()](#getprintpermission) | Indicates whether to allow to print the document. Possibly not at the highest quality level, depending on whether FullQu |
| [getUserPassword()](#getuserpassword) | Gets or sets the user password required for opening the encrypted PDF document. The owner password or user password will |
| [setAccessibilityExtractContent()](#setaccessibilityextractcontent) | Indicates whether to allow to extract text and graphics (in support of accessibility to users with disabilities or for o |
| [setAnnotationsPermission()](#setannotationspermission) | Indicates whether to allow to add or modify text annotations, fill in interactive form fields. if ModifyDocumentPermissi |
| [setAssembleDocumentPermission()](#setassembledocumentpermission) | Indicates whether to allow to assemble the document (insert, rotate, or delete pages and create bookmarks or thumbnail i |
| [setExtractContentPermission()](#setextractcontentpermission) | Indicates whether to allow to copy or otherwise extract text and graphics from the document by operations other than tha |
| [setExtractContentPermissionObsolete()](#setextractcontentpermissionobsolete) | Permission to copy or extract content Obsoleted according to PDF reference. NOTE: This member is now obsolete. Instead,  |
| [setFillFormsPermission()](#setfillformspermission) | Indicates whether to allow to fill in existing interactive form fields (including signature fields), even if ModifyDocum |
| [setFullQualityPrintPermission()](#setfullqualityprintpermission) | Indicates whether to allow to print the document to a representation from which a faithful digital copy of the PDF conte |
| [setModifyDocumentPermission()](#setmodifydocumentpermission) | Indicates whether to allow to modify the contents of the document by operations other than those controlled by Annotatio |
| [setOwnerPassword()](#setownerpassword) | Gets or sets the owner password for the encrypted PDF document. The owner password allows the user to open an encrypted  |
| [setPrintPermission()](#setprintpermission) | Indicates whether to allow to print the document. Possibly not at the highest quality level, depending on whether FullQu |
| [setUserPassword()](#setuserpassword) | Gets or sets the user password required for opening the encrypted PDF document. The owner password or user password will |

### getAccessibilityExtractContent() {#getaccessibilityextractcontent}

Indicates whether to allow to extract text and graphics (in support of accessibility to users with disabilities or for other purposes).

### getAnnotationsPermission() {#getannotationspermission}

Indicates whether to allow to add or modify text annotations, fill in interactive form fields. if ModifyDocumentPermission is also set, create or modify interactive form fields (including signature fields).

### getAssembleDocumentPermission() {#getassembledocumentpermission}

Indicates whether to allow to assemble the document (insert, rotate, or delete pages and create bookmarks or thumbnail images), even if ModifyDocumentPermission is clear.

### getExtractContentPermission() {#getextractcontentpermission}

Indicates whether to allow to copy or otherwise extract text and graphics from the document by operations other than that controlled by AccessibilityExtractContent.

### getExtractContentPermissionObsolete() {#getextractcontentpermissionobsolete}

Permission to copy or extract content Obsoleted according to PDF reference. NOTE: This member is now obsolete. Instead, please use ExtractContentPermission property. This property will be removed 12 months later since September 2023. Aspose apologizes for any inconvenience you may have experienced.

### getFillFormsPermission() {#getfillformspermission}

Indicates whether to allow to fill in existing interactive form fields (including signature fields), even if ModifyDocumentPermission is clear.

### getFullQualityPrintPermission() {#getfullqualityprintpermission}

Indicates whether to allow to print the document to a representation from which a faithful digital copy of the PDF content could be generated. When it is clear (and PrintPermission is set), printing is limited to a low level representation of the appearance, possibly of degraded quality.

### getModifyDocumentPermission() {#getmodifydocumentpermission}

Indicates whether to allow to modify the contents of the document by operations other than those controlled by AnnotationsPermission, FillFormsPermission and AssembleDocumentPermission.

### getOwnerPassword() {#getownerpassword}

Gets or sets the owner password for the encrypted PDF document. The owner password allows the user to open an encrypted PDF document without any access restrictions specified.

### getPrintPermission() {#getprintpermission}

Indicates whether to allow to print the document. Possibly not at the highest quality level, depending on whether FullQualityPrintPermission is also set.

### getUserPassword() {#getuserpassword}

Gets or sets the user password required for opening the encrypted PDF document. The owner password or user password will be required to open an encrypted PDF document for viewing.The user password can be null or empty string, in this case no password will be required from the user when opening the PDF document.Opening the document with the correct owner password allows full access to the document.Opening the document with the correct user password (or opening a document that does not have a user password) allows limited access as the permissions specified.

### setAccessibilityExtractContent() {#setaccessibilityextractcontent}

Indicates whether to allow to extract text and graphics (in support of accessibility to users with disabilities or for other purposes).

### setAnnotationsPermission() {#setannotationspermission}

Indicates whether to allow to add or modify text annotations, fill in interactive form fields. if ModifyDocumentPermission is also set, create or modify interactive form fields (including signature fields).

### setAssembleDocumentPermission() {#setassembledocumentpermission}

Indicates whether to allow to assemble the document (insert, rotate, or delete pages and create bookmarks or thumbnail images), even if ModifyDocumentPermission is clear.

### setExtractContentPermission() {#setextractcontentpermission}

Indicates whether to allow to copy or otherwise extract text and graphics from the document by operations other than that controlled by AccessibilityExtractContent.

### setExtractContentPermissionObsolete() {#setextractcontentpermissionobsolete}

Permission to copy or extract content Obsoleted according to PDF reference. NOTE: This member is now obsolete. Instead, please use ExtractContentPermission property. This property will be removed 12 months later since September 2023. Aspose apologizes for any inconvenience you may have experienced.

### setFillFormsPermission() {#setfillformspermission}

Indicates whether to allow to fill in existing interactive form fields (including signature fields), even if ModifyDocumentPermission is clear.

### setFullQualityPrintPermission() {#setfullqualityprintpermission}

Indicates whether to allow to print the document to a representation from which a faithful digital copy of the PDF content could be generated. When it is clear (and PrintPermission is set), printing is limited to a low level representation of the appearance, possibly of degraded quality.

### setModifyDocumentPermission() {#setmodifydocumentpermission}

Indicates whether to allow to modify the contents of the document by operations other than those controlled by AnnotationsPermission, FillFormsPermission and AssembleDocumentPermission.

### setOwnerPassword() {#setownerpassword}

Gets or sets the owner password for the encrypted PDF document. The owner password allows the user to open an encrypted PDF document without any access restrictions specified.

### setPrintPermission() {#setprintpermission}

Indicates whether to allow to print the document. Possibly not at the highest quality level, depending on whether FullQualityPrintPermission is also set.

### setUserPassword() {#setuserpassword}

Gets or sets the user password required for opening the encrypted PDF document. The owner password or user password will be required to open an encrypted PDF document for viewing.The user password can be null or empty string, in this case no password will be required from the user when opening the PDF document.Opening the document with the correct owner password allows full access to the document.Opening the document with the correct user password (or opening a document that does not have a user password) allows limited access as the permissions specified.
