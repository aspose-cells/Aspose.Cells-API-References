---
title: "GridValidation"
second_title: "Aspose.Cells for Java API Referansı"
description: "data validation.settings'i temsil eder."
type: docs
url: /tr/java/com.aspose.gridweb/gridvalidation/
---

**Inheritance:**
java.lang.Object
```
public class GridValidation
```

data validation.settings'i temsil eder.
## Alanlar

| Alan | Açıklama |
| --- | --- |
| [ServerValidation](#ServerValidation) | Sunucu tarafı doğrulama JavaScript işlevinin adını alır veya ayarlar. |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [addACell(int row, int column)](#addACell-int-int-) | Hücreye doğrulama ayarlarını ekleyin. |
| [addACell(String cellname)](#addACell-java.lang.String-) | Hücreye doğrulama ayarlarını ekleyin. |
| [addArea(GridCellArea cellArea)](#addArea-com.aspose.gridweb.GridCellArea-) | Doğrulamayı alana uygular. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAreaList()](#getAreaList--) | Veri doğrulama ayarlarını içeren [GridCellArea](../../com.aspose.gridweb/gridcellarea) koleksiyonunu temsil eder. |
| [getClass()](#getClass--) |  |
| [getClientValidationFunction()](#getClientValidationFunction--) | İstemci doğrulama JavaScript işlevinin adını alır. |
| [getErrorMessage()](#getErrorMessage--) | Veri doğrulama hata mesajını temsil eder. |
| [getErrorTitle()](#getErrorTitle--) | Veri doğrulama hata iletişim kutusunun başlığını temsil eder. |
| [getFormula1()](#getFormula1--) | Veri doğrulama ile ilişkili değeri veya ifadeyi temsil eder. |
| [getFormula2()](#getFormula2--) | Veri doğrulamanın ikinci bölümüyle ilişkili değeri veya ifadeyi temsil eder. |
| [getInputMessage()](#getInputMessage--) | Veri doğrulama hata mesajını temsil eder. |
| [getInputTitle()](#getInputTitle--) | Veri-doğrulama giriş iletişim kutusunun başlığını temsil eder. |
| [getListValue(int row, int column)](#getListValue-int-int-) | Belirtilen hücre için doğrulama listesinin değerini al. |
| [getOperator()](#getOperator--) | Veri doğrulama için operatörü temsil eder. |
| [getRegEx()](#getRegEx--) | Düzenli ifade dizesini alır. |
| [getShowError()](#getShowError--) | Kullanıcı geçersiz veri girdiğinde veri doğrulama hata mesajının gösterilip gösterilmeyeceğini belirtir. |
| [getShowInput()](#getShowInput--) | Kullanıcı veri doğrulama aralığındaki bir hücreyi seçtiğinde veri doğrulama giriş mesajının gösterilip gösterilmeyeceğini belirtir. |
| [getValidationType()](#getValidationType--) | Doğrulama türünü alır. |
| [getValue1()](#getValue1--) | Veri doğrulama ile ilişkili değeri temsil eder. |
| [getValueList()](#getValueList--) | Değer listesi nesnesini alır. |
| [hashCode()](#hashCode--) |  |
| [isRequired()](#isRequired--) | Hücre değerinin gerekli olup olmadığını alır. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [removeACell(int row, int column)](#removeACell-int-int-) | Hücredeki doğrulama ayarlarını kaldır. |
| [removeArea(GridCellArea cellArea)](#removeArea-com.aspose.gridweb.GridCellArea-) | Aralıktaki doğrulama ayarlarını kaldır. |
| [setClientValidationFunction(String value)](#setClientValidationFunction-java.lang.String-) | İstemci doğrulama JavaScript işlevinin adını ayarlar. |
| [setErrorMessage(String value)](#setErrorMessage-java.lang.String-) | Veri doğrulama hata mesajını temsil eder. |
| [setErrorTitle(String value)](#setErrorTitle-java.lang.String-) | Veri doğrulama hata iletişim kutusunun başlığını temsil eder. |
| [setFormula1(String value)](#setFormula1-java.lang.String-) | Veri doğrulama ile ilişkili değeri veya ifadeyi temsil eder. |
| [setFormula2(String value)](#setFormula2-java.lang.String-) | Veri doğrulamanın ikinci bölümüyle ilişkili değeri veya ifadeyi temsil eder. |
| [setInputMessage(String value)](#setInputMessage-java.lang.String-) | Veri doğrulama hata mesajını temsil eder. |
| [setInputTitle(String value)](#setInputTitle-java.lang.String-) | Veri-doğrulama giriş iletişim kutusunun başlığını temsil eder. |
| [setOperator(int value)](#setOperator-int-) | Veri doğrulama için operatörü temsil eder. |
| [setRegEx(String value)](#setRegEx-java.lang.String-) | Düzenli ifade dizesini ayarlar. |
| [setRequired(boolean value)](#setRequired-boolean-) | Hücre değerinin gerekli olup olmadığını ayarlar. |
| [setShowError(boolean value)](#setShowError-boolean-) | Kullanıcı geçersiz veri girdiğinde veri doğrulama hata mesajının gösterilip gösterilmeyeceğini belirtir. |
| [setShowInput(boolean value)](#setShowInput-boolean-) | Kullanıcı veri doğrulama aralığındaki bir hücreyi seçtiğinde veri doğrulama giriş mesajının gösterilip gösterilmeyeceğini belirtir. |
| [setValidationType(int value)](#setValidationType-int-) | Doğrulama türünü ayarlar. |
| [setValueList(ArrayList<String> value)](#setValueList-java.util.ArrayList-java.lang.String--) | Değer listesi nesnesini ayarlar. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### ServerValidation {#ServerValidation}
```
public GridCustomServerValidation ServerValidation
```


Sunucu tarafı doğrulama JavaScript işlevinin adını alır veya ayarlar.

**Remarks**

Sunucu tarafı doğrulamayı belirtmek için GridCustomServerValidation özelliğini kullanın.

### addACell(int row, int column) {#addACell-int-int-}
```
public void addACell(int row, int column)
```


Hücreye doğrulama ayarlarını ekleyin.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| satır | int | Satır indeksi. |
| sütun | int | Sütun indeksi. |

### addACell(String cellname) {#addACell-java.lang.String-}
```
public void addACell(String cellname)
```


Hücreye doğrulama ayarlarını ekleyin.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| cellname | java.lang.String | hücre adı. |

### addArea(GridCellArea cellArea) {#addArea-com.aspose.gridweb.GridCellArea-}
```
public void addArea(GridCellArea cellArea)
```


Doğrulamayı alana uygular.

**Remarks**

Bu yöntemde, bu alandaki tüm eski doğrulamaları kaldıracağız.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| cellArea | [GridCellArea](../../com.aspose.gridweb/gridcellarea) | Alan. |

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
### getAreaList() {#getAreaList--}
```
public ArrayList getAreaList()
```


Veri doğrulama ayarlarını içeren [GridCellArea](../../com.aspose.gridweb/gridcellarea) koleksiyonunu temsil eder.

**Remarks**

Alandaki eski doğrulamalar, doğrudan bu listeye eklenirse kaldırılmayacaktır.

**Returns:**
java.util.ArrayList
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getClientValidationFunction() {#getClientValidationFunction--}
```
public String getClientValidationFunction()
```


İstemci doğrulama JavaScript işlevinin adını alır.

**Remarks**

ClientValidationFunction özelliğini kullanarak istemci doğrulama fonksiyonunun adını belirtin. Fonksiyon şu şekilde tanımlanmalıdır:
function customValicationFunction(source, value)
"source" parametresi hücre nesnesidir. "value" parametresi kontrol edilecek bir hücrenin string değeridir. Fonksiyon değer geçerliyse true döndürmelidir.

**Returns:**
java.lang.String
### getErrorMessage() {#getErrorMessage--}
```
public String getErrorMessage()
```


Veri doğrulama hata mesajını temsil eder.

**Returns:**
java.lang.String
### getErrorTitle() {#getErrorTitle--}
```
public String getErrorTitle()
```


Veri doğrulama hata iletişim kutusunun başlığını temsil eder.

**Returns:**
java.lang.String
### getFormula1() {#getFormula1--}
```
public String getFormula1()
```


Veri doğrulama ile ilişkili değeri veya ifadeyi temsil eder.

**Returns:**
java.lang.String
### getFormula2() {#getFormula2--}
```
public String getFormula2()
```


Veri doğrulamanın ikinci bölümüyle ilişkili değeri veya ifadeyi temsil eder.

**Returns:**
java.lang.String
### getInputMessage() {#getInputMessage--}
```
public String getInputMessage()
```


Veri doğrulama hata mesajını temsil eder.

**Returns:**
java.lang.String
### getInputTitle() {#getInputTitle--}
```
public String getInputTitle()
```


Veri-doğrulama giriş iletişim kutusunun başlığını temsil eder.

**Returns:**
java.lang.String
### getListValue(int row, int column) {#getListValue-int-int-}
```
public Object getListValue(int row, int column)
```


Belirtilen hücre için doğrulama listesinin değerini al.

**Remarks**

Yalnızca türü Liste olan ve verilen hücreye uygulanmış doğrulama için, aksi takdirde null döndürülür.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| satır | int | Satır indeksi. |
| sütun | int | Sütun indeksi. |

**Returns:**
java.lang.Object - Belirtilen hücre için bu doğrulamanın listesini üretmek üzere değer. Liste bir aralığa referans veriyorsa, döndürülen değer bir ReferredArea nesnesi olacaktır; aksi takdirde döndürülen değer null, object[] veya basit bir nesne olabilir.
### getOperator() {#getOperator--}
```
public int getOperator()
```


Veri doğrulama için operatörü temsil eder.

Bakınız [GridOperatorType](../../com.aspose.gridweb/gridoperatortype).

**Returns:**
int
### getRegEx() {#getRegEx--}
```
public String getRegEx()
```


Düzenli ifade dizesini alır.

**Returns:**
java.lang.String
### getShowError() {#getShowError--}
```
public boolean getShowError()
```


Kullanıcı geçersiz veri girdiğinde veri doğrulama hata mesajının gösterilip gösterilmeyeceğini belirtir.

**Returns:**
boolean
### getShowInput() {#getShowInput--}
```
public boolean getShowInput()
```


Kullanıcı veri doğrulama aralığındaki bir hücreyi seçtiğinde veri doğrulama giriş mesajının gösterilip gösterilmeyeceğini belirtir.

**Returns:**
boolean
### getValidationType() {#getValidationType--}
```
public int getValidationType()
```


Doğrulama türünü alır.

Bakınız [GridValidationType](../../com.aspose.gridweb/gridvalidationtype).

**Returns:**
int
### getValue1() {#getValue1--}
```
public Object[] getValue1()
```


Veri doğrulama ile ilişkili değeri temsil eder.

**Returns:**
java.lang.Object[]
### getValueList() {#getValueList--}
```
public ArrayList<String> getValueList()
```


Değer listesi nesnesini alır.

**Returns:**
java.util.ArrayList<java.lang.String>
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isRequired() {#isRequired--}
```
public boolean isRequired()
```


Hücre değerinin gerekli olup olmadığını alır.

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




### removeACell(int row, int column) {#removeACell-int-int-}
```
public void removeACell(int row, int column)
```


Hücredeki doğrulama ayarlarını kaldır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| satır | int | Satır indeksi. |
| sütun | int | Sütun indeksi. |

### removeArea(GridCellArea cellArea) {#removeArea-com.aspose.gridweb.GridCellArea-}
```
public void removeArea(GridCellArea cellArea)
```


Aralıktaki doğrulama ayarlarını kaldır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| cellArea | [GridCellArea](../../com.aspose.gridweb/gridcellarea) | Veri doğrulama ayarlarını içeren aralık. |

### setClientValidationFunction(String value) {#setClientValidationFunction-java.lang.String-}
```
public void setClientValidationFunction(String value)
```


İstemci doğrulama JavaScript işlevinin adını ayarlar.

**Remarks**

ClientValidationFunction özelliğini kullanarak istemci doğrulama fonksiyonunun adını belirtin. Fonksiyon şu şekilde tanımlanmalıdır:
function customValicationFunction(source, value)
"source" parametresi hücre nesnesidir. "value" parametresi kontrol edilecek bir hücrenin string değeridir. Fonksiyon değer geçerliyse true döndürmelidir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

### setErrorMessage(String value) {#setErrorMessage-java.lang.String-}
```
public void setErrorMessage(String value)
```


Veri doğrulama hata mesajını temsil eder.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

### setErrorTitle(String value) {#setErrorTitle-java.lang.String-}
```
public void setErrorTitle(String value)
```


Veri doğrulama hata iletişim kutusunun başlığını temsil eder.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

### setFormula1(String value) {#setFormula1-java.lang.String-}
```
public void setFormula1(String value)
```


Veri doğrulama ile ilişkili değeri veya ifadeyi temsil eder.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

### setFormula2(String value) {#setFormula2-java.lang.String-}
```
public void setFormula2(String value)
```


Veri doğrulamanın ikinci bölümüyle ilişkili değeri veya ifadeyi temsil eder.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

### setInputMessage(String value) {#setInputMessage-java.lang.String-}
```
public void setInputMessage(String value)
```


Veri doğrulama hata mesajını temsil eder.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

### setInputTitle(String value) {#setInputTitle-java.lang.String-}
```
public void setInputTitle(String value)
```


Veri-doğrulama giriş iletişim kutusunun başlığını temsil eder.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

### setOperator(int value) {#setOperator-int-}
```
public void setOperator(int value)
```


Veri doğrulama için operatörü temsil eder.

Bakınız [GridOperatorType](../../com.aspose.gridweb/gridoperatortype).

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setRegEx(String value) {#setRegEx-java.lang.String-}
```
public void setRegEx(String value)
```


Düzenli ifade dizesini ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

### setRequired(boolean value) {#setRequired-boolean-}
```
public void setRequired(boolean value)
```


Hücre değerinin gerekli olup olmadığını ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setShowError(boolean value) {#setShowError-boolean-}
```
public void setShowError(boolean value)
```


Kullanıcı geçersiz veri girdiğinde veri doğrulama hata mesajının gösterilip gösterilmeyeceğini belirtir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setShowInput(boolean value) {#setShowInput-boolean-}
```
public void setShowInput(boolean value)
```


Kullanıcı veri doğrulama aralığındaki bir hücreyi seçtiğinde veri doğrulama giriş mesajının gösterilip gösterilmeyeceğini belirtir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setValidationType(int value) {#setValidationType-int-}
```
public void setValidationType(int value)
```


Doğrulama türünü ayarlar.

Bakınız [GridValidationType](../../com.aspose.gridweb/gridvalidationtype).

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setValueList(ArrayList<String> value) {#setValueList-java.util.ArrayList-java.lang.String--}
```
public void setValueList(ArrayList<String> value)
```


Değer listesi nesnesini ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.util.ArrayList<java.lang.String> |  |

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

