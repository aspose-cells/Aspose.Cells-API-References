##AbstractLowCodeProtectionProvider
Implementation to provide protection settings
**Inheritance:**
java.lang.Object
```
public class AbstractLowCodeProtectionProvider
```
Implementation to provide protection settings
## Constructors
| Constructor | Description |
| --- | --- |
| [AbstractLowCodeProtectionProvider()](#AbstractLowCodeProtectionProvider--) |  |
## Methods
| Method | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getOpenPassword()](#getOpenPassword--) | Gets the password to open spread sheet file. |
| [getWorkbookPassword()](#getWorkbookPassword--) | Gets the password to protect the workbook with specified protection type. |
| [getWorkbookProtectionType()](#getWorkbookProtectionType--) | Gets the protection type to protect the workbook. |
| [getWorksheetPassword(String sheetName)](#getWorksheetPassword-java.lang.String-) | Gets the password to protect the specified worksheet. |
| [getWorksheetProtectionType(String sheetName)](#getWorksheetProtectionType-java.lang.String-) | Gets the protection type to protect the specified worksheet. |
| [getWritePassword()](#getWritePassword--) | Gets the password to modify spread sheet file. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### AbstractLowCodeProtectionProvider() {#AbstractLowCodeProtectionProvider--}
```
public AbstractLowCodeProtectionProvider()
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
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```
**Returns:**
java.lang.Class<?>
### getOpenPassword() {#getOpenPassword--}
```
public String getOpenPassword()
```
Gets the password to open spread sheet file.
**Returns:**
java.lang.String - Password to open spread sheet file. Empty means no protection for openning the filel.
### getWorkbookPassword() {#getWorkbookPassword--}
```
public String getWorkbookPassword()
```
Gets the password to protect the workbook with specified protection type.
**Returns:**
java.lang.String - Password to protect the workbook.
### getWorkbookProtectionType() {#getWorkbookProtectionType--}
```
public int getWorkbookProtectionType()
```
Gets the protection type to protect the workbook.
**Returns:**
int - [ProtectionType](../../com.aspose.cells/protectiontype). Protection type to protect the workbook. [ProtectionType.NONE](../../com.aspose.cells/protectiontype\#NONE) means no protection for the workbook.
### getWorksheetPassword(String sheetName) {#getWorksheetPassword-java.lang.String-}
```
public String getWorksheetPassword(String sheetName)
```
Gets the password to protect the specified worksheet.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sheetName | java.lang.String |  |
**Returns:**
java.lang.String - Password to protect the specified worksheet.
### getWorksheetProtectionType(String sheetName) {#getWorksheetProtectionType-java.lang.String-}
```
public int getWorksheetProtectionType(String sheetName)
```
Gets the protection type to protect the specified worksheet.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sheetName | java.lang.String |  |
**Returns:**
int - [ProtectionType](../../com.aspose.cells/protectiontype). Protection type to protect the specified worksheet. [ProtectionType.NONE](../../com.aspose.cells/protectiontype\#NONE) means no protection for the worksheet.
### getWritePassword() {#getWritePassword--}
```
public String getWritePassword()
```
Gets the password to modify spread sheet file.
**Returns:**
java.lang.String - Password to modify the spread sheet file. Empty means no protection for modifying the file.
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
