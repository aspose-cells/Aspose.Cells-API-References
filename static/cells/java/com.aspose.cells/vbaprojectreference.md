##VbaProjectReference
Represents the reference of VBA project.
**Inheritance:**
java.lang.Object
```
public class VbaProjectReference
```
Represents the reference of VBA project.
**Example**
```
//Instantiating a Workbook object
Workbook workbook = new Workbook();
// Init VBA project.
VbaProject vbaProject = workbook.getVbaProject();
// Add vba project reference
vbaProject.getReferences().addRegisteredReference("stdole", "*\\G{00020430-0000-0000-C000-000000000046}#2.0#0#C:\\Windows\\system32\\stdole2.tlb#OLE Automation");
//Saving the Excel file
workbook.save("book1.xlsm");
```
## Methods
| Method | Description |
| --- | --- |
| [copy(VbaProjectReference source)](#copy-com.aspose.cells.VbaProjectReference-) |  |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getExtendedLibid()](#getExtendedLibid--) | Gets the extended Libid of the reference. |
| [getLibid()](#getLibid--) | Gets the Libid of the reference. |
| [getName()](#getName--) | Gets the name of the reference. |
| [getRelativeLibid()](#getRelativeLibid--) | Gets the referenced VBA project's identifier with an relative path. |
| [getTwiddledlibid()](#getTwiddledlibid--) | Gets the twiddled Libid of the reference. |
| [getType()](#getType--) | Gets the type of this reference. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setExtendedLibid(String value)](#setExtendedLibid-java.lang.String-) | Sets the extended Libid of the reference. |
| [setLibid(String value)](#setLibid-java.lang.String-) | Sets the Libid of the reference. |
| [setName(String value)](#setName-java.lang.String-) | Sets the name of the reference. |
| [setRelativeLibid(String value)](#setRelativeLibid-java.lang.String-) | Sets the referenced VBA project's identifier with an relative path. |
| [setTwiddledlibid(String value)](#setTwiddledlibid-java.lang.String-) | Sets the twiddled Libid of the reference. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### copy(VbaProjectReference source) {#copy-com.aspose.cells.VbaProjectReference-}
```
public void copy(VbaProjectReference source)
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| source | [VbaProjectReference](../../com.aspose.cells/vbaprojectreference) |  |
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
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```
**Returns:**
java.lang.Class<?>
### getExtendedLibid() {#getExtendedLibid--}
```
public String getExtendedLibid()
```
Gets the extended Libid of the reference.
**Remarks**
Only for control reference.
**Returns:**
java.lang.String
### getLibid() {#getLibid--}
```
public String getLibid()
```
Gets the Libid of the reference.
**Returns:**
java.lang.String
### getName() {#getName--}
```
public String getName()
```
Gets the name of the reference.
**Returns:**
java.lang.String
### getRelativeLibid() {#getRelativeLibid--}
```
public String getRelativeLibid()
```
Gets the referenced VBA project's identifier with an relative path.
**Remarks**
Only for project reference.
**Returns:**
java.lang.String
### getTwiddledlibid() {#getTwiddledlibid--}
```
public String getTwiddledlibid()
```
Gets the twiddled Libid of the reference.
**Remarks**
Only for control reference.
**Returns:**
java.lang.String
### getType() {#getType--}
```
public int getType()
```
Gets the type of this reference.
See [VbaProjectReferenceType](../../com.aspose.cells/vbaprojectreferencetype).
**Returns:**
int
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
### setExtendedLibid(String value) {#setExtendedLibid-java.lang.String-}
```
public void setExtendedLibid(String value)
```
Sets the extended Libid of the reference.
**Remarks**
Only for control reference.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |
### setLibid(String value) {#setLibid-java.lang.String-}
```
public void setLibid(String value)
```
Sets the Libid of the reference.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |
### setName(String value) {#setName-java.lang.String-}
```
public void setName(String value)
```
Sets the name of the reference.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |
### setRelativeLibid(String value) {#setRelativeLibid-java.lang.String-}
```
public void setRelativeLibid(String value)
```
Sets the referenced VBA project's identifier with an relative path.
**Remarks**
Only for project reference.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |
### setTwiddledlibid(String value) {#setTwiddledlibid-java.lang.String-}
```
public void setTwiddledlibid(String value)
```
Sets the twiddled Libid of the reference.
**Remarks**
Only for control reference.
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
