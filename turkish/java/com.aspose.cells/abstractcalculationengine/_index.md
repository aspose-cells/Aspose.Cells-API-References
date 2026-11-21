---
title: "AbstractCalculationEngine"
second_title: "Aspose.Cells for Java API Referansı"
description: "Kullanıcıların varsayılan Aspose.Cells hesaplama motorunu genişletmek için özel hesaplama motorunu temsil eder."
type: docs
url: /tr/java/com.aspose.cells/abstractcalculationengine/
---

**Inheritance:**
java.lang.Object
```
public abstract class AbstractCalculationEngine
```

Kullanıcının, Aspose.Cells'in varsayılan hesaplama motorunu genişletmek için özel hesaplama motorunu temsil eder.

**Remarks**

Kullanıcı, bu uygulamada Workbook'un herhangi bir bölümünü doğrudan değiştirmemelidir (özel işlevin hesaplanmış sonucu hariç, bu sonuç CalculationData.CalculatedValue özelliği ile ayarlanabilir). Aksi takdirde beklenmeyen sonuçlar veya Exception oluşabilir. Kullanıcı, bazı özel işlevler için hesaplanmış sonuç dışındaki diğer verileri (örneğin hücrenin formülünü, stilini, ... vb.) değiştirmesi gerekiyorsa, bu verileri bu uygulamada toplamalı ve formül hesaplamasının kapsamı dışına çıkararak değiştirmelidir.

**Example**

