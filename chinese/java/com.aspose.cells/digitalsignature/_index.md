---
title: "数字签名"
second_title: "Aspose.Cells for Java API 参考"
description: "文件中的签名。"
type: docs
url: /zh/java/com.aspose.cells/digitalsignature/
---

**Inheritance:**
java.lang.Object
```
public class DigitalSignature
```

文件中的签名。
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [DigitalSignature(KeyStore certificate, String privateKeyPassword, String comments, DateTime signTime)](#DigitalSignature-java.security.KeyStore-java.lang.String-java.lang.String-com.aspose.cells.DateTime-) | digitalSignature 的构造函数。 |
## 方法

| 方法 | 描述 |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getCertificate()](#getCertificate--) | 用于签署文档的证书对象。 |
| [getClass()](#getClass--) |  |
| [getComments()](#getComments--) | 签名的目的。 |
| [getId()](#getId--) | 指定一个 GUID，可与文档内容中存储的签名行的 GUID 交叉引用。 |
| [getImage()](#getImage--) | 指定数字签名的图像。 |
| [getProviderId()](#getProviderId--) | 指定签名提供程序的类 ID。 |
| [getSignTime()](#getSignTime--) | 文档签署的时间。 |
| [getText()](#getText--) | 指定数字签名中实际签名的文本。 |
| [getXAdESType()](#getXAdESType--) | XAdES 类型。 |
| [hashCode()](#hashCode--) |  |
| [isValid()](#isValid--) | 如果此数字签名有效且文档未被篡改，则此值为 true。 |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setCertificate(KeyStore value)](#setCertificate-java.security.KeyStore-) | 用于签署文档的证书对象。 |
| [setComments(String value)](#setComments-java.lang.String-) | 签名的目的。 |
| [setId(UUID value)](#setId-java.util.UUID-) | 指定一个 GUID，可与文档内容中存储的签名行的 GUID 交叉引用。 |
| [setImage(byte[] value)](#setImage-byte---) | 指定数字签名的图像。 |
| [setProviderId(UUID value)](#setProviderId-java.util.UUID-) | 指定签名提供程序的类 ID。 |
| [setSignTime(DateTime value)](#setSignTime-com.aspose.cells.DateTime-) | 文档签署的时间。 |
| [setText(String value)](#setText-java.lang.String-) | 指定数字签名中实际签名的文本。 |
| [setXAdESType(int value)](#setXAdESType-int-) | XAdES 类型。 |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### DigitalSignature(KeyStore certificate, String privateKeyPassword, String comments, DateTime signTime) {#DigitalSignature-java.security.KeyStore-java.lang.String-java.lang.String-com.aspose.cells.DateTime-}
```
public DigitalSignature(KeyStore certificate, String privateKeyPassword, String comments, DateTime signTime)
```


digitalSignature 的构造函数。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 证书 | java.security.KeyStore | 用于签署文档的证书对象。 |
| privateKeyPassword | java.lang.String | 私钥的密码。 |
| 注释 | java.lang.String | 签名的目的。 |
| signTime | [DateTime](../../com.aspose.cells/datetime) | 文档签署时的 UTC 时间。 |

### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| arg0 | java.lang.Object |  |

**Returns:**
boolean
### getCertificate() {#getCertificate--}
```
public KeyStore getCertificate()
```


用于签署文档的证书对象。

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


签名的目的。

**Returns:**
java.lang.String
### getId() {#getId--}
```
public UUID getId()
```


指定一个 GUID，可与文档内容中存储的签名行的 GUID 进行交叉引用。默认值为全为零的 Empty GUID。

**Remarks**

设置后，它会将 [SignatureLine](../../com.aspose.cells/signatureline) 与相应的 [DigitalSignature](../../com.aspose.cells/digitalsignature) 关联。

**Returns:**
java.util.UUID
### getImage() {#getImage--}
```
public byte[] getImage()
```


指定数字签名的图像。默认值为 null。

**Returns:**
byte[]
### getProviderId() {#getProviderId--}
```
public UUID getProviderId()
```


指定签名提供程序的类 ID。默认值为全为零的 Empty GUID。

**Remarks**

加密服务提供程序 (CSP) 是一个独立的软件模块，实际执行用于身份验证、编码和加密的密码算法。Microsoft Office 为其默认签名提供程序保留值 \{00000000-0000-0000-0000-000000000000\}，为其东亚签名提供程序保留值 \{000CD6A4-0000-0000-C000-000000000046\}。额外安装的提供程序的 GUID 应从随该提供程序提供的文档中获取。

**Returns:**
java.util.UUID
### getSignTime() {#getSignTime--}
```
public DateTime getSignTime()
```


文档签署的时间。

**Returns:**
[DateTime](../../com.aspose.cells/datetime)
### getText() {#getText--}
```
public String getText()
```


指定数字签名中实际签名的文本。默认值为 Empty。

**Returns:**
java.lang.String
### getXAdESType() {#getXAdESType--}
```
public int getXAdESType()
```


XAdES 类型。默认值为 None（XAdES 已关闭）。

参见 [XAdESType](../../com.aspose.cells/xadestype)。

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


如果此数字签名有效且文档未被篡改，则此值为 true。

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


用于签署文档的证书对象。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.security.KeyStore |  |

### setComments(String value) {#setComments-java.lang.String-}
```
public void setComments(String value)
```


签名的目的。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setId(UUID value) {#setId-java.util.UUID-}
```
public void setId(UUID value)
```


指定一个 GUID，可与文档内容中存储的签名行的 GUID 进行交叉引用。默认值为全为零的 Empty GUID。

**Remarks**

设置后，它会将 [SignatureLine](../../com.aspose.cells/signatureline) 与相应的 [DigitalSignature](../../com.aspose.cells/digitalsignature) 关联。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.util.UUID |  |

### setImage(byte[] value) {#setImage-byte---}
```
public void setImage(byte[] value)
```


指定数字签名的图像。默认值为 null。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | byte[] |  |

### setProviderId(UUID value) {#setProviderId-java.util.UUID-}
```
public void setProviderId(UUID value)
```


指定签名提供程序的类 ID。默认值为全为零的 Empty GUID。

**Remarks**

加密服务提供程序 (CSP) 是一个独立的软件模块，实际执行用于身份验证、编码和加密的密码算法。Microsoft Office 为其默认签名提供程序保留值 \{00000000-0000-0000-0000-000000000000\}，为其东亚签名提供程序保留值 \{000CD6A4-0000-0000-C000-000000000046\}。额外安装的提供程序的 GUID 应从随该提供程序提供的文档中获取。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.util.UUID |  |

### setSignTime(DateTime value) {#setSignTime-com.aspose.cells.DateTime-}
```
public void setSignTime(DateTime value)
```


文档签署的时间。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [DateTime](../../com.aspose.cells/datetime) |  |

### setText(String value) {#setText-java.lang.String-}
```
public void setText(String value)
```


指定数字签名中实际签名的文本。默认值为 Empty。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setXAdESType(int value) {#setXAdESType-int-}
```
public void setXAdESType(int value)
```


XAdES 类型。默认值为 None（XAdES 已关闭）。

参见 [XAdESType](../../com.aspose.cells/xadestype)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

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
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

