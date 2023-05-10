---
title: PdfSecurityOptions
second_title: Aspose.Cells for Java API Reference
description: Settings of pdf when converting excel to pdf PDF/A does not allow security setting.
type: docs
url: /java/com.aspose.cells/pdfsecurityoptions/
---

**Inheritance:**
java.lang.Object
```
public class PdfSecurityOptions
```

Settings of pdf when converting excel to pdf, PDF/A does not allow security setting.
## Constructors

| Constructor | Description |
| --- | --- |
| [PdfSecurityOptions()](#PdfSecurityOptions--) | The constructor of PdfSecurityOptions
**Example**
The following code sets hight resolution print permisson for the output pdf. |
## Methods

| Method | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAccessibilityExtractContent()](#getAccessibilityExtractContent--) | Permission to copy or extract content (in support of accessibility to disabled users or for other purposes). |
| [getAnnotationsPermission()](#getAnnotationsPermission--) | Permission to comment on the document. |
| [getAssembleDocumentPermission()](#getAssembleDocumentPermission--) | Permission to insert, rotate, or delete pages and create bookmarks or thumbnail images even if ModifyDocumentPermission is not set. |
| [getClass()](#getClass--) |  |
| [getExtractContentPermission()](#getExtractContentPermission--) | Permission to copy or extract content. |
| [getExtractContentPermissionObsolete()](#getExtractContentPermissionObsolete--) | Permission to copy or extract content Obsoleted according to PDF reference. |
| [getFillFormsPermission()](#getFillFormsPermission--) | Permission to fill the form fields. |
| [getFullQualityPrintPermission()](#getFullQualityPrintPermission--) | Permission to print in high quality. |
| [getModifyDocumentPermission()](#getModifyDocumentPermission--) | Permission to modify pdf document |
| [getOwnerPassword()](#getOwnerPassword--) | Gets the owner password of the document |
| [getPrintPermission()](#getPrintPermission--) | Permission to print pdf document |
| [getUserPassword()](#getUserPassword--) | Gets the user password |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAccessibilityExtractContent(boolean value)](#setAccessibilityExtractContent-boolean-) | Permission to copy or extract content (in support of accessibility to disabled users or for other purposes). |
| [setAnnotationsPermission(boolean value)](#setAnnotationsPermission-boolean-) | Permission to comment on the document. |
| [setAssembleDocumentPermission(boolean value)](#setAssembleDocumentPermission-boolean-) | Permission to insert, rotate, or delete pages and create bookmarks or thumbnail images even if ModifyDocumentPermission is not set. |
| [setExtractContentPermission(boolean value)](#setExtractContentPermission-boolean-) | Permission to copy or extract content. |
| [setExtractContentPermissionObsolete(boolean value)](#setExtractContentPermissionObsolete-boolean-) | Permission to copy or extract content Obsoleted according to PDF reference. |
| [setFillFormsPermission(boolean value)](#setFillFormsPermission-boolean-) | Permission to fill the form fields. |
| [setFullQualityPrintPermission(boolean value)](#setFullQualityPrintPermission-boolean-) | Permission to print in high quality. |
| [setModifyDocumentPermission(boolean value)](#setModifyDocumentPermission-boolean-) | Permission to modify pdf document |
| [setOwnerPassword(String value)](#setOwnerPassword-java.lang.String-) | Sets the owner password of the document |
| [setPrintPermission(boolean value)](#setPrintPermission-boolean-) | Permission to print pdf document |
| [setUserPassword(String value)](#setUserPassword-java.lang.String-) | Sets the user password |
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
The following code sets hight resolution print permisson for the output pdf.

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


Permission to copy or extract content (in support of accessibility to disabled users or for other purposes).

**Returns:**
boolean
### getAnnotationsPermission() {#getAnnotationsPermission--}
```
public boolean getAnnotationsPermission()
```


Permission to comment on the document.

**Returns:**
boolean
### getAssembleDocumentPermission() {#getAssembleDocumentPermission--}
```
public boolean getAssembleDocumentPermission()
```


Permission to insert, rotate, or delete pages and create bookmarks or thumbnail images even if ModifyDocumentPermission is not set.

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


Permission to copy or extract content.

**Returns:**
boolean
### getExtractContentPermissionObsolete() {#getExtractContentPermissionObsolete--}
```
public boolean getExtractContentPermissionObsolete()
```


Permission to copy or extract content Obsoleted according to PDF reference.

**Returns:**
boolean
### getFillFormsPermission() {#getFillFormsPermission--}
```
public boolean getFillFormsPermission()
```


Permission to fill the form fields.

**Returns:**
boolean
### getFullQualityPrintPermission() {#getFullQualityPrintPermission--}
```
public boolean getFullQualityPrintPermission()
```


Permission to print in high quality.

**Returns:**
boolean
### getModifyDocumentPermission() {#getModifyDocumentPermission--}
```
public boolean getModifyDocumentPermission()
```


Permission to modify pdf document

**Returns:**
boolean
### getOwnerPassword() {#getOwnerPassword--}
```
public String getOwnerPassword()
```


Gets the owner password of the document

**Returns:**
java.lang.String
### getPrintPermission() {#getPrintPermission--}
```
public boolean getPrintPermission()
```


Permission to print pdf document

**Returns:**
boolean
### getUserPassword() {#getUserPassword--}
```
public String getUserPassword()
```


Gets the user password

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


Permission to copy or extract content (in support of accessibility to disabled users or for other purposes).

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setAnnotationsPermission(boolean value) {#setAnnotationsPermission-boolean-}
```
public void setAnnotationsPermission(boolean value)
```


Permission to comment on the document.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setAssembleDocumentPermission(boolean value) {#setAssembleDocumentPermission-boolean-}
```
public void setAssembleDocumentPermission(boolean value)
```


Permission to insert, rotate, or delete pages and create bookmarks or thumbnail images even if ModifyDocumentPermission is not set.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setExtractContentPermission(boolean value) {#setExtractContentPermission-boolean-}
```
public void setExtractContentPermission(boolean value)
```


Permission to copy or extract content.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setExtractContentPermissionObsolete(boolean value) {#setExtractContentPermissionObsolete-boolean-}
```
public void setExtractContentPermissionObsolete(boolean value)
```


Permission to copy or extract content Obsoleted according to PDF reference.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setFillFormsPermission(boolean value) {#setFillFormsPermission-boolean-}
```
public void setFillFormsPermission(boolean value)
```


Permission to fill the form fields.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setFullQualityPrintPermission(boolean value) {#setFullQualityPrintPermission-boolean-}
```
public void setFullQualityPrintPermission(boolean value)
```


Permission to print in high quality.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setModifyDocumentPermission(boolean value) {#setModifyDocumentPermission-boolean-}
```
public void setModifyDocumentPermission(boolean value)
```


Permission to modify pdf document

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setOwnerPassword(String value) {#setOwnerPassword-java.lang.String-}
```
public void setOwnerPassword(String value)
```


Sets the owner password of the document

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

### setPrintPermission(boolean value) {#setPrintPermission-boolean-}
```
public void setPrintPermission(boolean value)
```


Permission to print pdf document

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setUserPassword(String value) {#setUserPassword-java.lang.String-}
```
public void setUserPassword(String value)
```


Sets the user password

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

