##HeaderFooterCommand
Represents the command of header/footer
**Inheritance:**
java.lang.Object
```
public class HeaderFooterCommand
```
Represents the command of header/footer
## Methods
| Method | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getFont()](#getFont--) | Gets the font of the command's value. |
| [getText()](#getText--) | Gets the text of the command. |
| [getType()](#getType--) | Gets the header/footer' command type . |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [toString()](#toString--) |  |
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
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```
**Returns:**
java.lang.Class<?>
### getFont() {#getFont--}
```
public Font getFont()
```
Gets the font of the command's value.
**Remarks**
Useless for HeaderFooterCommandType.Picture.
**Returns:**
[Font](../../com.aspose.cells/font)
### getText() {#getText--}
```
public String getText()
```
Gets the text of the command.
**Remarks**
Only valid for HeaderFooterCommandType.Text.
**Returns:**
java.lang.String
### getType() {#getType--}
```
public int getType()
```
Gets the header/footer' command type .
See [HeaderFooterCommandType](../../com.aspose.cells/headerfootercommandtype).
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
