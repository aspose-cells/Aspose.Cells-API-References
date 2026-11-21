---
title: "GridAbstractCalculationEngine"
second_title: "Aspose.Cells for Java API Referansı"
description: "Kullanıcıların varsayılan Aspose.Cells hesaplama motorunu genişletmek için özel hesaplama motorunu temsil eder."
type: docs
url: /tr/java/com.aspose.gridweb/gridabstractcalculationengine/
---

**Inheritance:**
java.lang.Object
```
public abstract class GridAbstractCalculationEngine
```

Kullanıcının, Aspose.Cells'in varsayılan hesaplama motorunu genişletmek için özel hesaplama motorunu temsil eder.

**Example**

```
          class MyEngine extends GridAbstractCalculationEngine
         {
             public /*override*/ void calculate(GridCalculationData data)
             {
                 String funcName = data.getFunctionName().toUpperCase();
                 if ("MYFUNC".equals(funcName))
                 {
                     //do calculation for MYFUNC here
                     int count = data.getParamCount();
                     Object res = null;
                     for (int i = 0; i <count; i++)
                     {
                         Object pv = data.getParamValue(i);
                         if (pv instanceof GridReferredArea)
                         {
                             GridReferredArea ra = (GridReferredArea)pv;
                             pv = ra.getValue(0, 0);
                         }
                         //process the parameter here
                         //res = ...;
                     }
                     data.setCalculatedValue(res);
                 }
             }
         }
```
## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [GridAbstractCalculationEngine()](#GridAbstractCalculationEngine--) |  |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [calculate(GridCalculationData data)](#calculate-com.aspose.gridweb.GridCalculationData-) | Verilen verilerle bir işlevi hesaplar. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### GridAbstractCalculationEngine() {#GridAbstractCalculationEngine--}
```
public GridAbstractCalculationEngine()
```


### calculate(GridCalculationData data) {#calculate-com.aspose.gridweb.GridCalculationData-}
```
public abstract void calculate(GridCalculationData data)
```


Verilen verilerle bir işlevi hesaplar.

**Remarks**

Kullanıcı, bu uygulamada kendisi hesaplamak istediği tüm işlevler (excel yerel işlevleri dahil) için verilen verilerin hesaplanmış değerini ayarlamalıdır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| data | [GridCalculationData](../../com.aspose.gridweb/gridcalculationdata) | İşlev adını, parametreleri vb. gibi işlevi hesaplamak için gerekli veriler. |

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

