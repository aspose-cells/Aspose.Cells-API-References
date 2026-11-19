---
title: "计量"
second_title: "Aspose.Cells for Java API 参考"
description: "提供设置计量键的方法。"
type: docs
url: /zh/java/com.aspose.cells/metered/
---

**Inheritance:**
java.lang.Object
```
public class Metered
```

提供设置计量键的方法。
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [Metered()](#Metered--) | 初始化此类的新实例。 |
## 方法

| 方法 | 描述 |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getConsumptionCredit()](#getConsumptionCredit--) | 获取消耗额度 |
| [getConsumptionQuantity()](#getConsumptionQuantity--) | 获取消耗文件大小 |
| [getProductName()](#getProductName--) | 获取产品名称 |
| [hashCode()](#hashCode--) |  |
| [isMeteredLicensed()](#isMeteredLicensed--) | 检查计量是否已授权 |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setMeteredKey(String publicKey, String privateKey)](#setMeteredKey-java.lang.String-java.lang.String-) | 设置计量的公钥和私钥。 |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### Metered() {#Metered--}
```
public Metered()
```


初始化此类的新实例。

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
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getConsumptionCredit() {#getConsumptionCredit--}
```
public static double getConsumptionCredit()
```


获取消耗额度

**Returns:**
double - 消耗数量
### getConsumptionQuantity() {#getConsumptionQuantity--}
```
public static double getConsumptionQuantity()
```


获取消耗文件大小

**Returns:**
double - 消耗数量
### getProductName() {#getProductName--}
```
public String getProductName()
```


获取产品名称

**Returns:**
java.lang.String - 产品名称
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isMeteredLicensed() {#isMeteredLicensed--}
```
public static boolean isMeteredLicensed()
```


检查计量是否已授权

**Returns:**
布尔 - 真或假
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### setMeteredKey(String publicKey, String privateKey) {#setMeteredKey-java.lang.String-java.lang.String-}
```
public void setMeteredKey(String publicKey, String privateKey)
```


设置计量的公钥和私钥。如果您购买了计量许可证，在启动应用程序时应调用此 API，通常这已足够。然而，如果始终无法上传消费数据且超过 24 小时，许可证将被设置为评估状态，为避免此情况，您应定期检查许可证状态，如果是评估状态，请再次调用此 API。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| publicKey | java.lang.String | 公钥 |
| privateKey | java.lang.String | 私钥 |

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

