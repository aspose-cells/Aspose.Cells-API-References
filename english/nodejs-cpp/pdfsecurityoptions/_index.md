---
title: PdfSecurityOptions
second_title: Aspose.Cells for Node.js via C++ API Reference
description: Options for encrypting and access permissions for a PDF document. PDFA does not allow security setting.
type: docs
url: /nodejs-cpp/pdfsecurityoptions/
---

## PdfSecurityOptions class

Options for encrypting and access permissions for a PDF document. PDF/A does not allow security setting.

```javascript
class PdfSecurityOptions;
```


## Constructors

| Name | Description |
| --- | --- |
| [constructor()](#constructor--)| The constructor of PdfSecurityOptions |

## Methods

| Method | Description |
| --- | --- |
| [getUserPassword()](#getUserPassword--)| Gets or sets the user password required for opening the encrypted PDF document. |
| [setUserPassword(string)](#setUserPassword-string-)| Gets or sets the user password required for opening the encrypted PDF document. |
| [getOwnerPassword()](#getOwnerPassword--)| Gets or sets the owner password for the encrypted PDF document. |
| [setOwnerPassword(string)](#setOwnerPassword-string-)| Gets or sets the owner password for the encrypted PDF document. |
| [getPrintPermission()](#getPrintPermission--)| Indicates whether to allow to print the document. |
| [setPrintPermission(boolean)](#setPrintPermission-boolean-)| Indicates whether to allow to print the document. |
| [getModifyDocumentPermission()](#getModifyDocumentPermission--)| Indicates whether to allow to modify the contents of the document by operations other than those controlled by [AnnotationsPermission](../annotationspermission/), [FillFormsPermission](../fillformspermission/) and [AssembleDocumentPermission](../assembledocumentpermission/). |
| [setModifyDocumentPermission(boolean)](#setModifyDocumentPermission-boolean-)| Indicates whether to allow to modify the contents of the document by operations other than those controlled by [AnnotationsPermission](../annotationspermission/), [FillFormsPermission](../fillformspermission/) and [AssembleDocumentPermission](../assembledocumentpermission/). |
| [getAnnotationsPermission()](#getAnnotationsPermission--)| Indicates whether to allow to add or modify text annotations, fill in interactive form fields. |
| [setAnnotationsPermission(boolean)](#setAnnotationsPermission-boolean-)| Indicates whether to allow to add or modify text annotations, fill in interactive form fields. |
| [getFillFormsPermission()](#getFillFormsPermission--)| Indicates whether to allow to fill in existing interactive form fields (including signature fields), even if [ModifyDocumentPermission](../modifydocumentpermission/) is clear. |
| [setFillFormsPermission(boolean)](#setFillFormsPermission-boolean-)| Indicates whether to allow to fill in existing interactive form fields (including signature fields), even if [ModifyDocumentPermission](../modifydocumentpermission/) is clear. |
| [getExtractContentPermission()](#getExtractContentPermission--)| Indicates whether to allow to copy or otherwise extract text and graphics from the document by operations other than that controlled by [AccessibilityExtractContent](../accessibilityextractcontent/). |
| [setExtractContentPermission(boolean)](#setExtractContentPermission-boolean-)| Indicates whether to allow to copy or otherwise extract text and graphics from the document by operations other than that controlled by [AccessibilityExtractContent](../accessibilityextractcontent/). |
| [getAccessibilityExtractContent()](#getAccessibilityExtractContent--)| Indicates whether to allow to extract text and graphics (in support of accessibility to users with disabilities or for other purposes). |
| [setAccessibilityExtractContent(boolean)](#setAccessibilityExtractContent-boolean-)| Indicates whether to allow to extract text and graphics (in support of accessibility to users with disabilities or for other purposes). |
| [getAssembleDocumentPermission()](#getAssembleDocumentPermission--)| Indicates whether to allow to assemble the document (insert, rotate, or delete pages and create bookmarks or thumbnail images), even if [ModifyDocumentPermission](../modifydocumentpermission/) is clear. |
| [setAssembleDocumentPermission(boolean)](#setAssembleDocumentPermission-boolean-)| Indicates whether to allow to assemble the document (insert, rotate, or delete pages and create bookmarks or thumbnail images), even if [ModifyDocumentPermission](../modifydocumentpermission/) is clear. |
| [getFullQualityPrintPermission()](#getFullQualityPrintPermission--)| Indicates whether to allow to print the document to a representation from which a faithful digital copy of the PDF content could be generated. |
| [setFullQualityPrintPermission(boolean)](#setFullQualityPrintPermission-boolean-)| Indicates whether to allow to print the document to a representation from which a faithful digital copy of the PDF content could be generated. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |


### constructor() {#constructor--}

The constructor of PdfSecurityOptions

```javascript
constructor();
```


### getUserPassword() {#getUserPassword--}

Gets or sets the user password required for opening the encrypted PDF document.

```javascript
getUserPassword() : string;
```


**Remarks**

The owner password or user password will be required to open an encrypted PDF document for viewing.</p> <p>The user password can be null or empty string, in this case no password will be required from the user when opening the PDF document.</p> <p>Opening the document with the correct owner password allows full access to the document.</p> <p>Opening the document with the correct user password (or opening a document that does not have a user password) allows limited access as the permissions specified.

### setUserPassword(string) {#setUserPassword-string-}

Gets or sets the user password required for opening the encrypted PDF document.

```javascript
setUserPassword(value: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |

**Remarks**

The owner password or user password will be required to open an encrypted PDF document for viewing.</p> <p>The user password can be null or empty string, in this case no password will be required from the user when opening the PDF document.</p> <p>Opening the document with the correct owner password allows full access to the document.</p> <p>Opening the document with the correct user password (or opening a document that does not have a user password) allows limited access as the permissions specified.

### getOwnerPassword() {#getOwnerPassword--}

Gets or sets the owner password for the encrypted PDF document.

```javascript
getOwnerPassword() : string;
```


**Remarks**

The owner password allows the user to open an encrypted PDF document without any access restrictions specified.

### setOwnerPassword(string) {#setOwnerPassword-string-}

Gets or sets the owner password for the encrypted PDF document.

```javascript
setOwnerPassword(value: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |

**Remarks**

The owner password allows the user to open an encrypted PDF document without any access restrictions specified.

### getPrintPermission() {#getPrintPermission--}

Indicates whether to allow to print the document.

```javascript
getPrintPermission() : boolean;
```


**Remarks**

Possibly not at the highest quality level, depending on whether [FullQualityPrintPermission](../fullqualityprintpermission/) is also set.

### setPrintPermission(boolean) {#setPrintPermission-boolean-}

Indicates whether to allow to print the document.

```javascript
setPrintPermission(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

**Remarks**

Possibly not at the highest quality level, depending on whether [FullQualityPrintPermission](../fullqualityprintpermission/) is also set.

### getModifyDocumentPermission() {#getModifyDocumentPermission--}

Indicates whether to allow to modify the contents of the document by operations other than those controlled by [AnnotationsPermission](../annotationspermission/), [FillFormsPermission](../fillformspermission/) and [AssembleDocumentPermission](../assembledocumentpermission/).

```javascript
getModifyDocumentPermission() : boolean;
```


### setModifyDocumentPermission(boolean) {#setModifyDocumentPermission-boolean-}

Indicates whether to allow to modify the contents of the document by operations other than those controlled by [AnnotationsPermission](../annotationspermission/), [FillFormsPermission](../fillformspermission/) and [AssembleDocumentPermission](../assembledocumentpermission/).

```javascript
setModifyDocumentPermission(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getAnnotationsPermission() {#getAnnotationsPermission--}

Indicates whether to allow to add or modify text annotations, fill in interactive form fields.

```javascript
getAnnotationsPermission() : boolean;
```


**Remarks**

if [ModifyDocumentPermission](../modifydocumentpermission/) is also set, create or modify interactive form fields (including signature fields).

### setAnnotationsPermission(boolean) {#setAnnotationsPermission-boolean-}

Indicates whether to allow to add or modify text annotations, fill in interactive form fields.

```javascript
setAnnotationsPermission(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

**Remarks**

if [ModifyDocumentPermission](../modifydocumentpermission/) is also set, create or modify interactive form fields (including signature fields).

### getFillFormsPermission() {#getFillFormsPermission--}

Indicates whether to allow to fill in existing interactive form fields (including signature fields), even if [ModifyDocumentPermission](../modifydocumentpermission/) is clear.

```javascript
getFillFormsPermission() : boolean;
```


### setFillFormsPermission(boolean) {#setFillFormsPermission-boolean-}

Indicates whether to allow to fill in existing interactive form fields (including signature fields), even if [ModifyDocumentPermission](../modifydocumentpermission/) is clear.

```javascript
setFillFormsPermission(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getExtractContentPermission() {#getExtractContentPermission--}

Indicates whether to allow to copy or otherwise extract text and graphics from the document by operations other than that controlled by [AccessibilityExtractContent](../accessibilityextractcontent/).

```javascript
getExtractContentPermission() : boolean;
```


### setExtractContentPermission(boolean) {#setExtractContentPermission-boolean-}

Indicates whether to allow to copy or otherwise extract text and graphics from the document by operations other than that controlled by [AccessibilityExtractContent](../accessibilityextractcontent/).

```javascript
setExtractContentPermission(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getAccessibilityExtractContent() {#getAccessibilityExtractContent--}

Indicates whether to allow to extract text and graphics (in support of accessibility to users with disabilities or for other purposes).

```javascript
getAccessibilityExtractContent() : boolean;
```


### setAccessibilityExtractContent(boolean) {#setAccessibilityExtractContent-boolean-}

Indicates whether to allow to extract text and graphics (in support of accessibility to users with disabilities or for other purposes).

```javascript
setAccessibilityExtractContent(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getAssembleDocumentPermission() {#getAssembleDocumentPermission--}

Indicates whether to allow to assemble the document (insert, rotate, or delete pages and create bookmarks or thumbnail images), even if [ModifyDocumentPermission](../modifydocumentpermission/) is clear.

```javascript
getAssembleDocumentPermission() : boolean;
```


### setAssembleDocumentPermission(boolean) {#setAssembleDocumentPermission-boolean-}

Indicates whether to allow to assemble the document (insert, rotate, or delete pages and create bookmarks or thumbnail images), even if [ModifyDocumentPermission](../modifydocumentpermission/) is clear.

```javascript
setAssembleDocumentPermission(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getFullQualityPrintPermission() {#getFullQualityPrintPermission--}

Indicates whether to allow to print the document to a representation from which a faithful digital copy of the PDF content could be generated.

```javascript
getFullQualityPrintPermission() : boolean;
```


**Remarks**

When it is clear (and [PrintPermission](../printpermission/) is set), printing is limited to a low level representation of the appearance, possibly of degraded quality.

### setFullQualityPrintPermission(boolean) {#setFullQualityPrintPermission-boolean-}

Indicates whether to allow to print the document to a representation from which a faithful digital copy of the PDF content could be generated.

```javascript
setFullQualityPrintPermission(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

**Remarks**

When it is clear (and [PrintPermission](../printpermission/) is set), printing is limited to a low level representation of the appearance, possibly of degraded quality.

### isNull() {#isNull--}

Checks whether the implementation object is null.

```javascript
isNull() : boolean;
```



