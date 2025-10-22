##DigitalSignatureCollection
Provides a collection of digital signatures attached to a document.
**Inheritance:**
java.lang.Object
**All Implemented Interfaces:**
java.lang.Iterable
```
public class DigitalSignatureCollection implements Iterable
```
Provides a collection of digital signatures attached to a document.
**Example**
The following example shows how to validate digital signature.
```
//workbook from a signed source file
Workbook signedWorkbook = new Workbook("signedFile.xlsx");
//wb.IsDigitallySigned is true when the workbook is signed already.
System.out.println(signedWorkbook.isDigitallySigned());
//get digitalSignature collection from workbook
DigitalSignatureCollection existingDsc = signedWorkbook.getDigitalSignature();
for (DigitalSignature existingDs : (Iterable<DigitalSignature>) existingDsc)
{
System.out.println(existingDs.getComments());
System.out.println(existingDs.getSignTime());
System.out.println(existingDs.isValid());
}
```
## Constructors
| Constructor | Description |
| --- | --- |
| [DigitalSignatureCollection()](#DigitalSignatureCollection--) | The constructor of DigitalSignatureCollection. |
## Methods
| Method | Description |
| --- | --- |
| [add(DigitalSignature digitalSignature)](#add-com.aspose.cells.DigitalSignature-) | Add one signature to DigitalSignatureCollection. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [hashCode()](#hashCode--) |  |
| [iterator()](#iterator--) | Get the enumerator for DigitalSignatureCollection, this enumerator allows iteration over the collection |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### DigitalSignatureCollection() {#DigitalSignatureCollection--}
```
public DigitalSignatureCollection()
```
The constructor of DigitalSignatureCollection.
### add(DigitalSignature digitalSignature) {#add-com.aspose.cells.DigitalSignature-}
```
public void add(DigitalSignature digitalSignature)
```
Add one signature to DigitalSignatureCollection.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| digitalSignature | [DigitalSignature](../../com.aspose.cells/digitalsignature) | Digital signature in collection. |
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
### hashCode() {#hashCode--}
```
public native int hashCode()
```
**Returns:**
int
### iterator() {#iterator--}
```
public Iterator iterator()
```
Get the enumerator for DigitalSignatureCollection, this enumerator allows iteration over the collection
**Returns:**
java.util.Iterator - The enumerator to iteration.
### notify() {#notify--}
```
public final native void notify()
```
### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```
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
