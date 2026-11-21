---
title: "Doğrulama"
second_title: "Aspose.Cells for Java API Referansı"
description: "data validation.settings'i temsil eder."
type: docs
url: /tr/java/com.aspose.cells/validation/
---

**Inheritance:**
java.lang.Object
```
public class Validation
```

data validation.settings'i temsil eder.

**Example**

```
         Workbook workbook = new Workbook();
         	ValidationCollection validations = workbook.getWorksheets().get(0).getValidations();
         	CellArea area = CellArea.createCellArea(0, 0, 1, 1);
         	Validation validation = validations.get(validations.add(area));
         	validation.setType(com.aspose.cells.ValidationType.WHOLE_NUMBER);
         	validation.setOperator(OperatorType.BETWEEN);
         	validation.setFormula1("3");
         	validation.setFormula2("1234");
```
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [addArea(CellArea cellArea)](#addArea-com.aspose.cells.CellArea-) | Doğrulamayı alana uygular. |
| [addArea(CellArea cellArea, boolean checkIntersection, boolean checkEdge)](#addArea-com.aspose.cells.CellArea-boolean-boolean-) | Doğrulamayı alana uygular. |
| [addAreas(CellArea[] areas, boolean checkIntersection, boolean checkEdge)](#addAreas-com.aspose.cells.CellArea---boolean-boolean-) | Doğrulamayı verilen alanlara uygular. |
| [copy(Validation source, CopyOptions copyOption)](#copy-com.aspose.cells.Validation-com.aspose.cells.CopyOptions-) | Doğrulamayı kopyala. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAlertStyle()](#getAlertStyle--) | Doğrulama uyarı stilini temsil eder. |
| [getAreas()](#getAreas--) | Veri doğrulama ayarlarını içeren tüm [CellArea](../../com.aspose.cells/cellarea) öğelerini alır. |
| [getClass()](#getClass--) |  |
| [getErrorMessage()](#getErrorMessage--) | Veri doğrulama hata mesajını temsil eder. |
| [getErrorTitle()](#getErrorTitle--) | Veri doğrulama hata iletişim kutusunun başlığını temsil eder. |
| [getFormula1()](#getFormula1--) | Veri doğrulama ile ilişkili değeri veya ifadeyi temsil eder. |
| [getFormula1(boolean isR1C1, boolean isLocal)](#getFormula1-boolean-boolean-) | Bu doğrulama ile ilişkili değeri veya ifadeyi alır. |
| [getFormula1(boolean isR1C1, boolean isLocal, int row, int column)](#getFormula1-boolean-boolean-int-int-) | Belirli bir hücre için bu doğrulama ile ilişkili değeri veya ifadeyi alır. |
| [getFormula2()](#getFormula2--) | Veri doğrulama ile ilişkili değeri veya ifadeyi temsil eder. |
| [getFormula2(boolean isR1C1, boolean isLocal)](#getFormula2-boolean-boolean-) | Bu doğrulama ile ilişkili değeri veya ifadeyi alır. |
| [getFormula2(boolean isR1C1, boolean isLocal, int row, int column)](#getFormula2-boolean-boolean-int-int-) | Belirli bir hücre için bu doğrulama ile ilişkili değeri veya ifadeyi alır. |
| [getIgnoreBlank()](#getIgnoreBlank--) | Aralık veri doğrulaması tarafından boş değerlerin izin verilip verilmediğini gösterir. |
| [getInCellDropDown()](#getInCellDropDown--) | Veri doğrulamanın kabul edilebilir değerleri içeren bir açılır liste gösterip göstermediğini belirtir. |
| [getInputMessage()](#getInputMessage--) | Veri doğrulama giriş mesajını temsil eder. |
| [getInputTitle()](#getInputTitle--) | Veri-doğrulama giriş iletişim kutusunun başlığını temsil eder. |
| [getListValue(int row, int column)](#getListValue-int-int-) | Belirtilen hücre için doğrulama listesinin değerini al. |
| [getOperator()](#getOperator--) | Veri doğrulama için operatörü temsil eder. |
| [getShowError()](#getShowError--) | Kullanıcı geçersiz veri girdiğinde veri doğrulama hata mesajının gösterilip gösterilmeyeceğini belirtir. |
| [getShowInput()](#getShowInput--) | Kullanıcı veri doğrulama aralığındaki bir hücreyi seçtiğinde veri doğrulama giriş mesajının gösterilip gösterilmeyeceğini belirtir. |
| [getType()](#getType--) | Veri doğrulama türünü temsil eder. |
| [getValue(int row, int column, boolean isValue1)](#getValue-int-int-boolean-) | Belirli hücredeki doğrulamanın değerini al. |
| [getValue1()](#getValue1--) | Veri doğrulama ile ilişkili ilk değeri temsil eder. |
| [getValue2()](#getValue2--) | Veri doğrulama ile ilişkili ikinci değeri temsil eder. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [removeACell(int row, int column)](#removeACell-int-int-) | Hücredeki doğrulama ayarlarını kaldır. |
| [removeArea(CellArea cellArea)](#removeArea-com.aspose.cells.CellArea-) | Aralıktaki doğrulama ayarlarını kaldır. |
| [removeAreas(CellArea[] areas)](#removeAreas-com.aspose.cells.CellArea---) | Bu doğrulamayı verilen alanlardan kaldırır. |
| [setAlertStyle(int value)](#setAlertStyle-int-) | Doğrulama uyarı stilini temsil eder. |
| [setErrorMessage(String value)](#setErrorMessage-java.lang.String-) | Veri doğrulama hata mesajını temsil eder. |
| [setErrorTitle(String value)](#setErrorTitle-java.lang.String-) | Veri doğrulama hata iletişim kutusunun başlığını temsil eder. |
| [setFormula1(String value)](#setFormula1-java.lang.String-) | Veri doğrulama ile ilişkili değeri veya ifadeyi temsil eder. |
| [setFormula1(String formula, boolean isR1C1, boolean isLocal)](#setFormula1-java.lang.String-boolean-boolean-) | Bu doğrulama ile ilişkili değeri veya ifadeyi ayarlar. |
| [setFormula2(String value)](#setFormula2-java.lang.String-) | Veri doğrulama ile ilişkili değeri veya ifadeyi temsil eder. |
| [setFormula2(String formula, boolean isR1C1, boolean isLocal)](#setFormula2-java.lang.String-boolean-boolean-) | Bu doğrulama ile ilişkili değeri veya ifadeyi ayarlar. |
| [setIgnoreBlank(boolean value)](#setIgnoreBlank-boolean-) | Aralık veri doğrulaması tarafından boş değerlerin izin verilip verilmediğini gösterir. |
| [setInCellDropDown(boolean value)](#setInCellDropDown-boolean-) | Veri doğrulamanın kabul edilebilir değerleri içeren bir açılır liste gösterip göstermediğini belirtir. |
| [setInputMessage(String value)](#setInputMessage-java.lang.String-) | Veri doğrulama giriş mesajını temsil eder. |
| [setInputTitle(String value)](#setInputTitle-java.lang.String-) | Veri-doğrulama giriş iletişim kutusunun başlığını temsil eder. |
| [setOperator(int value)](#setOperator-int-) | Veri doğrulama için operatörü temsil eder. |
| [setShowError(boolean value)](#setShowError-boolean-) | Kullanıcı geçersiz veri girdiğinde veri doğrulama hata mesajının gösterilip gösterilmeyeceğini belirtir. |
| [setShowInput(boolean value)](#setShowInput-boolean-) | Kullanıcı veri doğrulama aralığındaki bir hücreyi seçtiğinde veri doğrulama giriş mesajının gösterilip gösterilmeyeceğini belirtir. |
| [setType(int value)](#setType-int-) | Veri doğrulama türünü temsil eder. |
| [setValue1(Object value)](#setValue1-java.lang.Object-) | Veri doğrulama ile ilişkili ilk değeri temsil eder. |
| [setValue2(Object value)](#setValue2-java.lang.Object-) | Veri doğrulama ile ilişkili ikinci değeri temsil eder. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### addArea(CellArea cellArea) {#addArea-com.aspose.cells.CellArea-}
```
public void addArea(CellArea cellArea)
```


Doğrulamayı alana uygular.

**Remarks**

Kesişim ve kenar kontrolüyle [addArea(CellArea,boolean,boolean)](../../com.aspose.cells/validation\\#addArea-CellArea-boolean-boolean-) kullanmaya eşdeğerdir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| cellArea | [CellArea](../../com.aspose.cells/cellarea) | Alan. |

### addArea(CellArea cellArea, boolean checkIntersection, boolean checkEdge) {#addArea-com.aspose.cells.CellArea-boolean-boolean-}
```
public void addArea(CellArea cellArea, boolean checkIntersection, boolean checkEdge)
```


Doğrulamayı alana uygular.

**Remarks**

Bu yöntemde, verilen alandaki tüm eski doğrulamaları kaldıracağız. Doğrulamanın uygulanan aralıklarının sol üst öğesi için, önce StartRow en küçük, ardından aynı en küçük StartRow değerine sahip alanlar arasında StartColumn en küçük olanı seçilir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| cellArea | [CellArea](../../com.aspose.cells/cellarea) | Alan. |
| checkIntersection | boolean | Verilen alanın mevcut doğrulama alanlarıyla kesişimini kontrol edip etmeyeceği. Eğer bir doğrulama verilen alanda (veya bir kısmında) uygulanmışsa, mevcut doğrulama önce verilen alandan kaldırılmalıdır. Aksi takdirde oluşturulan Doğrulamalarda bozulma meydana gelebilir. Kullanıcı eklenen alanın herhangi bir mevcut alanla kesişmediğinden emin ise, bu parametre performans düşüncesiyle false olarak ayarlanabilir. |
| checkEdge | boolean | Bu doğrulamanın uygulanan alanlarının kenarının kontrol edilip edilmeyeceği. Doğrulamanın iç ayarları, uygulanan aralıklarının sol üst öğesine bağlıdır; bu nedenle verilen alan uygulanan aralıkların yeni sol üst öğesi olacaksa, iç ayarlar değiştirilip yeniden oluşturulmalıdır, aksi takdirde beklenmeyen sonuçlar ortaya çıkabilir. Kullanıcı eklenen alanın sol üst öğe olmadığından emin ise, bu parametre performans düşüncesiyle false olarak ayarlanabilir. |

### addAreas(CellArea[] areas, boolean checkIntersection, boolean checkEdge) {#addAreas-com.aspose.cells.CellArea---boolean-boolean-}
```
public void addAreas(CellArea[] areas, boolean checkIntersection, boolean checkEdge)
```


Doğrulamayı verilen alanlara uygular.

**Remarks**

Bu yöntemde, verilen alandaki tüm eski doğrulamaları kaldıracağız. Doğrulamanın uygulanan aralıklarının sol üst öğesi için, önce StartRow en küçük, ardından aynı en küçük StartRow değerine sahip alanlar arasında StartColumn en küçük olanı seçilir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| areas | [CellArea\[\]](../../com.aspose.cells/cellarea) | Alanlar. |
| checkIntersection | boolean | Verilen alanın mevcut doğrulama alanlarıyla kesişimini kontrol edip etmeyeceği. Eğer bir doğrulama verilen alanda (veya bir kısmında) uygulanmışsa, mevcut doğrulama önce verilen alandan kaldırılmalıdır. Aksi takdirde oluşturulan Doğrulamalarda bozulma meydana gelebilir. Kullanıcı eklenen tüm alanların herhangi bir mevcut alanla kesişmediğinden emin ise, bu parametre performans düşüncesiyle false olarak ayarlanabilir. |
| checkEdge | boolean | Bu doğrulamanın uygulanan alanlarının kenarının kontrol edilip edilmeyeceği. Doğrulamanın iç ayarları, uygulanan aralıklarının sol üst öğesine bağlıdır; bu nedenle verilen alanlardan biri uygulanan aralıkların yeni sol üst öğesi olacaksa, iç ayarlar değiştirilip yeniden oluşturulmalıdır, aksi takdirde beklenmeyen sonuçlar ortaya çıkabilir. Kullanıcı eklenen bu alanlardan hiçbirinin sol üst öğe olmadığından emin ise, bu parametre performans düşüncesiyle false olarak ayarlanabilir. |

### copy(Validation source, CopyOptions copyOption) {#copy-com.aspose.cells.Validation-com.aspose.cells.CopyOptions-}
```
public void copy(Validation source, CopyOptions copyOption)
```


Doğrulamayı kopyala.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| source | [Validation](../../com.aspose.cells/validation) | Kaynak doğrulama. |
| copyOption | [CopyOptions](../../com.aspose.cells/copyoptions) | Kopya seçeneği. |

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
### getAlertStyle() {#getAlertStyle--}
```
public int getAlertStyle()
```


Doğrulama uyarı stilini temsil eder.

Bakınız [ValidationAlertType](../../com.aspose.cells/validationalerttype).

**Returns:**
int
### getAreas() {#getAreas--}
```
public CellArea[] getAreas()
```


Veri doğrulama ayarlarını içeren tüm [CellArea](../../com.aspose.cells/cellarea) öğelerini alır.

**Returns:**
com.aspose.cells.CellArea[]
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
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
### getFormula1(boolean isR1C1, boolean isLocal) {#getFormula1-boolean-boolean-}
```
public String getFormula1(boolean isR1C1, boolean isLocal)
```


Bu doğrulama ile ilişkili değeri veya ifadeyi alır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| isR1C1 | boolean | Formülün R1C1 olarak biçimlendirilip biçimlendirilmesi gerekip gerekmediği. |
| isLocal | boolean | Formülün yerel ayara göre biçimlendirilip biçimlendirilmesi gerekip gerekmediği. |

**Returns:**
java.lang.String - Bu doğrulama ile ilişkili değer veya ifade.
### getFormula1(boolean isR1C1, boolean isLocal, int row, int column) {#getFormula1-boolean-boolean-int-int-}
```
public String getFormula1(boolean isR1C1, boolean isLocal, int row, int column)
```


Belirli bir hücre için bu doğrulama ile ilişkili değeri veya ifadeyi alır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| isR1C1 | boolean | Formülün R1C1 olarak biçimlendirilip biçimlendirilmesi gerekip gerekmediği. |
| isLocal | boolean | Formülün yerel ayara göre biçimlendirilip biçimlendirilmesi gerekip gerekmediği. |
| satır | int | Satır indeksi. |
| sütun | int | Sütun indeksi. |

**Returns:**
java.lang.String - Bu doğrulama ile ilişkili değer veya ifade.
### getFormula2() {#getFormula2--}
```
public String getFormula2()
```


Veri doğrulama ile ilişkili değeri veya ifadeyi temsil eder.

**Returns:**
java.lang.String
### getFormula2(boolean isR1C1, boolean isLocal) {#getFormula2-boolean-boolean-}
```
public String getFormula2(boolean isR1C1, boolean isLocal)
```


Bu doğrulama ile ilişkili değeri veya ifadeyi alır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| isR1C1 | boolean | Formülün R1C1 olarak biçimlendirilip biçimlendirilmesi gerekip gerekmediği. |
| isLocal | boolean | Formülün yerel ayara göre biçimlendirilip biçimlendirilmesi gerekip gerekmediği. |

**Returns:**
java.lang.String - Bu doğrulama ile ilişkili değer veya ifade.
### getFormula2(boolean isR1C1, boolean isLocal, int row, int column) {#getFormula2-boolean-boolean-int-int-}
```
public String getFormula2(boolean isR1C1, boolean isLocal, int row, int column)
```


Belirli bir hücre için bu doğrulama ile ilişkili değeri veya ifadeyi alır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| isR1C1 | boolean | Formülün R1C1 olarak biçimlendirilip biçimlendirilmesi gerekip gerekmediği. |
| isLocal | boolean | Formülün yerel ayara göre biçimlendirilip biçimlendirilmesi gerekip gerekmediği. |
| satır | int | Satır indeksi. |
| sütun | int | Sütun indeksi. |

**Returns:**
java.lang.String - Bu doğrulama ile ilişkili değer veya ifade.
### getIgnoreBlank() {#getIgnoreBlank--}
```
public boolean getIgnoreBlank()
```


Aralık veri doğrulaması tarafından boş değerlerin izin verilip verilmediğini gösterir.

**Returns:**
boolean
### getInCellDropDown() {#getInCellDropDown--}
```
public boolean getInCellDropDown()
```


Veri doğrulamanın kabul edilebilir değerleri içeren bir açılır liste gösterip göstermediğini belirtir.

**Returns:**
boolean
### getInputMessage() {#getInputMessage--}
```
public String getInputMessage()
```


Veri doğrulama giriş mesajını temsil eder.

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
java.lang.Object - Belirtilen hücre için bu doğrulamanın listesini üretmek üzere değer. Liste bir aralığa referans veriyorsa, döndürülen değer bir [ReferredArea](../../com.aspose.cells/referredarea) nesnesi olacaktır; Aksi takdirde döndürülen değer null, object[] veya basit bir nesne olabilir.
### getOperator() {#getOperator--}
```
public int getOperator()
```


Veri doğrulama için operatörü temsil eder.

Bakınız [OperatorType](../../com.aspose.cells/operatortype).

**Returns:**
int
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
### getType() {#getType--}
```
public int getType()
```


Veri doğrulama türünü temsil eder.

Bakınız [ValidationType](../../com.aspose.cells/validationtype).

**Returns:**
int
### getValue(int row, int column, boolean isValue1) {#getValue-int-int-boolean-}
```
public Object getValue(int row, int column, boolean isValue1)
```


Belirli hücredeki doğrulamanın değerini al.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| satır | int | Satır indeksi. |
| sütun | int | Sütun indeksi. |
| isValue1 | boolean | İlk değerin alınıp alınmadığını gösterir. |

**Returns:**
java.lang.Object - 
### getValue1() {#getValue1--}
```
public Object getValue1()
```


Veri doğrulama ile ilişkili ilk değeri temsil eder.

**Returns:**
java.lang.Object
### getValue2() {#getValue2--}
```
public Object getValue2()
```


Veri doğrulama ile ilişkili ikinci değeri temsil eder.

**Returns:**
java.lang.Object
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

### removeArea(CellArea cellArea) {#removeArea-com.aspose.cells.CellArea-}
```
public void removeArea(CellArea cellArea)
```


Aralıktaki doğrulama ayarlarını kaldır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| cellArea | [CellArea](../../com.aspose.cells/cellarea) | Bu doğrulama ayarlarının kaldırılması gereken alanlar. |

### removeAreas(CellArea[] areas) {#removeAreas-com.aspose.cells.CellArea---}
```
public void removeAreas(CellArea[] areas)
```


Bu doğrulamayı verilen alanlardan kaldırır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| areas | [CellArea\[\]](../../com.aspose.cells/cellarea) | Bu doğrulama ayarlarının kaldırılması gereken alanlar. |

### setAlertStyle(int value) {#setAlertStyle-int-}
```
public void setAlertStyle(int value)
```


Doğrulama uyarı stilini temsil eder.

Bakınız [ValidationAlertType](../../com.aspose.cells/validationalerttype).

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

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

### setFormula1(String formula, boolean isR1C1, boolean isLocal) {#setFormula1-java.lang.String-boolean-boolean-}
```
public void setFormula1(String formula, boolean isR1C1, boolean isLocal)
```


Bu doğrulama ile ilişkili değeri veya ifadeyi ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| formula | java.lang.String | Bu biçim koşuluyla ilişkili değer veya ifade. |
| isR1C1 | boolean | Formülün R1C1 formülü olup olmadığı. |
| isLocal | boolean | Formülün yerel ayara göre biçimlendirilip biçimlendirilmediği. |

### setFormula2(String value) {#setFormula2-java.lang.String-}
```
public void setFormula2(String value)
```


Veri doğrulama ile ilişkili değeri veya ifadeyi temsil eder.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

### setFormula2(String formula, boolean isR1C1, boolean isLocal) {#setFormula2-java.lang.String-boolean-boolean-}
```
public void setFormula2(String formula, boolean isR1C1, boolean isLocal)
```


Bu doğrulama ile ilişkili değeri veya ifadeyi ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| formula | java.lang.String | Bu biçim koşuluyla ilişkili değer veya ifade. |
| isR1C1 | boolean | Formülün R1C1 formülü olup olmadığı. |
| isLocal | boolean | Formülün yerel ayara göre biçimlendirilip biçimlendirilmediği. |

### setIgnoreBlank(boolean value) {#setIgnoreBlank-boolean-}
```
public void setIgnoreBlank(boolean value)
```


Aralık veri doğrulaması tarafından boş değerlerin izin verilip verilmediğini gösterir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setInCellDropDown(boolean value) {#setInCellDropDown-boolean-}
```
public void setInCellDropDown(boolean value)
```


Veri doğrulamanın kabul edilebilir değerleri içeren bir açılır liste gösterip göstermediğini belirtir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setInputMessage(String value) {#setInputMessage-java.lang.String-}
```
public void setInputMessage(String value)
```


Veri doğrulama giriş mesajını temsil eder.

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

Bakınız [OperatorType](../../com.aspose.cells/operatortype).

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

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

### setType(int value) {#setType-int-}
```
public void setType(int value)
```


Veri doğrulama türünü temsil eder.

Bakınız [ValidationType](../../com.aspose.cells/validationtype).

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setValue1(Object value) {#setValue1-java.lang.Object-}
```
public void setValue1(Object value)
```


Veri doğrulama ile ilişkili ilk değeri temsil eder.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.Object |  |

### setValue2(Object value) {#setValue2-java.lang.Object-}
```
public void setValue2(Object value)
```


Veri doğrulama ile ilişkili ikinci değeri temsil eder.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.Object |  |

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

