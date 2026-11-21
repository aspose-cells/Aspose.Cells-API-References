---
title: "AbstractCalculationMonitor"
second_title: "Aspose.Cells for Java API Referansı"
description: "Kullanıcının formül hesaplamasının ilerlemesini izleyebilmesi için izleme."
type: docs
url: /tr/java/com.aspose.cells/abstractcalculationmonitor/
---

**Inheritance:**
java.lang.Object
```
public abstract class AbstractCalculationMonitor
```

Kullanıcının formül hesaplamasının ilerlemesini izleyebilmesi için izleme.

**Example**

```
         class MyCalculationMonitor extends AbstractCalculationMonitor
         {
             public /*override*/ void beforeCalculate(int sheetIndex, int rowIndex, int colIndex)
             {
                 if(sheetIndex!=0 || rowIndex!=0 || colIndex!=0)
                 {
                     return;
                 }
                 System.out.println("Cell A1 will be calculated.");
             }
         }
         Workbook wb = new Workbook("calc.xlsx");
         CalculationOptions opts = new CalculationOptions();
         opts.setCalculationMonitor(new MyCalculationMonitor());
         wb.calculateFormula(opts);
```
## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [AbstractCalculationMonitor()](#AbstractCalculationMonitor--) |  |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [afterCalculate(int sheetIndex, int rowIndex, int colIndex)](#afterCalculate-int-int-int-) | Bu yöntemi, bir hücre hesaplandıktan sonra iş yapmak için uygulayın. |
| [beforeCalculate(int sheetIndex, int rowIndex, int colIndex)](#beforeCalculate-int-int-int-) | Bu yöntemi, bir hücre hesaplanmadan önce iş yapmak için uygulayın. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getCalculatedValue()](#getCalculatedValue--) | Hücrenin yeni hesaplanan değerini alır. |
| [getClass()](#getClass--) |  |
| [getOriginalValue()](#getOriginalValue--) | Hesaplanan hücrenin eski değerini alır. |
| [getValueChanged()](#getValueChanged--) | Hesaplamadan sonra hücrenin değerinin değişip değişmediği. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [onCircular(Iterator circularCellsData)](#onCircular-java.util.Iterator-) | Döngüsel referanslı formüller hesaplanırken iş yapmak için bu yöntemi uygulayın. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### AbstractCalculationMonitor() {#AbstractCalculationMonitor--}
```
public AbstractCalculationMonitor()
```


### afterCalculate(int sheetIndex, int rowIndex, int colIndex) {#afterCalculate-int-int-int-}
```
public void afterCalculate(int sheetIndex, int rowIndex, int colIndex)
```


Bu yöntemi, bir hücre hesaplandıktan sonra iş yapmak için uygulayın.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| sheetIndex | int | Hücrenin ait olduğu sayfanın indeksi. |
| rowIndex | int | Hücrenin satır indeksi |
| colIndex | int | Hücrenin sütun indeksi |

### beforeCalculate(int sheetIndex, int rowIndex, int colIndex) {#beforeCalculate-int-int-int-}
```
public void beforeCalculate(int sheetIndex, int rowIndex, int colIndex)
```


Bu yöntemi, bir hücre hesaplanmadan önce iş yapmak için uygulayın.

**Remarks**

Dizi formüllerindeki hücreler için bu yöntem genellikle hücrelerin birlikte hesaplanması nedeniyle çalıştırılamayabilir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| sheetIndex | int | Hücrenin ait olduğu sayfanın indeksi. |
| rowIndex | int | Hücrenin satır indeksi |
| colIndex | int | Hücrenin sütun indeksi |

### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| arg0 | java.lang.Object |  |

**Returns:**
boolean
### getCalculatedValue() {#getCalculatedValue--}
```
public Object getCalculatedValue()
```


Hücrenin yeni hesaplanmış değerini alır. Yalnızca [afterCalculate(int,int,int)](../../com.aspose.cells/abstractcalculationmonitor\#afterCalculate-int-int-int-) içinde kullanılmalıdır.

**Returns:**
java.lang.Object
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getOriginalValue() {#getOriginalValue--}
```
public Object getOriginalValue()
```


Hesaplanan hücrenin eski değerini alır. Yalnızca [beforeCalculate(int,int,int)](../../com.aspose.cells/abstractcalculationmonitor\#beforeCalculate-int-int-int-) ve [afterCalculate(int,int,int)](../../com.aspose.cells/abstractcalculationmonitor\#afterCalculate-int-int-int-) içinde kullanılmalıdır.

**Returns:**
java.lang.Object
### getValueChanged() {#getValueChanged--}
```
public boolean getValueChanged()
```


Hesaplamadan sonra hücrenin değerinin değişip değişmediği. Yalnızca [afterCalculate(int,int,int)](../../com.aspose.cells/abstractcalculationmonitor\#afterCalculate-int-int-int-) içinde kullanılmalıdır.

**Returns:**
boolean
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




### onCircular(Iterator circularCellsData) {#onCircular-java.util.Iterator-}
```
public boolean onCircular(Iterator circularCellsData)
```


Döngüsel referanslı formüller hesaplanırken iş yapmak için bu yöntemi uygulayın.

**Remarks**

Uygulamada kullanıcı, bu hücrelerin bir kısmı/ tamamı için beklenen değeri hesaplanmış sonuç olarak ayarlayabilir, böylece formül motoru onları yinelemeli olarak hesaplamaz.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| circularCellsData | java.util.Iterator | Döngüsel referanslara bağımlı hücreleri temsil eden [CalculationCell](../../com.aspose.cells/calculationcell) öğeleri içeren IEnumerator. |

**Returns:**
boolean - Bu çağrıdan sonra formül motorunun bu hücreleri döngüsel olarak hesaplaması gerekip gerekmediği. True ise formül motorunun hesaplamaya devam etmesine izin verir. False ise formül motorunun bu hücreleri sadece Hesaplanmış olarak işaretlemesine izin verir.
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
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

