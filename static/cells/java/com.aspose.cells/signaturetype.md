##SignatureType
Specifies the signature type.
**Inheritance:**
java.lang.Object
```
public final class SignatureType
```
Specifies the signature type.
## Fields
| Field | Description |
| --- | --- |
| [CUSTOM](#CUSTOM) | The corresponding ProviderId value usually needs to be set by the user. it should be obtained from the documentation shipped with the provider. |
| [DEFAULT](#DEFAULT) | The default value , the corresponding ProviderId value is fixed to \{0000000000-0000-0000-0000-0000000000\}. |
| [STAMP](#STAMP) | The corresponding ProviderId value is usually \{000CD6A4-0000-0000-C000-000000000046\}. |
## Methods
| Method | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### CUSTOM {#CUSTOM}
```
public static final int CUSTOM
```
The corresponding ProviderId value usually needs to be set by the user. it should be obtained from the documentation shipped with the provider.
### DEFAULT {#DEFAULT}
```
public static final int DEFAULT
```
The default value , the corresponding ProviderId value is fixed to \{0000000000-0000-0000-0000-0000000000\}.
### STAMP {#STAMP}
```
public static final int STAMP
```
The corresponding ProviderId value is usually \{000CD6A4-0000-0000-C000-000000000046\}.
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
