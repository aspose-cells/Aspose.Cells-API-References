##EncryptionType
Encryption Type.
**Inheritance:**
java.lang.Object
```
public final class EncryptionType
```
Encryption Type. Only used by excel2003. We will encrypt 2007/2010 workbook using SHA AES the same as Excel does, and this EncryptionType will be ignored.
## Fields
| Field | Description |
| --- | --- |
| [COMPATIBLE](#COMPATIBLE) | Office 97/2000 compatible. |
| [ENHANCED_CRYPTOGRAPHIC_PROVIDER_V_1](#ENHANCED-CRYPTOGRAPHIC-PROVIDER-V-1) | Enhanced encryption. |
| [STRONG_CRYPTOGRAPHIC_PROVIDER](#STRONG-CRYPTOGRAPHIC-PROVIDER) | Strong encryption algorithm. |
| [XOR](#XOR) | XOR encryption algorithm. |
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
### COMPATIBLE {#COMPATIBLE}
```
public static final int COMPATIBLE
```
Office 97/2000 compatible.
### ENHANCED_CRYPTOGRAPHIC_PROVIDER_V_1 {#ENHANCED-CRYPTOGRAPHIC-PROVIDER-V-1}
```
public static final int ENHANCED_CRYPTOGRAPHIC_PROVIDER_V_1
```
Enhanced encryption.
### STRONG_CRYPTOGRAPHIC_PROVIDER {#STRONG-CRYPTOGRAPHIC-PROVIDER}
```
public static final int STRONG_CRYPTOGRAPHIC_PROVIDER
```
Strong encryption algorithm.
### XOR {#XOR}
```
public static final int XOR
```
XOR encryption algorithm.
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
