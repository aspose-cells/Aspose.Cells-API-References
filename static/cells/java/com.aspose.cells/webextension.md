##WebExtension
Represents an Office Add-in instance.
**Inheritance:**
java.lang.Object
```
public class WebExtension
```
Represents an Office Add-in instance.
## Methods
| Method | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAlterReferences()](#getAlterReferences--) | Gets a list of alter references. |
| [getBindings()](#getBindings--) | Gets all bindings relationship between an Office Add-in and the data in the document. |
| [getClass()](#getClass--) |  |
| [getId()](#getId--) | Gets the uniquely identifies the Office Add-in instance in the current document. |
| [getProperties()](#getProperties--) | Gets all properties of web extension. |
| [getReference()](#getReference--) | Get the primary reference to an Office Add-in. |
| [hashCode()](#hashCode--) |  |
| [isFrozen()](#isFrozen--) | Indicates whether the user can interact with the Office Add-in or not. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setFrozen(boolean value)](#setFrozen-boolean-) | Indicates whether the user can interact with the Office Add-in or not. |
| [setId(String value)](#setId-java.lang.String-) | Sets the uniquely identifies the Office Add-in instance in the current document. |
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
### getAlterReferences() {#getAlterReferences--}
```
public WebExtensionReferenceCollection getAlterReferences()
```
Gets a list of alter references.
**Returns:**
[WebExtensionReferenceCollection](../../com.aspose.cells/webextensionreferencecollection)
### getBindings() {#getBindings--}
```
public WebExtensionBindingCollection getBindings()
```
Gets all bindings relationship between an Office Add-in and the data in the document.
**Returns:**
[WebExtensionBindingCollection](../../com.aspose.cells/webextensionbindingcollection)
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```
**Returns:**
java.lang.Class<?>
### getId() {#getId--}
```
public String getId()
```
Gets the uniquely identifies the Office Add-in instance in the current document.
**Returns:**
java.lang.String
### getProperties() {#getProperties--}
```
public WebExtensionPropertyCollection getProperties()
```
Gets all properties of web extension.
**Returns:**
[WebExtensionPropertyCollection](../../com.aspose.cells/webextensionpropertycollection)
### getReference() {#getReference--}
```
public WebExtensionReference getReference()
```
Get the primary reference to an Office Add-in.
**Returns:**
[WebExtensionReference](../../com.aspose.cells/webextensionreference)
### hashCode() {#hashCode--}
```
public native int hashCode()
```
**Returns:**
int
### isFrozen() {#isFrozen--}
```
public boolean isFrozen()
```
Indicates whether the user can interact with the Office Add-in or not.
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
### setFrozen(boolean value) {#setFrozen-boolean-}
```
public void setFrozen(boolean value)
```
Indicates whether the user can interact with the Office Add-in or not.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setId(String value) {#setId-java.lang.String-}
```
public void setId(String value)
```
Sets the uniquely identifies the Office Add-in instance in the current document.
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
