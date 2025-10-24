##VbaProject
Represents the VBA project.
**Inheritance:**
java.lang.Object
```
public class VbaProject
```
Represents the VBA project.
**Example**
```
//Instantiating a Workbook object
Workbook workbook = new Workbook();
// Init VBA project.
VbaProject vbaProject = workbook.getVbaProject();
//Saving the Excel file
workbook.save("book1.xlsm");
```
## Methods
| Method | Description |
| --- | --- |
| [copy(VbaProject source)](#copy-com.aspose.cells.VbaProject-) | Copy VBA project from other file. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getCertRawData()](#getCertRawData--) | Gets certificate raw data if this VBA project is signed. |
| [getClass()](#getClass--) |  |
| [getEncoding()](#getEncoding--) | Gets the encoding of VBA project. |
| [getIslockedForViewing()](#getIslockedForViewing--) | Indicates whether this VBA project is locked for viewing. |
| [getModules()](#getModules--) | Gets all [VbaModule](../../com.aspose.cells/vbamodule) objects. |
| [getName()](#getName--) | Gets the name of the VBA project. |
| [getReferences()](#getReferences--) | Gets all references of VBA project. |
| [hashCode()](#hashCode--) |  |
| [isProtected()](#isProtected--) | Indicates whether this VBA project is protected. |
| [isSigned()](#isSigned--) | Indicates whether VBAcode is signed or not. |
| [isValidSigned()](#isValidSigned--) | Indicates whether the signature of VBA project is valid or not. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [protect(boolean islockedForViewing, String password)](#protect-boolean-java.lang.String-) | Protects or unprotects this VBA project. |
| [setEncoding(Encoding value)](#setEncoding-com.aspose.cells.Encoding-) | Sets the encoding of VBA project. |
| [setName(String value)](#setName-java.lang.String-) | Sets the name of the VBA project. |
| [sign(DigitalSignature digitalSignature)](#sign-com.aspose.cells.DigitalSignature-) | Sign this VBA project by a DigitalSignature |
| [toString()](#toString--) |  |
| [validatePassword(String password)](#validatePassword-java.lang.String-) | Validates protection password. |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### copy(VbaProject source) {#copy-com.aspose.cells.VbaProject-}
```
public void copy(VbaProject source)
```
Copy VBA project from other file.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| source | [VbaProject](../../com.aspose.cells/vbaproject) |  |
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
### getCertRawData() {#getCertRawData--}
```
public byte[] getCertRawData()
```
Gets certificate raw data if this VBA project is signed.
**Returns:**
byte[]
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```
**Returns:**
java.lang.Class<?>
### getEncoding() {#getEncoding--}
```
public Encoding getEncoding()
```
Gets the encoding of VBA project.
**Returns:**
[Encoding](../../com.aspose.cells/encoding)
### getIslockedForViewing() {#getIslockedForViewing--}
```
public boolean getIslockedForViewing()
```
Indicates whether this VBA project is locked for viewing.
**Returns:**
boolean
### getModules() {#getModules--}
```
public VbaModuleCollection getModules()
```
Gets all [VbaModule](../../com.aspose.cells/vbamodule) objects.
**Returns:**
[VbaModuleCollection](../../com.aspose.cells/vbamodulecollection)
### getName() {#getName--}
```
public String getName()
```
Gets the name of the VBA project.
**Returns:**
java.lang.String
### getReferences() {#getReferences--}
```
public VbaProjectReferenceCollection getReferences()
```
Gets all references of VBA project.
**Returns:**
[VbaProjectReferenceCollection](../../com.aspose.cells/vbaprojectreferencecollection)
### hashCode() {#hashCode--}
```
public native int hashCode()
```
**Returns:**
int
### isProtected() {#isProtected--}
```
public boolean isProtected()
```
Indicates whether this VBA project is protected.
**Returns:**
boolean
### isSigned() {#isSigned--}
```
public boolean isSigned()
```
Indicates whether VBAcode is signed or not.
**Returns:**
boolean
### isValidSigned() {#isValidSigned--}
```
public boolean isValidSigned()
```
Indicates whether the signature of VBA project is valid or not.
**Returns:**
boolean
### notify() {#notify--}
```
public final native void notify()
```
### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```
### protect(boolean islockedForViewing, String password) {#protect-boolean-java.lang.String-}
```
public void protect(boolean islockedForViewing, String password)
```
Protects or unprotects this VBA project.
**Remarks**
If islockedForViewing is true, the password could not be null.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| islockedForViewing | boolean | indicates whether locks project for viewing. |
| password | java.lang.String | If the value is null, unprotects this VBA project, otherwise projects the this VBA project. |
### setEncoding(Encoding value) {#setEncoding-com.aspose.cells.Encoding-}
```
public void setEncoding(Encoding value)
```
Sets the encoding of VBA project.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [Encoding](../../com.aspose.cells/encoding) |  |
### setName(String value) {#setName-java.lang.String-}
```
public void setName(String value)
```
Sets the name of the VBA project.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |
### sign(DigitalSignature digitalSignature) {#sign-com.aspose.cells.DigitalSignature-}
```
public void sign(DigitalSignature digitalSignature)
```
Sign this VBA project by a DigitalSignature
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| digitalSignature | [DigitalSignature](../../com.aspose.cells/digitalsignature) | DigitalSignature |
### toString() {#toString--}
```
public String toString()
```
**Returns:**
java.lang.String
### validatePassword(String password) {#validatePassword-java.lang.String-}
```
public boolean validatePassword(String password)
```
Validates protection password.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| password | java.lang.String | the password |
**Returns:**
boolean - Whether password is the protection password of this VBA project
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
