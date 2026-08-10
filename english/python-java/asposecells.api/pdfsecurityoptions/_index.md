---
title: "PdfSecurityOptions Class"
linktitle: "PdfSecurityOptions"
articleTitle: "PdfSecurityOptions"
second_title: "Aspose.Cells for Python via Java"
description: "Options for encrypting and access permissions for a PDF document."
type: docs
weight: 4370
url: /python-java/asposecells.api/pdfsecurityoptions/
---

## PdfSecurityOptions class

Options for encrypting and access permissions for a PDF document. PDF/A does not allow security setting.

## Constructors

| Name | Description |
| --- | --- |
| [PdfSecurityOptions](#constructor) | The constructor of PdfSecurityOptions |

## Properties

| Name | Type | Description |
| --- | --- | --- |
| [UserPassword](#userpassword) | String | Gets or sets the user password required for opening the encrypted PDF document. The owner password or user password will |
| [OwnerPassword](#ownerpassword) | String | Gets or sets the owner password for the encrypted PDF document. The owner password allows the user to open an encrypted  |
| [PrintPermission](#printpermission) | boolean | Indicates whether to allow to print the document. Possibly not at the highest quality level, depending on whether FullQu |
| [ModifyDocumentPermission](#modifydocumentpermission) | boolean | Indicates whether to allow to modify the contents of the document by operations other than those controlled by Annotatio |
| [ExtractContentPermissionObsolete](#extractcontentpermissionobsolete) | boolean | Permission to copy or extract content Obsoleted according to PDF reference. NOTE: This member is now obsolete. Instead,  |
| [AnnotationsPermission](#annotationspermission) | boolean | Indicates whether to allow to add or modify text annotations, fill in interactive form fields. if ModifyDocumentPermissi |
| [FillFormsPermission](#fillformspermission) | boolean | Indicates whether to allow to fill in existing interactive form fields (including signature fields), even if ModifyDocum |
| [ExtractContentPermission](#extractcontentpermission) | boolean | Indicates whether to allow to copy or otherwise extract text and graphics from the document by operations other than tha |
| [AccessibilityExtractContent](#accessibilityextractcontent) | boolean | Indicates whether to allow to extract text and graphics (in support of accessibility to users with disabilities or for o |
| [AssembleDocumentPermission](#assembledocumentpermission) | boolean | Indicates whether to allow to assemble the document (insert, rotate, or delete pages and create bookmarks or thumbnail i |
| [FullQualityPrintPermission](#fullqualityprintpermission) | boolean | Indicates whether to allow to print the document to a representation from which a faithful digital copy of the PDF conte |

### PdfSecurityOptions() {#constructor}

The constructor of PdfSecurityOptions

### PdfSecurityOptions.UserPassword property {#userpassword}

Gets or sets the user password required for opening the encrypted PDF document. The owner password or user password will be required to open an encrypted PDF document for viewing. The user password can be null or empty string, in this case no password will be required from the user when opening the PDF document. Opening the document with the correct owner password allows full access to the document. Opening the document with the correct user password (or opening a document that does not have a user password) allows limited access as the permissions specified.

**Type:** String

### PdfSecurityOptions.OwnerPassword property {#ownerpassword}

Gets or sets the owner password for the encrypted PDF document. The owner password allows the user to open an encrypted PDF document without any access restrictions specified.

**Type:** String

### PdfSecurityOptions.PrintPermission property {#printpermission}

Indicates whether to allow to print the document. Possibly not at the highest quality level, depending on whether FullQualityPrintPermission is also set.

**Type:** boolean

### PdfSecurityOptions.ModifyDocumentPermission property {#modifydocumentpermission}

Indicates whether to allow to modify the contents of the document by operations other than those controlled by AnnotationsPermission , FillFormsPermission and AssembleDocumentPermission .

**Type:** boolean

### PdfSecurityOptions.ExtractContentPermissionObsolete property {#extractcontentpermissionobsolete}

Permission to copy or extract content Obsoleted according to PDF reference. NOTE: This member is now obsolete. Instead, please use ExtractContentPermission property. This property will be removed 12 months later since September 2023. Aspose apologizes for any inconvenience you may have experienced.

**Type:** boolean

### PdfSecurityOptions.AnnotationsPermission property {#annotationspermission}

Indicates whether to allow to add or modify text annotations, fill in interactive form fields. if ModifyDocumentPermission is also set, create or modify interactive form fields (including signature fields).

**Type:** boolean

### PdfSecurityOptions.FillFormsPermission property {#fillformspermission}

Indicates whether to allow to fill in existing interactive form fields (including signature fields), even if ModifyDocumentPermission is clear.

**Type:** boolean

### PdfSecurityOptions.ExtractContentPermission property {#extractcontentpermission}

Indicates whether to allow to copy or otherwise extract text and graphics from the document by operations other than that controlled by AccessibilityExtractContent .

**Type:** boolean

### PdfSecurityOptions.AccessibilityExtractContent property {#accessibilityextractcontent}

Indicates whether to allow to extract text and graphics (in support of accessibility to users with disabilities or for other purposes).

**Type:** boolean

### PdfSecurityOptions.AssembleDocumentPermission property {#assembledocumentpermission}

Indicates whether to allow to assemble the document (insert, rotate, or delete pages and create bookmarks or thumbnail images), even if ModifyDocumentPermission is clear.

**Type:** boolean

### PdfSecurityOptions.FullQualityPrintPermission property {#fullqualityprintpermission}

Indicates whether to allow to print the document to a representation from which a faithful digital copy of the PDF content could be generated. When it is clear (and PrintPermission is set), printing is limited to a low level representation of the appearance, possibly of degraded quality.

**Type:** boolean
