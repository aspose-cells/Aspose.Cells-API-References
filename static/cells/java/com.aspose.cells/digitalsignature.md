##DigitalSignature
Signature in file.
**Inheritance:**
java.lang.Object
```
public class DigitalSignature
```
Signature in file.
## Constructors
| Constructor | Description |
| --- | --- |
| [DigitalSignature(KeyStore certificate, String privateKeyPassword, String comments, DateTime signTime)](#DigitalSignature-java.security.KeyStore-java.lang.String-java.lang.String-com.aspose.cells.DateTime-) | Constructor of digitalSignature. |
## Methods
| Method | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getCertificate()](#getCertificate--) | Certificate object that was used to sign the document. |
| [getClass()](#getClass--) |  |
| [getComments()](#getComments--) | The purpose to signature. |
| [getId()](#getId--) | Specifies a GUID which can be cross-referenced with the GUID of the signature line stored in the document content. |
| [getImage()](#getImage--) | Specifies an image for the digital signature. |
| [getProviderId()](#getProviderId--) | Specifies the class ID of the signature provider. |
| [getSignTime()](#getSignTime--) | The time when the document was signed. |
| [getText()](#getText--) | Specifies the text of actual signature in the digital signature. |
| [getXAdESType()](#getXAdESType--) | XAdES type. |
| [hashCode()](#hashCode--) |  |
| [isValid()](#isValid--) | If this digital signature is valid and the document has not been tampered with, this value will be true. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setCertificate(KeyStore value)](#setCertificate-java.security.KeyStore-) | Certificate object that was used to sign the document. |
| [setComments(String value)](#setComments-java.lang.String-) | The purpose to signature. |
| [setId(UUID value)](#setId-java.util.UUID-) | Specifies a GUID which can be cross-referenced with the GUID of the signature line stored in the document content. |
| [setImage(byte[] value)](#setImage-byte---) | Specifies an image for the digital signature. |
| [setProviderId(UUID value)](#setProviderId-java.util.UUID-) | Specifies the class ID of the signature provider. |
| [setSignTime(DateTime value)](#setSignTime-com.aspose.cells.DateTime-) | The time when the document was signed. |
| [setText(String value)](#setText-java.lang.String-) | Specifies the text of actual signature in the digital signature. |
| [setXAdESType(int value)](#setXAdESType-int-) | XAdES type. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### DigitalSignature(KeyStore certificate, String privateKeyPassword, String comments, DateTime signTime) {#DigitalSignature-java.security.KeyStore-java.lang.String-java.lang.String-com.aspose.cells.DateTime-}
```
public DigitalSignature(KeyStore certificate, String privateKeyPassword, String comments, DateTime signTime)
```
Constructor of digitalSignature.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| certificate | java.security.KeyStore | Certificate object that was used to sign the document. |
| privateKeyPassword | java.lang.String | The password for private key. |
| comments | java.lang.String | The purpose to signature. |
| signTime | [DateTime](../../com.aspose.cells/datetime) | The utc time when the document was signed. |
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
### getCertificate() {#getCertificate--}
```
public KeyStore getCertificate()
```
Certificate object that was used to sign the document.
**Returns:**
java.security.KeyStore
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```
**Returns:**
java.lang.Class<?>
### getComments() {#getComments--}
```
public String getComments()
```
The purpose to signature.
**Returns:**
java.lang.String
### getId() {#getId--}
```
public UUID getId()
```
Specifies a GUID which can be cross-referenced with the GUID of the signature line stored in the document content. Default value is Empty (all zeroes) Guid.
**Remarks**
When set, it associates [SignatureLine](../../com.aspose.cells/signatureline) with corresponding [DigitalSignature](../../com.aspose.cells/digitalsignature).
**Returns:**
java.util.UUID
### getImage() {#getImage--}
```
public byte[] getImage()
```
Specifies an image for the digital signature. Default value is null.
**Returns:**
byte[]
### getProviderId() {#getProviderId--}
```
public UUID getProviderId()
```
Specifies the class ID of the signature provider. Default value is Empty (all zeroes) Guid.
**Remarks**
The cryptographic service provider (CSP) is an independent software module that actually performs cryptography algorithms for authentication, encoding, and encryption. Microsoft Office reserves the value of \{00000000-0000-0000-0000-000000000000\} for its default signature provider, and \{000CD6A4-0000-0000-C000-000000000046\} for its East Asian signature provider. The GUID of the additionally installed provider should be obtained from the documentation shipped with the provider.
**Returns:**
java.util.UUID
### getSignTime() {#getSignTime--}
```
public DateTime getSignTime()
```
The time when the document was signed.
**Returns:**
[DateTime](../../com.aspose.cells/datetime)
### getText() {#getText--}
```
public String getText()
```
Specifies the text of actual signature in the digital signature. Default value is Empty.
**Returns:**
java.lang.String
### getXAdESType() {#getXAdESType--}
```
public int getXAdESType()
```
XAdES type. Default value is None(XAdES is off).
See [XAdESType](../../com.aspose.cells/xadestype).
**Returns:**
int
### hashCode() {#hashCode--}
```
public native int hashCode()
```
**Returns:**
int
### isValid() {#isValid--}
```
public boolean isValid()
```
If this digital signature is valid and the document has not been tampered with, this value will be true.
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
### setCertificate(KeyStore value) {#setCertificate-java.security.KeyStore-}
```
public void setCertificate(KeyStore value)
```
Certificate object that was used to sign the document.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.security.KeyStore |  |
### setComments(String value) {#setComments-java.lang.String-}
```
public void setComments(String value)
```
The purpose to signature.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |
### setId(UUID value) {#setId-java.util.UUID-}
```
public void setId(UUID value)
```
Specifies a GUID which can be cross-referenced with the GUID of the signature line stored in the document content. Default value is Empty (all zeroes) Guid.
**Remarks**
When set, it associates [SignatureLine](../../com.aspose.cells/signatureline) with corresponding [DigitalSignature](../../com.aspose.cells/digitalsignature).
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.util.UUID |  |
### setImage(byte[] value) {#setImage-byte---}
```
public void setImage(byte[] value)
```
Specifies an image for the digital signature. Default value is null.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | byte[] |  |
### setProviderId(UUID value) {#setProviderId-java.util.UUID-}
```
public void setProviderId(UUID value)
```
Specifies the class ID of the signature provider. Default value is Empty (all zeroes) Guid.
**Remarks**
The cryptographic service provider (CSP) is an independent software module that actually performs cryptography algorithms for authentication, encoding, and encryption. Microsoft Office reserves the value of \{00000000-0000-0000-0000-000000000000\} for its default signature provider, and \{000CD6A4-0000-0000-C000-000000000046\} for its East Asian signature provider. The GUID of the additionally installed provider should be obtained from the documentation shipped with the provider.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.util.UUID |  |
### setSignTime(DateTime value) {#setSignTime-com.aspose.cells.DateTime-}
```
public void setSignTime(DateTime value)
```
The time when the document was signed.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [DateTime](../../com.aspose.cells/datetime) |  |
### setText(String value) {#setText-java.lang.String-}
```
public void setText(String value)
```
Specifies the text of actual signature in the digital signature. Default value is Empty.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |
### setXAdESType(int value) {#setXAdESType-int-}
```
public void setXAdESType(int value)
```
XAdES type. Default value is None(XAdES is off).
See [XAdESType](../../com.aspose.cells/xadestype).
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |
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
