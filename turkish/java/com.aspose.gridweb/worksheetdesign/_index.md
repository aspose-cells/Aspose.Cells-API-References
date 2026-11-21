---
title: "WorksheetDesign"
second_title: "Aspose.Cells for Java API Referansı"
description: "WebWorksheet sınıfından miras alınmıştır."
type: docs
url: /tr/java/com.aspose.gridweb/worksheetdesign/
---

**Inheritance:**
java.lang.Object, [com.aspose.gridweb.Control](../../com.aspose.gridweb/control), [com.aspose.gridweb.WebWorksheet](../../com.aspose.gridweb/webworksheet)
```
public class WorksheetDesign extends WebWorksheet
```

WebWorksheet'ten kalıtılmıştır. Yalnızca tasarım zamanında kullanılır.
## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [WorksheetDesign()](#WorksheetDesign--) | Varsayılan yapıcı. |
| [WorksheetDesign(MainWeb mw, GridWorksheet gwk)](#WorksheetDesign-com.aspose.gridweb.MainWeb-com.aspose.gridweb.GridWorksheet-) | MainWeb ve GridWorksheet ile oluşturucu |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [autoFitColumn(int columnIndex)](#autoFitColumn-int-) | Sütun genişliğini otomatik olarak ayarlar. |
| [autoFitColumn(int columnIndex, int startRow, int endRow)](#autoFitColumn-int-int-int-) | Sütun genişliğini otomatik olarak ayarlar. |
| [cancelNewBindRow()](#cancelNewBindRow--) | Yeni eklenen bağlama satırını iptal eder ve siler. |
| [commitNewBindRow()](#commitNewBindRow--) | Yeni eklenen bağlama satırını onaylar ve veri kaynağına ekler. |
| [copy(WebWorksheet source)](#copy-com.aspose.gridweb.WebWorksheet-) | Başka bir çalışma sayfası nesnesinden kopyalar. |
| [createAutoGenratedColumns()](#createAutoGenratedColumns--) | Çalışma sayfası için bir veri kaynağı ayarladıktan sonra, bağlama sütunlarını otomatik olarak oluşturmak için bu yöntemi çağırın. |
| [createNewBindRow()](#createNewBindRow--) | Yeni bir bağlama satırı oluşturur ve veri kaynağına bağlar. |
| [createSubtotal(int columnNameRowIndex, int dataRows, int groupByColumnIndex, int subtotalFunction, int[] subtotalColumnIndexList, String functionLabel, GridTableItemStyle grandCellStyle, GridTableItemStyle subtotalCellStyle, int numberType, String customString)](#createSubtotal-int-int-int-int-int---java.lang.String-com.aspose.gridweb.GridTableItemStyle-com.aspose.gridweb.GridTableItemStyle-int-java.lang.String-) | Sayfada ara toplam oluşturur. |
| [dataBind()](#dataBind--) | Sayfayı DataSource'a bağla. |
| [deleteBindRow(int rowNum)](#deleteBindRow-int-) | Bir bağlama satırını siler. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [freezePanes(int row, int column, int freezedRows, int freezedColumns)](#freezePanes-int-int-int-int-) | Çalışma sayfasındaki belirtilen hücrede bölmeleri dondurur. |
| [getBindStartColumn()](#getBindStartColumn--) | Veri bağlama modunda, BindStartRow ve BindStartColumn, ızgaranın veri kaynağına bağlanacağı konumu gösterir. |
| [getBindStartRow()](#getBindStartRow--) | Veri bağlama modunda, BindStartRow ve BindStartColumn, ızgaranın veri kaynağına bağlanacağı konumu gösterir. |
| [getBindingSource()](#getBindingSource--) | Çalışma zamanında gerçek bağlanan veri kaynağı nesnesi. |
| [getClass()](#getClass--) |  |
| [getCurrentBindRows()](#getCurrentBindRows--) | Veri bağlama modunda bağlama satır sayısını alır. |
| [getDataMember()](#getDataMember--) | Çok üyeli DataSource'dan DataMember'ı alır. |
| [getDataSource()](#getDataSource--) | DataSource'ı alır. |
| [getEnableCreateBindColumnHeader()](#getEnableCreateBindColumnHeader--) | Veri bağlama modunda, sayfada bağlama sütun başlık açıklamalarının oluşturulup oluşturulmayacağını gösterir. |
| [getIndex()](#getIndex--) | Çalışma sayfaları içinde kendi indeksini alır. |
| [getName()](#getName--) | Sayfanın adını alır. |
| [getUniqueID()](#getUniqueID--) | Denetimde UniqueID'yi alır |
| [getValidations()](#getValidations--) | Çalışma sayfasındaki veri doğrulama ayarları koleksiyonunu alır. |
| [getVisible()](#getVisible--) | Bu sayfanın adının denetimin sayfa sekmelerinde gösterilip gösterilmediğini belirtir. |
| [groupRows(int firstIndex, int lastIndex)](#groupRows-int-int-) | Satırları gruplar. |
| [groupRows(int firstIndex, int lastIndex, boolean isHidden)](#groupRows-int-int-boolean-) | Satırları gruplar. |
| [hashCode()](#hashCode--) |  |
| [isProtected()](#isProtected--) | Çalışma sayfasının korumalı olup olmadığını alır. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAllCellsEditable()](#setAllCellsEditable--) | Tüm hücreleri düzenlenebilir yapar. bu bir genişletilmiş özelliktir |
| [setAllCellsReadonly()](#setAllCellsReadonly--) | Tüm hücreleri salt okunur yapar. bu bir genişletilmiş özelliktir; bu özelliğin gerçek hücrede tutulamayacağını unutmayın, korumayı sürdürmek istiyorsanız lütfen setProtect kullanın |
| [setBindStartColumn(int value)](#setBindStartColumn-int-) | Veri bağlama modunda, BindStartRow ve BindStartColumn, ızgaranın veri kaynağına bağlanacağı konumu gösterir. |
| [setBindStartRow(int value)](#setBindStartRow-int-) | Veri bağlama modunda, BindStartRow ve BindStartColumn, ızgaranın veri kaynağına bağlanacağı konumu gösterir. |
| [setCurrentBindRows(int value)](#setCurrentBindRows-int-) | Veri bağlama modunda bağlama satır sayısını alır. |
| [setDataMember(String value)](#setDataMember-java.lang.String-) | Çok üyeli DataSource'dan DataMember'ı ayarlar. |
| [setDataSource(Object value)](#setDataSource-java.lang.Object-) | DataSource'ı ayarlar. |
| [setEditableRange(int startRow, int startColumn, int rows, int columns)](#setEditableRange-int-int-int-int-) | Bir hücre aralığını düzenlenebilir yapar. http://docs.aspose.com:8082/docs/display/cellsnet/Protecting+Cells SetAllCellsReadonly yöntemini çağırarak tüm hücreleri salt okunur yapın. |
| [setEnableCreateBindColumnHeader(boolean value)](#setEnableCreateBindColumnHeader-boolean-) | Veri bağlama modunda, sayfada bağlama sütun başlık açıklamalarının oluşturulup oluşturulmayacağını gösterir. |
| [setName(String value)](#setName-java.lang.String-) | Sayfanın adını ayarlar. |
| [setProtected(boolean value)](#setProtected-boolean-) | Çalışma sayfasının korumalı olup olmadığını ayarlar. |
| [setReadonlyRange(int startRow, int startColumn, int rows, int columns)](#setReadonlyRange-int-int-int-int-) | Bir hücre aralığını salt okunur yapar. http://docs.aspose.com:8082/docs/display/cellsnet/Protecting+Cells Önce SetAllCellsEditable yöntemini çağırarak tüm hücreleri düzenlenebilir yapın. |
| [setVisible(boolean value)](#setVisible-boolean-) | Bu sayfanın adının denetimin sayfa sekmelerinde gösterilip gösterilmediğini belirtir. |
| [toString()](#toString--) |  |
| [unfreezePanes()](#unfreezePanes--) | Çalışma sayfasındaki bölmeleri dondurmayı kaldırır. |
| [ungroupRows(int firstIndex, int lastIndex)](#ungroupRows-int-int-) | Satırların gruplamasını kaldırır. |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### WorksheetDesign() {#WorksheetDesign--}
```
public WorksheetDesign()
```


Varsayılan yapıcı.

### WorksheetDesign(MainWeb mw, GridWorksheet gwk) {#WorksheetDesign-com.aspose.gridweb.MainWeb-com.aspose.gridweb.GridWorksheet-}
```
public WorksheetDesign(MainWeb mw, GridWorksheet gwk)
```


MainWeb ve GridWorksheet ile oluşturucu

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| mw | [MainWeb](../../com.aspose.gridweb/mainweb) |  |
| gwk | [GridWorksheet](../../com.aspose.gridweb/gridworksheet) |  |

### autoFitColumn(int columnIndex) {#autoFitColumn-int-}
```
public void autoFitColumn(int columnIndex)
```


Sütun genişliğini otomatik olarak ayarlar.

**Remarks**

AutoFitColumn, kesin olmayan bir işlevdir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| columnIndex | int | Sütun indeksi. |

### autoFitColumn(int columnIndex, int startRow, int endRow) {#autoFitColumn-int-int-int-}
```
public void autoFitColumn(int columnIndex, int startRow, int endRow)
```


Sütun genişliğini otomatik ayarlar. Bu yöntem, sütundaki startRow ile endRow arasındaki hücre aralığındaki içeriğe göre bir sütunu otomatik ayarlar. AutoFitColumn, kesin olmayan bir işlevdir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| columnIndex | int | sütun indeksi, sıfır tabanlı |
| startRow | int | başlangıç satır indeksi, sıfır tabanlı |
| endRow | int | bitiş satır indeksi, sıfır tabanlı |

### cancelNewBindRow() {#cancelNewBindRow--}
```
public int cancelNewBindRow()
```


Yeni eklenen bağlama satırını iptal eder ve siler.

**Returns:**
int - Satır indeksi. Yeni oluşturulan bağlama satırı yoksa, -1 döndürür.
### commitNewBindRow() {#commitNewBindRow--}
```
public int commitNewBindRow()
```


Yeni eklenen bağlama satırını onaylar ve veri kaynağına ekler.

**Returns:**
int - Yeni satırın satır indeksi. Satır oluşturulmazsa, -1 döndürür.
### copy(WebWorksheet source) {#copy-com.aspose.gridweb.WebWorksheet-}
```
public void copy(WebWorksheet source)
```


Başka bir çalışma sayfası nesnesinden kopyalar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| source | [WebWorksheet](../../com.aspose.gridweb/webworksheet) | Diğer sayfa. |

### createAutoGenratedColumns() {#createAutoGenratedColumns--}
```
public void createAutoGenratedColumns()
```


Çalışma sayfası için bir veri kaynağı ayarladıktan sonra, bağlama sütunlarını otomatik olarak oluşturmak için bu yöntemi çağırın.

### createNewBindRow() {#createNewBindRow--}
```
public int createNewBindRow()
```


Yeni bir bağlama satırı oluşturur ve veri kaynağına bağlar.

**Returns:**
int - Yeni satırın satır indeksi. Satır oluşturulmazsa, -1 döndürür.
### createSubtotal(int columnNameRowIndex, int dataRows, int groupByColumnIndex, int subtotalFunction, int[] subtotalColumnIndexList, String functionLabel, GridTableItemStyle grandCellStyle, GridTableItemStyle subtotalCellStyle, int numberType, String customString) {#createSubtotal-int-int-int-int-int---java.lang.String-com.aspose.gridweb.GridTableItemStyle-com.aspose.gridweb.GridTableItemStyle-int-java.lang.String-}
```
public void createSubtotal(int columnNameRowIndex, int dataRows, int groupByColumnIndex, int subtotalFunction, int[] subtotalColumnIndexList, String functionLabel, GridTableItemStyle grandCellStyle, GridTableItemStyle subtotalCellStyle, int numberType, String customString)
```


Sayfada ara toplam oluşturur.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| columnNameRowIndex | int | Sütun adı satırının satır indeksi. |
| dataRows | int | Veri satırlarının sayısı. |
| groupByColumnIndex | int | Gruplanacak sütunun sütun indeksi. |
| subtotalFunction | int | [SubtotalFunction](../../com.aspose.gridweb/subtotalfunction). Ara toplam işlevi türü. |
| subtotalColumnIndexList | int[] | Ara toplam yapılacak sütun indeksleri. |
| functionLabel | java.lang.String | Ara toplam işlevinin etiketi. |
| grandCellStyle | [GridTableItemStyle](../../com.aspose.gridweb/gridtableitemstyle) | Genel toplam satırının stili. |
| subtotalCellStyle | [GridTableItemStyle](../../com.aspose.gridweb/gridtableitemstyle) | Ara toplam satırının stili. |
| numberType | int | [NumberType](../../com.aspose.gridweb/numbertype). Ara toplam sonuç hücrelerinin sayı türü. |
| customString | java.lang.String | Ara toplam sonuç hücrelerinin özel biçim dizesi. Null olabilir. |

### dataBind() {#dataBind--}
```
public void dataBind()
```


Sayfayı DataSource'a bağla.

### deleteBindRow(int rowNum) {#deleteBindRow-int-}
```
public int deleteBindRow(int rowNum)
```


Bir bağlama satırını siler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| rowNum | int | Satır indeksi. |

**Returns:**
int - Silinen satır indeksi. Bağlama satırı silinmezse, -1 döndürür.
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
### freezePanes(int row, int column, int freezedRows, int freezedColumns) {#freezePanes-int-int-int-int-}
```
public void freezePanes(int row, int column, int freezedRows, int freezedColumns)
```


Çalışma sayfasındaki belirtilen hücrede bölmeleri dondurur.

**Remarks**

Satır indeksi ve sütun indeksi aynı anda sıfır olamaz. Satır sayısı ve sütun sayısı da aynı anda sıfır olamaz.

İlk iki parametre dondurulmuş konumu belirtir ve son iki parametre sol üst bölmede dondurulmuş alanı belirtir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| satır | int | Satır indeksi. |
| sütun | int | Sütun indeksi. |
| freezedRows | int | Üst bölmede görünen satır sayısı, satır indeksinden fazla olamaz. |
| freezedColumns | int | Sol bölmede görünen sütun sayısı, sütun indeksinden fazla olamaz. |

### getBindStartColumn() {#getBindStartColumn--}
```
public int getBindStartColumn()
```


Veri bağlama modunda, BindStartRow ve BindStartColumn, ızgaranın veri kaynağına bağlanacağı konumu gösterir.

**Returns:**
int
### getBindStartRow() {#getBindStartRow--}
```
public int getBindStartRow()
```


Veri bağlama modunda, BindStartRow ve BindStartColumn, ızgaranın veri kaynağına bağlanacağı konumu gösterir.

**Returns:**
int
### getBindingSource() {#getBindingSource--}
```
public Iterable getBindingSource()
```


Çalışma zamanında gerçek bağlama veri kaynağı nesnesi. DataSource özelliği bir DataSet, DataTable veya DataView nesnesi olduğunda, bu bir DataView nesnesidir.

**Returns:**
java.lang.Iterable
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getCurrentBindRows() {#getCurrentBindRows--}
```
public int getCurrentBindRows()
```


Veri bağlama modunda bağlama satır sayısını alır.

**Returns:**
int
### getDataMember() {#getDataMember--}
```
public String getDataMember()
```


Çok üyeli DataSource'dan DataMember'ı alır. Genel olarak bir DataSet'in DataTable nesnesini temsil eder.

**Returns:**
java.lang.String
### getDataSource() {#getDataSource--}
```
public Object getDataSource()
```


DataSource'ı alır. Genel olarak bir DataSet nesnesidir.

**Returns:**
java.lang.Object
### getEnableCreateBindColumnHeader() {#getEnableCreateBindColumnHeader--}
```
public boolean getEnableCreateBindColumnHeader()
```


Veri bağlama modunda, sayfada bağlama sütun başlık açıklamalarının oluşturulup oluşturulmayacağını gösterir.

**Returns:**
boolean
### getIndex() {#getIndex--}
```
public int getIndex()
```


Çalışma sayfaları içinde kendi indeksini alır.

**Returns:**
int
### getName() {#getName--}
```
public String getName()
```


Sayfanın adını alır.

**Returns:**
java.lang.String
### getUniqueID() {#getUniqueID--}
```
public String getUniqueID()
```


Denetimde UniqueID'yi alır

**Returns:**
java.lang.String
### getValidations() {#getValidations--}
```
public GridValidationCollection getValidations()
```


Çalışma sayfasındaki veri doğrulama ayarları koleksiyonunu alır.

**Returns:**
[GridValidationCollection](../../com.aspose.gridweb/gridvalidationcollection)
### getVisible() {#getVisible--}
```
public boolean getVisible()
```


Bu sayfanın adının denetimin sayfa sekmelerinde gösterilip gösterilmediğini belirtir.

**Returns:**
boolean
### groupRows(int firstIndex, int lastIndex) {#groupRows-int-int-}
```
public void groupRows(int firstIndex, int lastIndex)
```


Satırları gruplar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| firstIndex | int | Gruplanacak ilk satır indeksi. |
| lastIndex | int | Gruplanacak son satır indeksi. |

### groupRows(int firstIndex, int lastIndex, boolean isHidden) {#groupRows-int-int-boolean-}
```
public void groupRows(int firstIndex, int lastIndex, boolean isHidden)
```


Satırları gruplar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| firstIndex | int | Gruplanacak ilk satır indeksi. |
| lastIndex | int | Gruplanacak son satır indeksi. |
| isHidden | boolean | Gruplanan satırların gizli olup olmadığını belirtir. |

### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isProtected() {#isProtected--}
```
public boolean isProtected()
```


Çalışma sayfasının korumalı olup olmadığını alır. Bir çalışma sayfası korunduğunda, IsLocked özelliği false olan hücre dışındaki tüm hücreler düzenlenemez.

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




### setAllCellsEditable() {#setAllCellsEditable--}
```
public void setAllCellsEditable()
```


Tüm hücreleri düzenlenebilir yapar. bu bir genişletilmiş özelliktir

### setAllCellsReadonly() {#setAllCellsReadonly--}
```
public void setAllCellsReadonly()
```


Tüm hücreleri salt okunur yapar. bu bir genişletilmiş özelliktir; bu özelliğin gerçek hücrede tutulamayacağını unutmayın, korumayı sürdürmek istiyorsanız lütfen setProtect kullanın

### setBindStartColumn(int value) {#setBindStartColumn-int-}
```
public void setBindStartColumn(int value)
```


Veri bağlama modunda, BindStartRow ve BindStartColumn, ızgaranın veri kaynağına bağlanacağı konumu gösterir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setBindStartRow(int value) {#setBindStartRow-int-}
```
public void setBindStartRow(int value)
```


Veri bağlama modunda, BindStartRow ve BindStartColumn, ızgaranın veri kaynağına bağlanacağı konumu gösterir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setCurrentBindRows(int value) {#setCurrentBindRows-int-}
```
public void setCurrentBindRows(int value)
```


Veri bağlama modunda bağlama satır sayısını alır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setDataMember(String value) {#setDataMember-java.lang.String-}
```
public void setDataMember(String value)
```


Çok üyeli DataSource'dan DataMember'ı ayarlar. Genel olarak bir DataSet'in DataTable nesnesini temsil eder.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

### setDataSource(Object value) {#setDataSource-java.lang.Object-}
```
public void setDataSource(Object value)
```


DataSource'ı ayarlar. Genel olarak bir DataSet nesnesidir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.Object |  |

### setEditableRange(int startRow, int startColumn, int rows, int columns) {#setEditableRange-int-int-int-int-}
```
public void setEditableRange(int startRow, int startColumn, int rows, int columns)
```


Bir hücre aralığını düzenlenebilir yapar. http://docs.aspose.com:8082/docs/display/cellsnet/Protecting+Cells Tüm hücreleri SetAllCellsReadonly metodunu çağırarak yalnızca okunur yapın. ardından bu yöntemi, düzenlenebilir olacak hücre aralığını belirtmek için çağırın.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| startRow | int | Aralığın başlangıç satırı. |
| startColumn | int | Aralığın başlangıç sütunu. |
| satırlar | int | Satır sayısı. |
| sütunlar | int | Sütun sayısı. |

### setEnableCreateBindColumnHeader(boolean value) {#setEnableCreateBindColumnHeader-boolean-}
```
public void setEnableCreateBindColumnHeader(boolean value)
```


Veri bağlama modunda, sayfada bağlama sütun başlık açıklamalarının oluşturulup oluşturulmayacağını gösterir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setName(String value) {#setName-java.lang.String-}
```
public void setName(String value)
```


Sayfanın adını ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

### setProtected(boolean value) {#setProtected-boolean-}
```
public void setProtected(boolean value)
```


Çalışma sayfasının korumalı olup olmadığını ayarlar. Bir çalışma sayfası korunduğunda, IsLocked özelliği false olan hücre dışındaki tüm hücreler düzenlenemez.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setReadonlyRange(int startRow, int startColumn, int rows, int columns) {#setReadonlyRange-int-int-int-int-}
```
public void setReadonlyRange(int startRow, int startColumn, int rows, int columns)
```


Bir hücre aralığını readonly yapar. http://docs.aspose.com:8082/docs/display/cellsnet/Protecting+Cells İlk olarak tüm hücreleri SetAllCellsEditable metodunu çağırarak düzenlenebilir yapın. ardından bu yöntemi, readonly olacak hücre aralığını belirtmek için çağırın.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| startRow | int | Aralığın başlangıç satırı. |
| startColumn | int | Aralığın başlangıç sütunu. |
| satırlar | int | Satır sayısı. |
| sütunlar | int | Sütun sayısı. |

### setVisible(boolean value) {#setVisible-boolean-}
```
public void setVisible(boolean value)
```


Bu sayfanın adının denetimin sayfa sekmelerinde gösterilip gösterilmediğini belirtir.

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
### unfreezePanes() {#unfreezePanes--}
```
public void unfreezePanes()
```


Çalışma sayfasındaki bölmeleri dondurmayı kaldırır.

### ungroupRows(int firstIndex, int lastIndex) {#ungroupRows-int-int-}
```
public void ungroupRows(int firstIndex, int lastIndex)
```


Satırların gruplamasını kaldırır.

**Remarks**

Yalnızca dış grup bilgilerini kaldırır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| firstIndex | int | Gruplanması kaldırılacak ilk satır indeksi. |
| lastIndex | int | Gruplanması kaldırılacak son satır indeksi. |

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

