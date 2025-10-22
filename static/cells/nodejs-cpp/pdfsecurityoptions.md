##PdfSecurityOptions
Options for encrypting and access permissions for a PDF document. PDFA does not allow security setting.
## PdfSecurityOptions class
Options for encrypting and access permissions for a PDF document. PDF/A does not allow security setting.
```javascript
class PdfSecurityOptions;
```
## Constructors
| Constructor | Description |
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
## Methods
| Method | Description |
| --- | --- |
| [getUserPassword()](#getUserPassword--)| <b>@deprecated.</b> Please use the 'userPassword' property instead. Gets or sets the user password required for opening the encrypted PDF document. |
| [setUserPassword(string)](#setUserPassword-string-)| <b>@deprecated.</b> Please use the 'userPassword' property instead. Gets or sets the user password required for opening the encrypted PDF document. |
| [getOwnerPassword()](#getOwnerPassword--)| <b>@deprecated.</b> Please use the 'ownerPassword' property instead. Gets or sets the owner password for the encrypted PDF document. |
| [setOwnerPassword(string)](#setOwnerPassword-string-)| <b>@deprecated.</b> Please use the 'ownerPassword' property instead. Gets or sets the owner password for the encrypted PDF document. |
| [getPrintPermission()](#getPrintPermission--)| <b>@deprecated.</b> Please use the 'printPermission' property instead. Indicates whether to allow to print the document. |
| [setPrintPermission(boolean)](#setPrintPermission-boolean-)| <b>@deprecated.</b> Please use the 'printPermission' property instead. Indicates whether to allow to print the document. |
| [getModifyDocumentPermission()](#getModifyDocumentPermission--)| <b>@deprecated.</b> Please use the 'modifyDocumentPermission' property instead. Indicates whether to allow to modify the contents of the document by operations other than those controlled by [AnnotationsPermission](../annotationspermission/), [FillFormsPermission](../fillformspermission/) and [AssembleDocumentPermission](../assembledocumentpermission/). |
| [setModifyDocumentPermission(boolean)](#setModifyDocumentPermission-boolean-)| <b>@deprecated.</b> Please use the 'modifyDocumentPermission' property instead. Indicates whether to allow to modify the contents of the document by operations other than those controlled by [AnnotationsPermission](../annotationspermission/), [FillFormsPermission](../fillformspermission/) and [AssembleDocumentPermission](../assembledocumentpermission/). |
| [getAnnotationsPermission()](#getAnnotationsPermission--)| <b>@deprecated.</b> Please use the 'annotationsPermission' property instead. Indicates whether to allow to add or modify text annotations, fill in interactive form fields. |
| [setAnnotationsPermission(boolean)](#setAnnotationsPermission-boolean-)| <b>@deprecated.</b> Please use the 'annotationsPermission' property instead. Indicates whether to allow to add or modify text annotations, fill in interactive form fields. |
| [getFillFormsPermission()](#getFillFormsPermission--)| <b>@deprecated.</b> Please use the 'fillFormsPermission' property instead. Indicates whether to allow to fill in existing interactive form fields (including signature fields), even if [ModifyDocumentPermission](../modifydocumentpermission/) is clear. |
| [setFillFormsPermission(boolean)](#setFillFormsPermission-boolean-)| <b>@deprecated.</b> Please use the 'fillFormsPermission' property instead. Indicates whether to allow to fill in existing interactive form fields (including signature fields), even if [ModifyDocumentPermission](../modifydocumentpermission/) is clear. |
| [getExtractContentPermission()](#getExtractContentPermission--)| <b>@deprecated.</b> Please use the 'extractContentPermission' property instead. Indicates whether to allow to copy or otherwise extract text and graphics from the document by operations other than that controlled by [AccessibilityExtractContent](../accessibilityextractcontent/). |
| [setExtractContentPermission(boolean)](#setExtractContentPermission-boolean-)| <b>@deprecated.</b> Please use the 'extractContentPermission' property instead. Indicates whether to allow to copy or otherwise extract text and graphics from the document by operations other than that controlled by [AccessibilityExtractContent](../accessibilityextractcontent/). |
| [getAccessibilityExtractContent()](#getAccessibilityExtractContent--)| <b>@deprecated.</b> Please use the 'accessibilityExtractContent' property instead. Indicates whether to allow to extract text and graphics (in support of accessibility to users with disabilities or for other purposes). |
| [setAccessibilityExtractContent(boolean)](#setAccessibilityExtractContent-boolean-)| <b>@deprecated.</b> Please use the 'accessibilityExtractContent' property instead. Indicates whether to allow to extract text and graphics (in support of accessibility to users with disabilities or for other purposes). |
| [getAssembleDocumentPermission()](#getAssembleDocumentPermission--)| <b>@deprecated.</b> Please use the 'assembleDocumentPermission' property instead. Indicates whether to allow to assemble the document (insert, rotate, or delete pages and create bookmarks or thumbnail images), even if [ModifyDocumentPermission](../modifydocumentpermission/) is clear. |
| [setAssembleDocumentPermission(boolean)](#setAssembleDocumentPermission-boolean-)| <b>@deprecated.</b> Please use the 'assembleDocumentPermission' property instead. Indicates whether to allow to assemble the document (insert, rotate, or delete pages and create bookmarks or thumbnail images), even if [ModifyDocumentPermission](../modifydocumentpermission/) is clear. |
| [getFullQualityPrintPermission()](#getFullQualityPrintPermission--)| <b>@deprecated.</b> Please use the 'fullQualityPrintPermission' property instead. Indicates whether to allow to print the document to a representation from which a faithful digital copy of the PDF content could be generated. |
| [setFullQualityPrintPermission(boolean)](#setFullQualityPrintPermission-boolean-)| <b>@deprecated.</b> Please use the 'fullQualityPrintPermission' property instead. Indicates whether to allow to print the document to a representation from which a faithful digital copy of the PDF content could be generated. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |
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
### getUserPassword() {#getUserPassword--}
```javascript
getUserPassword() : string;
```
**Remarks**
The owner password or user password will be required to open an encrypted PDF document for viewing.</p> <p>The user password can be null or empty string, in this case no password will be required from the user when opening the PDF document.</p> <p>Opening the document with the correct owner password allows full access to the document.</p> <p>Opening the document with the correct user password (or opening a document that does not have a user password) allows limited access as the permissions specified.
### setUserPassword(string) {#setUserPassword-string-}
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
```javascript
getOwnerPassword() : string;
```
**Remarks**
The owner password allows the user to open an encrypted PDF document without any access restrictions specified.
### setOwnerPassword(string) {#setOwnerPassword-string-}
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
```javascript
getPrintPermission() : boolean;
```
**Remarks**
Possibly not at the highest quality level, depending on whether [FullQualityPrintPermission](../fullqualityprintpermission/) is also set.
### setPrintPermission(boolean) {#setPrintPermission-boolean-}
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
```javascript
getModifyDocumentPermission() : boolean;
```
### setModifyDocumentPermission(boolean) {#setModifyDocumentPermission-boolean-}
```javascript
setModifyDocumentPermission(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### getAnnotationsPermission() {#getAnnotationsPermission--}
```javascript
getAnnotationsPermission() : boolean;
```
**Remarks**
if [ModifyDocumentPermission](../modifydocumentpermission/) is also set, create or modify interactive form fields (including signature fields).
### setAnnotationsPermission(boolean) {#setAnnotationsPermission-boolean-}
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
```javascript
getFillFormsPermission() : boolean;
```
### setFillFormsPermission(boolean) {#setFillFormsPermission-boolean-}
```javascript
setFillFormsPermission(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### getExtractContentPermission() {#getExtractContentPermission--}
```javascript
getExtractContentPermission() : boolean;
```
### setExtractContentPermission(boolean) {#setExtractContentPermission-boolean-}
```javascript
setExtractContentPermission(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### getAccessibilityExtractContent() {#getAccessibilityExtractContent--}
```javascript
getAccessibilityExtractContent() : boolean;
```
### setAccessibilityExtractContent(boolean) {#setAccessibilityExtractContent-boolean-}
```javascript
setAccessibilityExtractContent(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### getAssembleDocumentPermission() {#getAssembleDocumentPermission--}
```javascript
getAssembleDocumentPermission() : boolean;
```
### setAssembleDocumentPermission(boolean) {#setAssembleDocumentPermission-boolean-}
```javascript
setAssembleDocumentPermission(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### getFullQualityPrintPermission() {#getFullQualityPrintPermission--}
```javascript
getFullQualityPrintPermission() : boolean;
```
**Remarks**
When it is clear (and [PrintPermission](../printpermission/) is set), printing is limited to a low level representation of the appearance, possibly of degraded quality.
### setFullQualityPrintPermission(boolean) {#setFullQualityPrintPermission-boolean-}
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
