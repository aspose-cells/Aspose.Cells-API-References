---
title: "مقاس"
second_title: "Aspose.Cells for Java API Reference"
description: "يوفر طرقًا لتعيين المفتاح المقاس."
type: docs
url: /ar/java/com.aspose.cells/metered/
---

**Inheritance:**
java.lang.Object
```
public class Metered
```

يوفر طرقًا لتعيين المفتاح المقاس.
## المنشئات

| منشئ | الوصف |
| --- | --- |
| [Metered()](#Metered--) | ينشئ مثيلاً جديداً لهذه الفئة. |
## الطرق

| طريقة | الوصف |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getConsumptionCredit()](#getConsumptionCredit--) | يحصل على رصيد الاستهلاك |
| [getConsumptionQuantity()](#getConsumptionQuantity--) | يحصل على حجم ملف الاستهلاك |
| [getProductName()](#getProductName--) | يحصل على اسم المنتج |
| [hashCode()](#hashCode--) |  |
| [isMeteredLicensed()](#isMeteredLicensed--) | تحقق مما إذا كان العداد مرخصًا |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setMeteredKey(String publicKey, String privateKey)](#setMeteredKey-java.lang.String-java.lang.String-) | يضبط المفتاح العام والخاص للعداد. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### Metered() {#Metered--}
```
public Metered()
```


ينشئ مثيلاً جديداً لهذه الفئة.

### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| معامل | نوع | الوصف |
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


يحصل على رصيد الاستهلاك

**Returns:**
double - كمية الاستهلاك
### getConsumptionQuantity() {#getConsumptionQuantity--}
```
public static double getConsumptionQuantity()
```


يحصل على حجم ملف الاستهلاك

**Returns:**
double - كمية الاستهلاك
### getProductName() {#getProductName--}
```
public String getProductName()
```


يحصل على اسم المنتج

**Returns:**
java.lang.String - اسم المنتج
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


تحقق مما إذا كان العداد مرخصًا

**Returns:**
boolean - صحيح أو خطأ
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


يضبط المفتاح العام والخاص للعداد. إذا قمت بشراء ترخيص عداد، عند بدء التطبيق يجب استدعاء هذه الواجهة البرمجية، عادةً يكون هذا كافيًا. ومع ذلك، إذا فشل دائمًا تحميل بيانات الاستهلاك وتجاوز 24 ساعة، سيتم ضبط الترخيص إلى حالة التقييم. لتجنب هذه الحالة، يجب عليك فحص حالة الترخيص بانتظام، إذا كانت في حالة التقييم، استدعِ هذه الواجهة البرمجية مرة أخرى.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| publicKey | java.lang.String | المفتاح العام |
| privateKey | java.lang.String | المفتاح الخاص |

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
| معامل | نوع | الوصف |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