```
         class MyEngine extends AbstractCalculationEngine
         {
             public /*override*/ void calculate(CalculationData data)
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
                         if (pv instanceof ReferredArea)
                         {
                             ReferredArea ra = (ReferredArea)pv;
                             pv = ra.getValue(0, 0);
                         }
                         //process the parameter here
                         //res = ...;
                     }
                     data.setCalculatedValue(res);
                 }
             }
         }
         Workbook wb = new Workbook("custom_calc.xlsx");
         CalculationOptions opts = new CalculationOptions();
         opts.setCustomEngine(new MyEngine());
         wb.calculateFormula(opts);
```
## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [AbstractCalculationEngine()](#AbstractCalculationEngine--) |  |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [calculate(CalculationData data)](#calculate-com.aspose.cells.CalculationData-) | Verilen verilerle bir işlevi hesaplar. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [forceRecalculate(String functionName)](#forceRecalculate-java.lang.String-) | Paylaşılan formüller hesaplanırken verilen işlevin her zaman yeniden hesaplanmasını zorlayıp zorlamayacağını belirtir. |
| [getClass()](#getClass--) |  |
| [getProcessBuiltInFunctions()](#getProcessBuiltInFunctions--) | Yerleşik motor tarafından desteklenen yerleşik işlevlerin bu uygulama tarafından kontrol edilip işlenip işlenmeyeceğini belirtir. |
| [hashCode()](#hashCode--) |  |
| [isParamArrayModeRequired()](#isParamArrayModeRequired--) | Bu motorun parametrenin dizi modunda hesaplanması gerekip gerekmediğini gösterir. |
| [isParamLiteralRequired()](#isParamLiteralRequired--) | Bu motorun hesaplama sırasında parametrenin gerçek metnini gerekip gerektirmediğini gösterir. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [skipCalculation()](#skipCalculation--) | Şu anda değerlendirilen işlevi referans alan tüm formülün hesaplamasını atlar. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### AbstractCalculationEngine() {#AbstractCalculationEngine--}
```
public AbstractCalculationEngine()
```


### calculate(CalculationData data) {#calculate-com.aspose.cells.CalculationData-}
```
public abstract void calculate(CalculationData data)
```


Verilen verilerle bir işlevi hesaplar.

**Remarks**

Kullanıcı, bu uygulamada kendisi hesaplamak istediği tüm işlevler (excel yerel işlevleri dahil) için verilen verilerin hesaplanmış değerini ayarlamalıdır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| data | [CalculationData](../../com.aspose.cells/calculationdata) | İşlev adını, parametreleri vb. gibi işlevi hesaplamak için gerekli veriler. |

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
### forceRecalculate(String functionName) {#forceRecalculate-java.lang.String-}
```
public boolean forceRecalculate(String functionName)
```


Paylaşılan formüller hesaplanırken verilen işlevin her zaman yeniden hesaplanmasını zorlayıp zorlamayacağını belirtir.

**Remarks**

Paylaşılan formüller için birden fazla hücre aynı işlevi paylaşır. İşlevin parametreleri bu hücreler için de aynı kalıyorsa, genellikle bu işlev yalnızca bir kez hesaplanmalıdır. Bu nedenle performans açısından bu tür işlevi de yalnızca bir kez hesaplarız ([calculate(CalculationData)](../../com.aspose.cells/abstractcalculationengine\#calculate-CalculationData-) yalnızca bir kez çağrılır, her hücre için tekrar tekrar çağrılmak yerine). Ancak, kullanıcının özel uygulamasında, özellikle özel işlev, farklı hücreler için farklı şekilde hesaplanması gerekebilir. Bu durumda, kullanıcı bu yöntemi geçersiz kılarak işlev için true döndürmelidir. Ve [calculate(CalculationData)](../../com.aspose.cells/abstractcalculationengine\#calculate-CalculationData-) için verilen [CalculationData.getCalculatedValue()](../../com.aspose.cells/calculationdata\#getCalculatedValue--) önceki hesaplamanın önbelleğe alınmış değeriyle başlatılmış olabilir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| functionName | java.lang.String | İşlevin adı. Genellikle özel işlevin adıdır. Eğer [getProcessBuiltInFunctions()](../../com.aspose.cells/abstractcalculationengine\#getProcessBuiltInFunctions--) true ise, yerleşik işlevler de burada kontrol edilir. |

**Returns:**
boolean - belirtilen işlevin her zaman yeniden hesaplanması gerekiyorsa true.
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getProcessBuiltInFunctions() {#getProcessBuiltInFunctions--}
```
public boolean getProcessBuiltInFunctions()
```


Yerleşik motor tarafından desteklenen yerleşik işlevlerin bu uygulama tarafından kontrol edilip işlenip işlenmeyeceği. Varsayılan false.

**Remarks**

Kullanıcı bazı yerleşik işlevlerin hesaplama mantığını değiştirmek istiyorsa, bu özellik true olarak ayarlanmalıdır. Aksi takdirde performans açısından bu özelliği false bırakınız.

**Returns:**
boolean
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isParamArrayModeRequired() {#isParamArrayModeRequired--}
```
public boolean isParamArrayModeRequired()
```


Bu motorun parametrenin dizi modunda hesaplanması gerekip gerekmediğini gösterir. Varsayılan değer false'tur. Özel işlevler hesaplanırken [CalculationData.getParamValueInArrayMode(int,int,int)](../../com.aspose.cells/calculationdata\#getParamValueInArrayMode-int-int-int-) gerekli ise ve kullanıcı bu işlevlerin tanımını ( [Workbook.updateCustomFunctionDefinition(CustomFunctionDefinition)](../../com.aspose.cells/workbook\#updateCustomFunctionDefinition-CustomFunctionDefinition-) ile) güncellememişse, bu özellik true olarak ayarlanmalıdır.

**Remarks**

Eğer bu özel hesaplama motoru parametrenin dizi modunda hesaplanmasını gerektiriyorsa, parametreler için ağacı önbelleğe almak üzere daha fazla yığına ihtiyaç duyulur ve Calculate() yöntemi parametrenin değerini hesaplamak için özyinelemeli olarak çağrılabilir. Performans açısından, özel bir gereksinim yoksa lütfen bu özelliği varsayılan değer (false) olarak tutun.

**Returns:**
boolean
### isParamLiteralRequired() {#isParamLiteralRequired--}
```
public boolean isParamLiteralRequired()
```


Bu motorun bir hesaplama yaparken parametrenin gerçek metnine ihtiyacı olup olmadığını gösterir. Varsayılan değer false'tur.

**Remarks**

Bu özel hesaplama motoru parametrenin gerçek metnine ihtiyaç duyuyorsa, parametreler için gerçek metni önbelleğe almak üzere daha fazla yığın gerekecek ve `Calculate()` yöntemi parametrenin değerini hesaplamak için yinelemeli olarak çağrılabilir. Genel olarak, formüllerin hesaplanması için gerçek metin gerekli değildir ve bu özellik, çoğu uygulama için daha iyi performans elde etmek amacıyla false olarak tutulmalıdır.

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




### skipCalculation() {#skipCalculation--}
```
public void skipCalculation()
```


Şu anda değerlendirilen işlevi referans alan tüm formülün hesaplamasını atlar.

**Remarks**

Bu yöntem, tüm formülün hesaplamasını atlamak ve formülün orijinal değerinin değişmeden korunmasını sağlamak için [calculate(CalculationData)](../../com.aspose.cells/abstractcalculationengine\#calculate-CalculationData-) uygulamasında çağrılabilir.

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

