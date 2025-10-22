##WriteProtection
Specifies write protection settings for a workbook.
**Inheritance:**
java.lang.Object
```
public class WriteProtection
```
Specifies write protection settings for a workbook.
## Methods
| Method | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAuthor()](#getAuthor--) | Gets the author. |
| [getClass()](#getClass--) |  |
| [getPassword()](#getPassword--) | Sets the protected password to modify the file. |
| [getRecommendReadOnly()](#getRecommendReadOnly--) | Indicates if the Read Only Recommended option is selected. |
| [hashCode()](#hashCode--) |  |
| [isWriteProtected()](#isWriteProtected--) | Indicates whether this workbook is write protected. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAuthor(String value)](#setAuthor-java.lang.String-) | Sets the author. |
| [setPassword(String value)](#setPassword-java.lang.String-) | Sets the protected password to modify the file. |
| [setRecommendReadOnly(boolean value)](#setRecommendReadOnly-boolean-) | Indicates if the Read Only Recommended option is selected. |
| [toString()](#toString--) |  |
| [validatePassword(String password)](#validatePassword-java.lang.String-) | Returns true if the specified password is the same as the write-protection password the file was protected with. |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
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
### getAuthor() {#getAuthor--}
```
public String getAuthor()
```
Gets the author.
**Returns:**
java.lang.String
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```
**Returns:**
java.lang.Class<?>
### getPassword() {#getPassword--}
```
public String getPassword()
```
Sets the protected password to modify the file.
**Remarks**
**Returns:**
java.lang.String
### getRecommendReadOnly() {#getRecommendReadOnly--}
```
public boolean getRecommendReadOnly()
```
Indicates if the Read Only Recommended option is selected.
**Returns:**
boolean
### hashCode() {#hashCode--}
```
public native int hashCode()
```
**Returns:**
int
### isWriteProtected() {#isWriteProtected--}
```
public boolean isWriteProtected()
```
Indicates whether this workbook is write protected.
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
### setAuthor(String value) {#setAuthor-java.lang.String-}
```
public void setAuthor(String value)
```
Sets the author.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |
### setPassword(String value) {#setPassword-java.lang.String-}
```
public void setPassword(String value)
```
Sets the protected password to modify the file.
**Remarks**
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |
### setRecommendReadOnly(boolean value) {#setRecommendReadOnly-boolean-}
```
public void setRecommendReadOnly(boolean value)
```
Indicates if the Read Only Recommended option is selected.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
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
Returns true if the specified password is the same as the write-protection password the file was protected with.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| password | java.lang.String | The specified password. |
**Returns:**
boolean -
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
