---
title: "FindOptions"
second_title: "Aspose.Cells for Java API Referansı"
description: "Bulma seçeneklerini temsil eder."
type: docs
url: /tr/java/com.aspose.cells/findoptions/
---

**Inheritance:**
java.lang.Object
```
public class FindOptions
```

Bulma seçeneklerini temsil eder.

**Example**

```
         //Instantiate the workbook object
         Workbook workbook = new Workbook("book1.xls");
 
         //Get Cells collection 
         Cells cells = workbook.getWorksheets().get(0).getCells();
 
         //Instantiate FindOptions Object
         FindOptions findOptions = new FindOptions();
 
         //Create a Cells Area
         CellArea ca = new CellArea();
         ca.StartRow = 8;
         ca.StartColumn = 2;
         ca.EndRow = 17;
         ca.EndColumn = 13;
 
         //Set cells area for find options
         findOptions.setRange(ca);
 
         //Set searching properties
         findOptions.setSearchBackward(false);
 
         findOptions.setSearchOrderByRows(true);
 
         findOptions.setLookInType(LookInType.VALUES);
 
         //Find the cell with 0 value
         Cell cell = cells.find(0, null, findOptions);
```
## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [FindOptions()](#FindOptions--) |  |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getCaseSensitive()](#getCaseSensitive--) | Aranan dizgenin büyük/küçük harfe duyarlı olup olmadığını gösterir. |
| [getClass()](#getClass--) |  |
| [getConvertNumericData()](#getConvertNumericData--) | Aranan dize değerinin sayısal veriye dönüştürülüp dönüştürülmediğini gösteren bir değer alır. |
| [getLookAtType()](#getLookAtType--) | Bakma türü. |
| [getLookInType()](#getLookInType--) | İçinde bakma türü. |
| [getRange()](#getRange--) | Aranan aralığı alır ve ayarlar. |
| [getRegexKey()](#getRegexKey--) | Aranan anahtarın regex olup olmadığını gösterir. |
| [getSearchBackward()](#getSearchBackward--) | Hücreler için geriye doğru arama yapılıp yapılmayacağını belirtir. |
| [getSearchNext()](#getSearchNext--) | Arama sırası. |
| [getSearchOrderByRows()](#getSearchOrderByRows--) | Arama sırasının satırlara mı yoksa sütunlara mı göre yapılacağını gösterir. |
| [getStyle()](#getStyle--) | Aranacak format. |
| [getValueTypeSensitive()](#getValueTypeSensitive--) | Aranan hücre değeri türünün aranan anahtar ile aynı olup olması gerektiğini gösterir. |
| [hashCode()](#hashCode--) |  |
| [isRangeSet()](#isRangeSet--) | Aranan aralığın ayarlanıp ayarlanmadığını gösterir. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setCaseSensitive(boolean value)](#setCaseSensitive-boolean-) | Aranan dizgenin büyük/küçük harfe duyarlı olup olmadığını gösterir. |
| [setConvertNumericData(boolean value)](#setConvertNumericData-boolean-) | Aranan dize değerinin sayısal veriye dönüştürülüp dönüştürülmeyeceğini gösteren bir değer ayarlar. |
| [setLookAtType(int value)](#setLookAtType-int-) | Bakma türü. |
| [setLookInType(int value)](#setLookInType-int-) | İçinde bakma türü. |
| [setRange(CellArea ca)](#setRange-com.aspose.cells.CellArea-) | Aranan aralığı ayarlar. |
| [setRegexKey(boolean value)](#setRegexKey-boolean-) | Aranan anahtarın regex olup olmadığını gösterir. |
| [setSearchBackward(boolean value)](#setSearchBackward-boolean-) | Hücreler için geriye doğru arama yapılıp yapılmayacağını belirtir. |
| [setSearchNext(boolean value)](#setSearchNext-boolean-) | Arama sırası. |
| [setSearchOrderByRows(boolean value)](#setSearchOrderByRows-boolean-) | Arama sırasının satırlara mı yoksa sütunlara mı göre yapılacağını gösterir. |
| [setStyle(Style value)](#setStyle-com.aspose.cells.Style-) | Aranacak format. |
| [setValueTypeSensitive(boolean value)](#setValueTypeSensitive-boolean-) | Aranan hücre değeri türünün aranan anahtar ile aynı olup olması gerektiğini gösterir. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### FindOptions() {#FindOptions--}
```
public FindOptions()
```


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
### getCaseSensitive() {#getCaseSensitive--}
```
public boolean getCaseSensitive()
```


Aranan dizgenin büyük/küçük harfe duyarlı olup olmadığını gösterir.

**Returns:**
boolean
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getConvertNumericData() {#getConvertNumericData--}
```
public boolean getConvertNumericData()
```


Aranan dize değerinin sayısal veriye dönüştürülüp dönüştürülmediğini gösteren bir değer alır.

**Returns:**
boolean
### getLookAtType() {#getLookAtType--}
```
public int getLookAtType()
```


Bakma türü.

Bakınız [LookAtType](../../com.aspose.cells/lookattype).

**Remarks**

When [getRegexKey()](../../com.aspose.cells/findoptions\#getRegexKey--) true ise ve kullanıcı regex için kesin kuralı belirtmişse, performans açısından bu özellik [LookAtType.ENTIRE\_CONTENT](../../com.aspose.cells/lookattype\#ENTIRE-CONTENT) olarak ayarlanmalıdır. Aksi takdirde arama anahtarını, belirli türe göre eşleşebileceğinden emin olmak için yeniden düzenleyeceğiz. Örneğin, tür [LookAtType.CONTAINS](../../com.aspose.cells/lookattype\#CONTAINS) (bu özellik için varsayılan değerdir) olduğunda, arama anahtarının başına ve sonuna otomatik olarak joker karakterler ekleyeceğiz. Bu durumda, düzenli ifadeler daha karmaşık hâle gelecek ve performans da azalacaktır.

**Returns:**
int
### getLookInType() {#getLookInType--}
```
public int getLookInType()
```


İçinde bakma türü.

Bakınız [LookInType](../../com.aspose.cells/lookintype).

**Returns:**
int
### getRange() {#getRange--}
```
public CellArea getRange()
```


Aranan aralığı alır ve ayarlar.

**Returns:**
[CellArea](../../com.aspose.cells/cellarea) - Returns the searched range.
### getRegexKey() {#getRegexKey--}
```
public boolean getRegexKey()
```


Aranan anahtarın regex olup olmadığını gösterir. True ise aranan anahtar regex olarak alınır ve ayrıştırılır. Aksi takdirde anahtar MS Excel'deki kurallara göre ayrıştırılır.

**Remarks**

Arama anahtarı regex olarak belirtilmiş olsa da, belirtilen [getLookAtType()](../../com.aspose.cells/findoptions\#getLookAtType--) göre yeniden düzenlenebilir. Örneğin, tür [LookAtType.CONTAINS](../../com.aspose.cells/lookattype\#CONTAINS) (bu seçenekler için varsayılan değerdir) olduğunda, eşleşmenin "contains" olarak kontrol edilmesini sağlamak için arama anahtarının başına ve sonuna otomatik olarak joker karakterler eklenir. Bu durumda, düzenli ifadeler daha karmaşık hâle gelir ve performans da azalır. Bu nedenle, performans açısından, kullanıcı regex için kesin kuralı belirtmişse, ek bir kısıtlama olarak [getLookAtType()](../../com.aspose.cells/findoptions\#getLookAtType--) kullanmaya gerek yoktur ve kullanıcı daha iyi performans için bunu [LookAtType.ENTIRE\_CONTENT](../../com.aspose.cells/lookattype\#ENTIRE-CONTENT) olarak ayarlayabilir.

**Returns:**
boolean
### getSearchBackward() {#getSearchBackward--}
```
public boolean getSearchBackward()
```


Hücreler için geriye doğru arama yapılıp yapılmayacağını belirtir.

**Returns:**
boolean
### getSearchNext() {#getSearchNext--}
```
public boolean getSearchNext()
```


Arama sırası. True: sonraki öğeyi ara. False: önceki öğeyi ara.

**Remarks**

NOT: Bu üye artık kullanımdan kaldırıldı. Bunun yerine lütfen FindOptions.SearchBackward özelliğini kullanın. Bu özellik Kasım 2018'den itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

**Returns:**
boolean
### getSearchOrderByRows() {#getSearchOrderByRows--}
```
public boolean getSearchOrderByRows()
```


Arama sırasının satırlara mı yoksa sütunlara mı göre yapılacağını gösterir.

**Returns:**
boolean
### getStyle() {#getStyle--}
```
public Style getStyle()
```


Aranacak format.

**Returns:**
[Style](../../com.aspose.cells/style)
### getValueTypeSensitive() {#getValueTypeSensitive--}
```
public boolean getValueTypeSensitive()
```


Aranan hücre değeri türünün aranan anahtar ile aynı olup olması gerektiğini gösterir.

**Returns:**
boolean
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isRangeSet() {#isRangeSet--}
```
public boolean isRangeSet()
```


Aranan aralığın ayarlanıp ayarlanmadığını gösterir.

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




### setCaseSensitive(boolean value) {#setCaseSensitive-boolean-}
```
public void setCaseSensitive(boolean value)
```


Aranan dizgenin büyük/küçük harfe duyarlı olup olmadığını gösterir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setConvertNumericData(boolean value) {#setConvertNumericData-boolean-}
```
public void setConvertNumericData(boolean value)
```


Aranan dize değerinin sayısal veriye dönüştürülüp dönüştürülmeyeceğini gösteren bir değer ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setLookAtType(int value) {#setLookAtType-int-}
```
public void setLookAtType(int value)
```


Bakma türü.

Bakınız [LookAtType](../../com.aspose.cells/lookattype).

**Remarks**

When [getRegexKey()](../../com.aspose.cells/findoptions\#getRegexKey--) true ise ve kullanıcı regex için kesin kuralı belirtmişse, performans açısından bu özellik [LookAtType.ENTIRE\_CONTENT](../../com.aspose.cells/lookattype\#ENTIRE-CONTENT) olarak ayarlanmalıdır. Aksi takdirde arama anahtarını, belirli türe göre eşleşebileceğinden emin olmak için yeniden düzenleyeceğiz. Örneğin, tür [LookAtType.CONTAINS](../../com.aspose.cells/lookattype\#CONTAINS) (bu özellik için varsayılan değerdir) olduğunda, arama anahtarının başına ve sonuna otomatik olarak joker karakterler ekleyeceğiz. Bu durumda, düzenli ifadeler daha karmaşık hâle gelecek ve performans da azalacaktır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setLookInType(int value) {#setLookInType-int-}
```
public void setLookInType(int value)
```


İçinde bakma türü.

Bakınız [LookInType](../../com.aspose.cells/lookintype).

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setRange(CellArea ca) {#setRange-com.aspose.cells.CellArea-}
```
public void setRange(CellArea ca)
```


Aranan aralığı ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| ca | [CellArea](../../com.aspose.cells/cellarea) | aranan aralık. |

### setRegexKey(boolean value) {#setRegexKey-boolean-}
```
public void setRegexKey(boolean value)
```


Aranan anahtarın regex olup olmadığını gösterir. True ise aranan anahtar regex olarak alınır ve ayrıştırılır. Aksi takdirde anahtar MS Excel'deki kurallara göre ayrıştırılır.

**Remarks**

Arama anahtarı regex olarak belirtilmiş olsa da, belirtilen [getLookAtType()](../../com.aspose.cells/findoptions\#getLookAtType--) göre yeniden düzenlenebilir. Örneğin, tür [LookAtType.CONTAINS](../../com.aspose.cells/lookattype\#CONTAINS) (bu seçenekler için varsayılan değerdir) olduğunda, eşleşmenin "contains" olarak kontrol edilmesini sağlamak için arama anahtarının başına ve sonuna otomatik olarak joker karakterler eklenir. Bu durumda, düzenli ifadeler daha karmaşık hâle gelir ve performans da azalır. Bu nedenle, performans açısından, kullanıcı regex için kesin kuralı belirtmişse, ek bir kısıtlama olarak [getLookAtType()](../../com.aspose.cells/findoptions\#getLookAtType--) kullanmaya gerek yoktur ve kullanıcı daha iyi performans için bunu [LookAtType.ENTIRE\_CONTENT](../../com.aspose.cells/lookattype\#ENTIRE-CONTENT) olarak ayarlayabilir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setSearchBackward(boolean value) {#setSearchBackward-boolean-}
```
public void setSearchBackward(boolean value)
```


Hücreler için geriye doğru arama yapılıp yapılmayacağını belirtir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setSearchNext(boolean value) {#setSearchNext-boolean-}
```
public void setSearchNext(boolean value)
```


Arama sırası. True: sonraki öğeyi ara. False: önceki öğeyi ara.

**Remarks**

NOT: Bu üye artık kullanımdan kaldırıldı. Bunun yerine lütfen FindOptions.SearchBackward özelliğini kullanın. Bu özellik Kasım 2018'den itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setSearchOrderByRows(boolean value) {#setSearchOrderByRows-boolean-}
```
public void setSearchOrderByRows(boolean value)
```


Arama sırasının satırlara mı yoksa sütunlara mı göre yapılacağını gösterir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setStyle(Style value) {#setStyle-com.aspose.cells.Style-}
```
public void setStyle(Style value)
```


Aranacak format.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [Style](../../com.aspose.cells/style) |  |

### setValueTypeSensitive(boolean value) {#setValueTypeSensitive-boolean-}
```
public void setValueTypeSensitive(boolean value)
```


Aranan hücre değeri türünün aranan anahtar ile aynı olup olması gerektiğini gösterir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

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

