---
title: "WorkbookDesigner"
second_title: "Aspose.Cells for Java API Referansı"
description: "Tasarımcı çalışma sayfasını temsil eden nesneyi kapsüller."
type: docs
url: /tr/java/com.aspose.cells/workbookdesigner/
---

**Inheritance:**
java.lang.Object
```
public class WorkbookDesigner
```

Tasarımcı çalışma sayfasını temsil eden nesneyi kapsüller.

**Example**

```
         //Create WorkbookDesigner object.
         WorkbookDesigner wd = new WorkbookDesigner();
         //Open the template file (which contains smart markers).
         wd.setWorkbook(new Workbook("SmartMarker_Designer.xls"));
 
         //Initialize your data from data source
         //DataSet ds = new DataSet();
 
 
         //Set the datatable as the data source.
         //wd.SetDataSource(dt);
         //Process the smart markers to fill the data into the worksheets.
         wd.process(true);
         //Save the excel file.
         wd.getWorkbook().save("outSmartMarker_Designer.xls");
```
## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [WorkbookDesigner()](#WorkbookDesigner--) | Yeni bir [WorkbookDesigner](../../com.aspose.cells/workbookdesigner) sınıfı örneği başlatır. |
| [WorkbookDesigner(Workbook workbook)](#WorkbookDesigner-com.aspose.cells.Workbook-) | Yeni bir [WorkbookDesigner](../../com.aspose.cells/workbookdesigner) sınıfı örneği başlatır. |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [clearDataSource()](#clearDataSource--) | Tüm veri kaynaklarını temizler. |
| [containsVariables()](#containsVariables--) | İlk çalışma sayfasının özel değişkenler içerip içermediğini gösterir. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getCalculateFormula()](#getCalculateFormula--) | Formüllerin hesaplanıp hesaplanmayacağını gösterir. |
| [getCallBack()](#getCallBack--) | Smartmarker işleme geri çağırma arayüzünü alır. |
| [getClass()](#getClass--) |  |
| [getEnableHeaderFooterMarkers()](#getEnableHeaderFooterMarkers--) | Üstbilgi/altbilginin akıllı işaretler içerip içermediğini ve birlikte işlenmesi gerektiğini gösterir. |
| [getLineByLine()](#getLineByLine--) | Akıllı işaretin satır satır işlenip işlenmeyeceğini gösterir. |
| [getRepeatFormulasWithSubtotal()](#getRepeatFormulasWithSubtotal--) | Ara toplam satırıyla birlikte formüllerin tekrarlanıp tekrarlanmayacağını gösterir. |
| [getSmartMarkers()](#getSmartMarkers--) | Bir elektronik tabloda bulunan akıllı işaretlerin koleksiyonunu döndürür. |
| [getSortDataSource()](#getSortDataSource--) | Veri kaynağının sıralanıp sıralanmayacağını gösterir. |
| [getUpdateEmptyStringAsNull()](#getUpdateEmptyStringAsNull--) | TRUE ise, değer "" olduğunda Null eklenecektir; |
| [getUpdateReference()](#getUpdateReference--) | Diğer çalışma sayfalarındaki referansların güncellenip güncellenmeyeceğini gösterir. |
| [getVariablesWorksheetName()](#getVariablesWorksheetName--) | Değişken akıllı işaret içeren çalışma sayfasının adını alır. |
| [getWorkbook()](#getWorkbook--) | [getWorkbook()](../../com.aspose.cells/workbookdesigner\#getWorkbook--) nesnesini alır. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [process()](#process--) | Akıllı işaretleri işler ve veri kaynağı değerlerini doldurur. |
| [process(boolean isPreserved)](#process-boolean-) | Akıllı işaretleri işler ve veri kaynağı değerlerini doldurur. |
| [process(Range range, boolean isPreserved)](#process-com.aspose.cells.Range-boolean-) | Akıllı işaretleri işler ve veri kaynağı değerlerini doldurur. |
| [process(int sheetIndex, boolean isPreserved)](#process-int-boolean-) | Akıllı işaretleri işler ve veri kaynağı değerlerini doldurur. |
| [setCalculateFormula(boolean value)](#setCalculateFormula-boolean-) | Formüllerin hesaplanıp hesaplanmayacağını gösterir. |
| [setCallBack(ISmartMarkerCallBack value)](#setCallBack-com.aspose.cells.ISmartMarkerCallBack-) | Akıllı işaret işleme için geri çağırma arayüzünü ayarlar. |
| [setContainsVariables(boolean value)](#setContainsVariables-boolean-) | İlk çalışma sayfasının özel değişkenler içerip içermediğini gösterir. |
| [setDataSource(String dataSource, ICellsDataTable cellsDataTable)](#setDataSource-java.lang.String-com.aspose.cells.ICellsDataTable-) | [ICellsDataTable](../../com.aspose.cells/icellsdatatable) nesnesinin veri kaynağını ayarlar. |
| [setDataSource(String variable, Object data)](#setDataSource-java.lang.String-java.lang.Object-) | Bir değişkene veri bağlamasını ayarlar. |
| [setDataSource(String dataSource, ResultSet rs)](#setDataSource-java.lang.String-java.sql.ResultSet-) | Veri kaynağını ayarla. |
| [setDataSource(String dataSource, ResultSet rs, int rowCount)](#setDataSource-java.lang.String-java.sql.ResultSet-int-) | Veri kaynağını ayarla. |
| [setDataSource(ResultSet rs)](#setDataSource-java.sql.ResultSet-) | Veri kaynağını ayarla. |
| [setEnableHeaderFooterMarkers(boolean value)](#setEnableHeaderFooterMarkers-boolean-) | Üstbilgi/altbilginin akıllı işaretler içerip içermediğini ve birlikte işlenmesi gerektiğini gösterir. |
| [setJsonDataSource(String name, String json)](#setJsonDataSource-java.lang.String-java.lang.String-) | JSON dize değerini akıllı işaretlerin veri kaynağı olarak ayarla. |
| [setLineByLine(boolean value)](#setLineByLine-boolean-) | Akıllı işaretin satır satır işlenip işlenmeyeceğini gösterir. |
| [setRepeatFormulasWithSubtotal(boolean value)](#setRepeatFormulasWithSubtotal-boolean-) | Ara toplam satırıyla birlikte formüllerin tekrarlanıp tekrarlanmayacağını gösterir. |
| [setSortDataSource(boolean value)](#setSortDataSource-boolean-) | Veri kaynağının sıralanıp sıralanmayacağını gösterir. |
| [setUpdateEmptyStringAsNull(boolean value)](#setUpdateEmptyStringAsNull-boolean-) | TRUE ise, değer "" olduğunda Null eklenecektir; |
| [setUpdateReference(boolean value)](#setUpdateReference-boolean-) | Diğer çalışma sayfalarındaki referansların güncellenip güncellenmeyeceğini gösterir. |
| [setVariablesWorksheetName(String value)](#setVariablesWorksheetName-java.lang.String-) | Değişken akıllı işaret içeren çalışma sayfasının adını ayarlar. |
| [setWorkbook(Workbook value)](#setWorkbook-com.aspose.cells.Workbook-) | [getWorkbook()](../../com.aspose.cells/workbookdesigner\#getWorkbook--) nesnesini ayarlar. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### WorkbookDesigner() {#WorkbookDesigner--}
```
public WorkbookDesigner()
```


Yeni bir [WorkbookDesigner](../../com.aspose.cells/workbookdesigner) sınıfı örneği başlatır.

### WorkbookDesigner(Workbook workbook) {#WorkbookDesigner-com.aspose.cells.Workbook-}
```
public WorkbookDesigner(Workbook workbook)
```


Yeni bir [WorkbookDesigner](../../com.aspose.cells/workbookdesigner) sınıfı örneği başlatır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| workbook | [Workbook](../../com.aspose.cells/workbook) | Şablon çalışma kitabı dosyası. |

### clearDataSource() {#clearDataSource--}
```
public void clearDataSource()
```


Tüm veri kaynaklarını temizler.

### containsVariables() {#containsVariables--}
```
public boolean containsVariables()
```


İlk çalışma sayfasının özel değişkenler içerip içermediğini gösterir.

**Remarks**

NOT: Bu üye artık kullanımdan kaldırılmıştır. Bunun yerine lütfen WorkbookDesigner.VariablesWorksheetName özelliğini kullanın. Bu özellik Eylül 2025 itibarıyla 3 ay içinde kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

**Returns:**
boolean
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
### getCalculateFormula() {#getCalculateFormula--}
```
public boolean getCalculateFormula()
```


Formüllerin hesaplanıp hesaplanmayacağını gösterir.

**Returns:**
boolean
### getCallBack() {#getCallBack--}
```
public ISmartMarkerCallBack getCallBack()
```


Smartmarker işleme geri çağırma arayüzünü alır.

**Returns:**
[ISmartMarkerCallBack](../../com.aspose.cells/ismartmarkercallback)
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getEnableHeaderFooterMarkers() {#getEnableHeaderFooterMarkers--}
```
public boolean getEnableHeaderFooterMarkers()
```


Üstbilgi/altbilginin akıllı işaretler içerip içermediğini ve birlikte işlenmesi gerektiğini gösterir.

**Returns:**
boolean
### getLineByLine() {#getLineByLine--}
```
public boolean getLineByLine()
```


Akıllı işaretin satır satır işlenip işlenmeyeceğini gösterir.

**Remarks**

NOT: Bu sınıf artık kullanımdan kaldırılmıştır. Bunun yerine lütfen aralık akıllı işaretlerini kullanın. Bu özellik Temmuz 2025 itibarıyla 12 ay içinde kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

**Returns:**
boolean
### getRepeatFormulasWithSubtotal() {#getRepeatFormulasWithSubtotal--}
```
public boolean getRepeatFormulasWithSubtotal()
```


Ara toplam satırıyla birlikte formüllerin tekrarlanıp tekrarlanmayacağını gösterir.

**Returns:**
boolean
### getSmartMarkers() {#getSmartMarkers--}
```
public String[] getSmartMarkers()
```


Bir elektronik tabloda bulunan akıllı işaretlerin koleksiyonunu döndürür.

**Remarks**

Her çağrıda bir dize dizisi oluşturulur. Dizi sıralanır ve yinelenen değerler kaldırılır.

**Returns:**
java.lang.String[] - Akıllı işaretlerin bir koleksiyonu
### getSortDataSource() {#getSortDataSource--}
```
public boolean getSortDataSource()
```


Veri kaynağının sıralanıp sıralanmayacağını gösterir.

**Remarks**

NOT: Bu özellik artık kullanımdan kaldırılmıştır. Bu özellik Ekim 2026 itibarıyla 12 ay içinde kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler. Akıllı işaret artan ve azalan parametreler içeriyorsa JSON veri kaynağı sıralanacaktır.

**Returns:**
boolean
### getUpdateEmptyStringAsNull() {#getUpdateEmptyStringAsNull--}
```
public boolean getUpdateEmptyStringAsNull()
```


TRUE ise, değer "" olduğunda Null eklenecektir;

**Returns:**
boolean
### getUpdateReference() {#getUpdateReference--}
```
public boolean getUpdateReference()
```


Diğer çalışma sayfalarındaki referansların güncellenip güncellenmeyeceğini gösterir.

**Returns:**
boolean
### getVariablesWorksheetName() {#getVariablesWorksheetName--}
```
public String getVariablesWorksheetName()
```


Değişken akıllı işaret içeren çalışma sayfasının adını alır.

**Returns:**
java.lang.String
### getWorkbook() {#getWorkbook--}
```
public Workbook getWorkbook()
```


[getWorkbook()](../../com.aspose.cells/workbookdesigner\#getWorkbook--) nesnesini alır.

**Returns:**
[Workbook](../../com.aspose.cells/workbook)
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




### process() {#process--}
```
public void process()
```


Akıllı işaretleri işler ve veri kaynağı değerlerini doldurur.

### process(boolean isPreserved) {#process-boolean-}
```
public void process(boolean isPreserved)
```


Akıllı işaretleri işler ve veri kaynağı değerlerini doldurur.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| isPreserved | boolean | Tanımlanamayan akıllı işaret korunuyorsa True. |

### process(Range range, boolean isPreserved) {#process-com.aspose.cells.Range-boolean-}
```
public void process(Range range, boolean isPreserved)
```


Akıllı işaretleri işler ve veri kaynağı değerlerini doldurur.

**Remarks**

NOT: Bu sınıf artık kullanımdan kaldırılmıştır. Bunun yerine lütfen Range akıllı işaretlerini kullanın. Bu özellik Temmuz 2025 itibarıyla 12 ay içinde kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| range | [Range](../../com.aspose.cells/range) | İşlenecek aralık |
| isPreserved | boolean | Tanımlanamayan akıllı işaret korunuyorsa True. |

### process(int sheetIndex, boolean isPreserved) {#process-int-boolean-}
```
public void process(int sheetIndex, boolean isPreserved)
```


Akıllı işaretleri işler ve veri kaynağı değerlerini doldurur.

**Remarks**

Bu yöntem çalışma sayfası düzeyinde çalışır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| sheetIndex | int | Çalışma sayfası indeksi. |
| isPreserved | boolean | Tanımlanamayan akıllı işaret korunuyorsa True. |

### setCalculateFormula(boolean value) {#setCalculateFormula-boolean-}
```
public void setCalculateFormula(boolean value)
```


Formüllerin hesaplanıp hesaplanmayacağını gösterir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setCallBack(ISmartMarkerCallBack value) {#setCallBack-com.aspose.cells.ISmartMarkerCallBack-}
```
public void setCallBack(ISmartMarkerCallBack value)
```


Akıllı işaret işleme için geri çağırma arayüzünü ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [ISmartMarkerCallBack](../../com.aspose.cells/ismartmarkercallback) |  |

### setContainsVariables(boolean value) {#setContainsVariables-boolean-}
```
public void setContainsVariables(boolean value)
```


İlk çalışma sayfasının özel değişkenler içerip içermediğini gösterir.

**Remarks**

NOT: Bu üye artık kullanımdan kaldırılmıştır. Bunun yerine lütfen WorkbookDesigner.VariablesWorksheetName özelliğini kullanın. Bu özellik Eylül 2025 itibarıyla 3 ay içinde kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setDataSource(String dataSource, ICellsDataTable cellsDataTable) {#setDataSource-java.lang.String-com.aspose.cells.ICellsDataTable-}
```
public void setDataSource(String dataSource, ICellsDataTable cellsDataTable)
```


[ICellsDataTable](../../com.aspose.cells/icellsdatatable) nesnesinin veri kaynağını ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| dataSource | java.lang.String | Veri kaynağının adı. |
| cellsDataTable | [ICellsDataTable](../../com.aspose.cells/icellsdatatable) | veri tablosu. |

### setDataSource(String variable, Object data) {#setDataSource-java.lang.String-java.lang.Object-}
```
public void setDataSource(String variable, Object data)
```


Bir değişkene veri bağlamasını ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değişken | java.lang.String | Akıllı işaretleyici kullanılarak oluşturulan değişken adı. |
| veri | java.lang.Object | Kaynak veri. |

### setDataSource(String dataSource, ResultSet rs) {#setDataSource-java.lang.String-java.sql.ResultSet-}
```
public void setDataSource(String dataSource, ResultSet rs)
```


Veri kaynağını ayarla.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| dataSource | java.lang.String | Veri kaynağının adı. |
| rs | java.sql.ResultSet | Sonuç kümesi. |

### setDataSource(String dataSource, ResultSet rs, int rowCount) {#setDataSource-java.lang.String-java.sql.ResultSet-int-}
```
public void setDataSource(String dataSource, ResultSet rs, int rowCount)
```


Veri kaynağını ayarla.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| dataSource | java.lang.String | Veri kaynağının adı. |
| rs | java.sql.ResultSet | Sonuç kümesi. |
| rowCount | int | Verilen sonuç kümesinin veri sayısı. Tam satır sayısı ya da -1 olmalıdır; Eğer sonuç kümesi sadece ileriye doğru ise, kullanıcı burada tam satır sayısını vermelidir, aksi takdirde akıllı işaretleyicinin "noadd" ayarı yapılmadığında akıllı doğru işlenmeyebilir. |

### setDataSource(ResultSet rs) {#setDataSource-java.sql.ResultSet-}
```
public void setDataSource(ResultSet rs)
```


Veri kaynağını ayarla.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| rs | java.sql.ResultSet | Sonuç kümesi. |

### setEnableHeaderFooterMarkers(boolean value) {#setEnableHeaderFooterMarkers-boolean-}
```
public void setEnableHeaderFooterMarkers(boolean value)
```


Üstbilgi/altbilginin akıllı işaretler içerip içermediğini ve birlikte işlenmesi gerektiğini gösterir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setJsonDataSource(String name, String json) {#setJsonDataSource-java.lang.String-java.lang.String-}
```
public void setJsonDataSource(String name, String json)
```


JSON dize değerini akıllı işaretlerin veri kaynağı olarak ayarla.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| ad | java.lang.String | Tablonun adı. JSON değerinin bir nesneyi temsil etmesi durumunda, null olabilir. |
| json | java.lang.String | Json dizesinin değeri. |

### setLineByLine(boolean value) {#setLineByLine-boolean-}
```
public void setLineByLine(boolean value)
```


Akıllı işaretin satır satır işlenip işlenmeyeceğini gösterir.

**Remarks**

NOT: Bu sınıf artık kullanımdan kaldırılmıştır. Bunun yerine lütfen aralık akıllı işaretlerini kullanın. Bu özellik Temmuz 2025 itibarıyla 12 ay içinde kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setRepeatFormulasWithSubtotal(boolean value) {#setRepeatFormulasWithSubtotal-boolean-}
```
public void setRepeatFormulasWithSubtotal(boolean value)
```


Ara toplam satırıyla birlikte formüllerin tekrarlanıp tekrarlanmayacağını gösterir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setSortDataSource(boolean value) {#setSortDataSource-boolean-}
```
public void setSortDataSource(boolean value)
```


Veri kaynağının sıralanıp sıralanmayacağını gösterir.

**Remarks**

NOT: Bu özellik artık kullanımdan kaldırılmıştır. Bu özellik Ekim 2026 itibarıyla 12 ay içinde kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler. Akıllı işaret artan ve azalan parametreler içeriyorsa JSON veri kaynağı sıralanacaktır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setUpdateEmptyStringAsNull(boolean value) {#setUpdateEmptyStringAsNull-boolean-}
```
public void setUpdateEmptyStringAsNull(boolean value)
```


TRUE ise, değer "" olduğunda Null eklenecektir;

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setUpdateReference(boolean value) {#setUpdateReference-boolean-}
```
public void setUpdateReference(boolean value)
```


Diğer çalışma sayfalarındaki referansların güncellenip güncellenmeyeceğini gösterir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setVariablesWorksheetName(String value) {#setVariablesWorksheetName-java.lang.String-}
```
public void setVariablesWorksheetName(String value)
```


Değişken akıllı işaret içeren çalışma sayfasının adını ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

### setWorkbook(Workbook value) {#setWorkbook-com.aspose.cells.Workbook-}
```
public void setWorkbook(Workbook value)
```


[getWorkbook()](../../com.aspose.cells/workbookdesigner\#getWorkbook--) nesnesini ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [Workbook](../../com.aspose.cells/workbook) |  |

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

