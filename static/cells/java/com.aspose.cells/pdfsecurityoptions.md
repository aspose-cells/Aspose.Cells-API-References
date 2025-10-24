##PdfSecurityOptions
Options for encrypting and access permissions for a PDF document.
**Inheritance:**
java.lang.Object
```
public class PdfSecurityOptions
```
Options for encrypting and access permissions for a PDF document. PDF/A does not allow security setting.
## Constructors
| Constructor | Description |
| --- | --- |
| [PdfSecurityOptions()](#PdfSecurityOptions--) | The constructor of PdfSecurityOptions |
## Methods
| Method | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAccessibilityExtractContent()](#getAccessibilityExtractContent--) | Indicates whether to allow to extract text and graphics (in support of accessibility to users with disabilities or for other purposes). |
| [getAnnotationsPermission()](#getAnnotationsPermission--) | Indicates whether to allow to add or modify text annotations, fill in interactive form fields. |
| [getAssembleDocumentPermission()](#getAssembleDocumentPermission--) | Indicates whether to allow to assemble the document (insert, rotate, or delete pages and create bookmarks or thumbnail images), even if [getModifyDocumentPermission()](../../com.aspose.cells/pdfsecurityoptions\#getModifyDocumentPermission--) is clear. |
| [getClass()](#getClass--) |  |
| [getExtractContentPermission()](#getExtractContentPermission--) | Indicates whether to allow to copy or otherwise extract text and graphics from the document by operations other than that controlled by [getAccessibilityExtractContent()](../../com.aspose.cells/pdfsecurityoptions\#getAccessibilityExtractContent--). |
| [getExtractContentPermissionObsolete()](#getExtractContentPermissionObsolete--) | Permission to copy or extract content Obsoleted according to PDF reference. |
| [getFillFormsPermission()](#getFillFormsPermission--) | Indicates whether to allow to fill in existing interactive form fields (including signature fields), even if [getModifyDocumentPermission()](../../com.aspose.cells/pdfsecurityoptions\#getModifyDocumentPermission--) is clear. |
| [getFullQualityPrintPermission()](#getFullQualityPrintPermission--) | Indicates whether to allow to print the document to a representation from which a faithful digital copy of the PDF content could be generated. |
| [getModifyDocumentPermission()](#getModifyDocumentPermission--) | Indicates whether to allow to modify the contents of the document by operations other than those controlled by [getAnnotationsPermission()](../../com.aspose.cells/pdfsecurityoptions\#getAnnotationsPermission--), [getFillFormsPermission()](../../com.aspose.cells/pdfsecurityoptions\#getFillFormsPermission--) and [getAssembleDocumentPermission()](../../com.aspose.cells/pdfsecurityoptions\#getAssembleDocumentPermission--). |
| [getOwnerPassword()](#getOwnerPassword--) | Gets the owner password for the encrypted PDF document. |
| [getPrintPermission()](#getPrintPermission--) | Indicates whether to allow to print the document. |
| [getUserPassword()](#getUserPassword--) | Gets the user password required for opening the encrypted PDF document. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAccessibilityExtractContent(boolean value)](#setAccessibilityExtractContent-boolean-) | Indicates whether to allow to extract text and graphics (in support of accessibility to users with disabilities or for other purposes). |
| [setAnnotationsPermission(boolean value)](#setAnnotationsPermission-boolean-) | Indicates whether to allow to add or modify text annotations, fill in interactive form fields. |
| [setAssembleDocumentPermission(boolean value)](#setAssembleDocumentPermission-boolean-) | Indicates whether to allow to assemble the document (insert, rotate, or delete pages and create bookmarks or thumbnail images), even if [getModifyDocumentPermission()](../../com.aspose.cells/pdfsecurityoptions\#getModifyDocumentPermission--) is clear. |
| [setExtractContentPermission(boolean value)](#setExtractContentPermission-boolean-) | Indicates whether to allow to copy or otherwise extract text and graphics from the document by operations other than that controlled by [getAccessibilityExtractContent()](../../com.aspose.cells/pdfsecurityoptions\#getAccessibilityExtractContent--). |
| [setExtractContentPermissionObsolete(boolean value)](#setExtractContentPermissionObsolete-boolean-) | Permission to copy or extract content Obsoleted according to PDF reference. |
| [setFillFormsPermission(boolean value)](#setFillFormsPermission-boolean-) | Indicates whether to allow to fill in existing interactive form fields (including signature fields), even if [getModifyDocumentPermission()](../../com.aspose.cells/pdfsecurityoptions\#getModifyDocumentPermission--) is clear. |
| [setFullQualityPrintPermission(boolean value)](#setFullQualityPrintPermission-boolean-) | Indicates whether to allow to print the document to a representation from which a faithful digital copy of the PDF content could be generated. |
| [setModifyDocumentPermission(boolean value)](#setModifyDocumentPermission-boolean-) | Indicates whether to allow to modify the contents of the document by operations other than those controlled by [getAnnotationsPermission()](../../com.aspose.cells/pdfsecurityoptions\#getAnnotationsPermission--), [getFillFormsPermission()](../../com.aspose.cells/pdfsecurityoptions\#getFillFormsPermission--) and [getAssembleDocumentPermission()](../../com.aspose.cells/pdfsecurityoptions\#getAssembleDocumentPermission--). |
| [setOwnerPassword(String value)](#setOwnerPassword-java.lang.String-) | Sets the owner password for the encrypted PDF document. |
| [setPrintPermission(boolean value)](#setPrintPermission-boolean-) | Indicates whether to allow to print the document. |
| [setUserPassword(String value)](#setUserPassword-java.lang.String-) | Sets the user password required for opening the encrypted PDF document. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### PdfSecurityOptions() {#PdfSecurityOptions--}
```
public PdfSecurityOptions()
```
The constructor of PdfSecurityOptions
**Example**
The following code sets high resolution print permisson for the output pdf.
```
Workbook wb = new Workbook();
wb.getWorksheets().get(0).getCells().get("A1").setValue("Aspose");
PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
PdfSecurityOptions pdfSecurityOptions = new PdfSecurityOptions();
//set owner password
pdfSecurityOptions.setOwnerPassword("YourOwnerPassword");
//set user password
pdfSecurityOptions.setUserPassword("YourUserPassword");
//set print permisson
pdfSecurityOptions.setPrintPermission(true);
//set high resolution for print
pdfSecurityOptions.setFullQualityPrintPermission(true);
pdfSaveOptions.setSecurityOptions(pdfSecurityOptions);
wb.save("output.pdf", pdfSaveOptions);
```
### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| arg0 | java.lang.Object |  |
**Returns:**
boolean
### getAccessibilityExtractContent() {#getAccessibilityExtractContent--}
```
public boolean getAccessibilityExtractContent()
```
Indicates whether to allow to extract text and graphics (in support of accessibility to users with disabilities or for other purposes).
**Returns:**
boolean
### getAnnotationsPermission() {#getAnnotationsPermission--}
```
public boolean getAnnotationsPermission()
```
Indicates whether to allow to add or modify text annotations, fill in interactive form fields.
**Remarks**
if [getModifyDocumentPermission()](../../com.aspose.cells/pdfsecurityoptions\#getModifyDocumentPermission--) is also set, create or modify interactive form fields (including signature fields).
**Returns:**
boolean
### getAssembleDocumentPermission() {#getAssembleDocumentPermission--}
```
public boolean getAssembleDocumentPermission()
```
Indicates whether to allow to assemble the document (insert, rotate, or delete pages and create bookmarks or thumbnail images), even if [getModifyDocumentPermission()](../../com.aspose.cells/pdfsecurityoptions\#getModifyDocumentPermission--) is clear.
**Returns:**
boolean
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```
**Returns:**
java.lang.Class<?>
### getExtractContentPermission() {#getExtractContentPermission--}
```
public boolean getExtractContentPermission()
```
Indicates whether to allow to copy or otherwise extract text and graphics from the document by operations other than that controlled by [getAccessibilityExtractContent()](../../com.aspose.cells/pdfsecurityoptions\#getAccessibilityExtractContent--).
**Returns:**
boolean
### getExtractContentPermissionObsolete() {#getExtractContentPermissionObsolete--}
```
public boolean getExtractContentPermissionObsolete()
```
Permission to copy or extract content Obsoleted according to PDF reference.
**Remarks**
NOTE: This member is now obsolete. Instead, please use ExtractContentPermission property. This property will be removed 12 months later since September 2023. Aspose apologizes for any inconvenience you may have experienced.
**Returns:**
boolean
### getFillFormsPermission() {#getFillFormsPermission--}
```
public boolean getFillFormsPermission()
```
Indicates whether to allow to fill in existing interactive form fields (including signature fields), even if [getModifyDocumentPermission()](../../com.aspose.cells/pdfsecurityoptions\#getModifyDocumentPermission--) is clear.
**Returns:**
boolean
### getFullQualityPrintPermission() {#getFullQualityPrintPermission--}
```
public boolean getFullQualityPrintPermission()
```
Indicates whether to allow to print the document to a representation from which a faithful digital copy of the PDF content could be generated.
**Remarks**
When it is clear (and [getPrintPermission()](../../com.aspose.cells/pdfsecurityoptions\#getPrintPermission--) is set), printing is limited to a low level representation of the appearance, possibly of degraded quality.
**Returns:**
boolean
### getModifyDocumentPermission() {#getModifyDocumentPermission--}
```
public boolean getModifyDocumentPermission()
```
Indicates whether to allow to modify the contents of the document by operations other than those controlled by [getAnnotationsPermission()](../../com.aspose.cells/pdfsecurityoptions\#getAnnotationsPermission--), [getFillFormsPermission()](../../com.aspose.cells/pdfsecurityoptions\#getFillFormsPermission--) and [getAssembleDocumentPermission()](../../com.aspose.cells/pdfsecurityoptions\#getAssembleDocumentPermission--).
**Returns:**
boolean
### getOwnerPassword() {#getOwnerPassword--}
```
public String getOwnerPassword()
```
Gets the owner password for the encrypted PDF document.
**Remarks**
The owner password allows the user to open an encrypted PDF document without any access restrictions specified.
**Returns:**
java.lang.String
### getPrintPermission() {#getPrintPermission--}
```
public boolean getPrintPermission()
```
Indicates whether to allow to print the document.
**Remarks**
Possibly not at the highest quality level, depending on whether [getFullQualityPrintPermission()](../../com.aspose.cells/pdfsecurityoptions\#getFullQualityPrintPermission--) is also set.
**Returns:**
boolean
### getUserPassword() {#getUserPassword--}
```
public String getUserPassword()
```
Gets the user password required for opening the encrypted PDF document.
**Remarks**
The owner password or user password will be required to open an encrypted PDF document for viewing.
The user password can be null or empty string, in this case no password will be required from the user when opening the PDF document.
Opening the document with the correct owner password allows full access to the document.
Opening the document with the correct user password (or opening a document that does not have a user password) allows limited access as the permissions specified.
**Returns:**
java.lang.String
### hashCode() {#hashCode--}
```
public native int hashCode()
```
**Returns:**
int
### notify() {#notify--}
```
public final native void notify()
```
### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```
### setAccessibilityExtractContent(boolean value) {#setAccessibilityExtractContent-boolean-}
```
public void setAccessibilityExtractContent(boolean value)
```
Indicates whether to allow to extract text and graphics (in support of accessibility to users with disabilities or for other purposes).
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setAnnotationsPermission(boolean value) {#setAnnotationsPermission-boolean-}
```
public void setAnnotationsPermission(boolean value)
```
Indicates whether to allow to add or modify text annotations, fill in interactive form fields.
**Remarks**
if [getModifyDocumentPermission()](../../com.aspose.cells/pdfsecurityoptions\#getModifyDocumentPermission--) is also set, create or modify interactive form fields (including signature fields).
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setAssembleDocumentPermission(boolean value) {#setAssembleDocumentPermission-boolean-}
```
public void setAssembleDocumentPermission(boolean value)
```
Indicates whether to allow to assemble the document (insert, rotate, or delete pages and create bookmarks or thumbnail images), even if [getModifyDocumentPermission()](../../com.aspose.cells/pdfsecurityoptions\#getModifyDocumentPermission--) is clear.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setExtractContentPermission(boolean value) {#setExtractContentPermission-boolean-}
```
public void setExtractContentPermission(boolean value)
```
Indicates whether to allow to copy or otherwise extract text and graphics from the document by operations other than that controlled by [getAccessibilityExtractContent()](../../com.aspose.cells/pdfsecurityoptions\#getAccessibilityExtractContent--).
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setExtractContentPermissionObsolete(boolean value) {#setExtractContentPermissionObsolete-boolean-}
```
public void setExtractContentPermissionObsolete(boolean value)
```
Permission to copy or extract content Obsoleted according to PDF reference.
**Remarks**
NOTE: This member is now obsolete. Instead, please use ExtractContentPermission property. This property will be removed 12 months later since September 2023. Aspose apologizes for any inconvenience you may have experienced.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setFillFormsPermission(boolean value) {#setFillFormsPermission-boolean-}
```
public void setFillFormsPermission(boolean value)
```
Indicates whether to allow to fill in existing interactive form fields (including signature fields), even if [getModifyDocumentPermission()](../../com.aspose.cells/pdfsecurityoptions\#getModifyDocumentPermission--) is clear.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setFullQualityPrintPermission(boolean value) {#setFullQualityPrintPermission-boolean-}
```
public void setFullQualityPrintPermission(boolean value)
```
Indicates whether to allow to print the document to a representation from which a faithful digital copy of the PDF content could be generated.
**Remarks**
When it is clear (and [getPrintPermission()](../../com.aspose.cells/pdfsecurityoptions\#getPrintPermission--) is set), printing is limited to a low level representation of the appearance, possibly of degraded quality.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setModifyDocumentPermission(boolean value) {#setModifyDocumentPermission-boolean-}
```
public void setModifyDocumentPermission(boolean value)
```
Indicates whether to allow to modify the contents of the document by operations other than those controlled by [getAnnotationsPermission()](../../com.aspose.cells/pdfsecurityoptions\#getAnnotationsPermission--), [getFillFormsPermission()](../../com.aspose.cells/pdfsecurityoptions\#getFillFormsPermission--) and [getAssembleDocumentPermission()](../../com.aspose.cells/pdfsecurityoptions\#getAssembleDocumentPermission--).
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setOwnerPassword(String value) {#setOwnerPassword-java.lang.String-}
```
public void setOwnerPassword(String value)
```
Sets the owner password for the encrypted PDF document.
**Remarks**
The owner password allows the user to open an encrypted PDF document without any access restrictions specified.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |
### setPrintPermission(boolean value) {#setPrintPermission-boolean-}
```
public void setPrintPermission(boolean value)
```
Indicates whether to allow to print the document.
**Remarks**
Possibly not at the highest quality level, depending on whether [getFullQualityPrintPermission()](../../com.aspose.cells/pdfsecurityoptions\#getFullQualityPrintPermission--) is also set.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setUserPassword(String value) {#setUserPassword-java.lang.String-}
```
public void setUserPassword(String value)
```
Sets the user password required for opening the encrypted PDF document.
**Remarks**
The owner password or user password will be required to open an encrypted PDF document for viewing.
The user password can be null or empty string, in this case no password will be required from the user when opening the PDF document.
Opening the document with the correct owner password allows full access to the document.
Opening the document with the correct user password (or opening a document that does not have a user password) allows limited access as the permissions specified.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |
### toString() {#toString--}
```
public String toString()
```
**Returns:**
java.lang.String
### wait() {#wait--}
```
public final void wait()
```
### wait(long arg0) {#wait-long-}
```
public final native void wait(long arg0)
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| arg0 | long |  |
### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |
