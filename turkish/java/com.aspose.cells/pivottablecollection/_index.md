---
title: "PivotTableCollection"
second_title: "Aspose.Cells for Java API Referansı"
description: "Belirtilen çalışma sayfasındaki tüm PivotTable nesnelerinin koleksiyonunu temsil eder."
type: docs
url: /tr/java/com.aspose.cells/pivottablecollection/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.CollectionBase](../../com.aspose.cells/collectionbase)
```
public class PivotTableCollection extends CollectionBase
```

Belirtilen çalışma sayfasındaki tüm PivotTable nesnelerinin koleksiyonunu temsil eder.

**Example**

```
         Workbook book = new Workbook();
         Worksheet sheet = book.getWorksheets().get(0);
         Cells cells = sheet.getCells();
         cells.get(0, 0).setValue("fruit");
         cells.get(1, 0).setValue("grape");
         cells.get(2, 0).setValue("blueberry");
         cells.get(3, 0).setValue("kiwi");
         cells.get(4, 0).setValue("cherry");
         cells.get(5, 0).setValue("grape");
         cells.get(6, 0).setValue("blueberry");
         cells.get(7, 0).setValue("kiwi");
         cells.get(8, 0).setValue("cherry");
 
         cells.get(0, 1).setValue("year");
         cells.get(1, 1).setValue(2020);
         cells.get(2, 1).setValue(2020);
         cells.get(3, 1).setValue(2020);
         cells.get(4, 1).setValue(2020);
         cells.get(5, 1).setValue(2021);
         cells.get(6, 1).setValue(2021);
         cells.get(7, 1).setValue(2021);
         cells.get(8, 1).setValue(2021);
 
         cells.get(0, 2).setValue("amount");
         cells.get(1, 2).setValue(50);
         cells.get(2, 2).setValue(60);
         cells.get(3, 2).setValue(70);
         cells.get(4, 2).setValue(80);
         cells.get(5, 2).setValue(90);
         cells.get(6, 2).setValue(100);
         cells.get(7, 2).setValue(110);
         cells.get(8, 2).setValue(120);
 
         PivotTableCollection pivots = sheet.getPivotTables();
 
         PivotTable pivot = pivots.add("=Sheet1!A1:C9", "A12");
 
         pivot.addFieldToArea(PivotFieldType.ROW, "fruit");
         pivot.addFieldToArea(PivotFieldType.COLUMN, "year");
         pivot.addFieldToArea(PivotFieldType.DATA, "amount");
 
         pivot.setPivotTableStyleType(PivotTableStyleType.PIVOT_TABLE_STYLE_MEDIUM_10);
 
         //Change PivotField's attributes
         PivotField rowField = pivot.getRowFields().get(0);
         rowField.setDisplayName("custom display name");
 
         //Add PivotFilter
         PivotFilter filter = pivot.getRowFields().get(0).filterTop10(0, PivotFilterType.PERCENT, false, 2);
 
 
         //Add PivotFormatCondition
         int formatIndex = pivot.getConditionalFormats().add();
         PivotConditionalFormat pfc = pivot.getConditionalFormats().get(formatIndex);
         pfc.addCellArea(pivot.getDataBodyRange());
         FormatConditionCollection fcc = pfc.getFormatConditions();
         int ii = fcc.addCondition(FormatConditionType.CELL_VALUE, OperatorType.GREATER_OR_EQUAL, "100", null);
 
         FormatCondition fc = fcc.get(ii);
 
         fc.getStyle().setBackgroundColor(Color.getRed());
 
         pivot.calculateData();
 
         //do your business
 
         book.save("out.xlsx");
```
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [add(PivotTable pivotTable, int row, int column, String tableName)](#add-com.aspose.cells.PivotTable-int-int-java.lang.String-) | Başka bir PivotTable'a dayanarak yeni bir PivotTable ekler. |
| [add(PivotTable pivotTable, String destCellName, String tableName)](#add-com.aspose.cells.PivotTable-java.lang.String-java.lang.String-) | Başka bir PivotTable'a dayanarak yeni bir PivotTable ekler. |
| [add(Object o)](#add-java.lang.Object-) | CollectionBase örneğine bir öğe ekler. |
| [add(String sourceData, int row, int column)](#add-java.lang.String-int-int-) | Belirtilen çalışma sayfası satır ve sütun konumunda, varsayılan seçeneklerle yeni bir modern PivotTable (Excel 2007'den beri) ekler. |
| [add(String sourceData, int row, int column, PivotTableCreateOptions options)](#add-java.lang.String-int-int-com.aspose.cells.PivotTableCreateOptions-) | Belirtilen çalışma sayfası satır ve sütun konumunda yeni bir PivotTable ekler. |
| [add(String sourceData, int row, int column, String tableName)](#add-java.lang.String-int-int-java.lang.String-) | Eski Excel 97-2003 düzeni ve stiliyle yeni bir PivotTable ekler. |
| [add(String sourceData, int row, int column, String tableName, boolean useSameSource)](#add-java.lang.String-int-int-java.lang.String-boolean-) | Eski Excel 97-2003 düzeni ve stiliyle yeni bir PivotTable ekler. |
| [add(String sourceData, int row, int column, String tableName, boolean useSameSource, boolean isXlsClassic)](#add-java.lang.String-int-int-java.lang.String-boolean-boolean-) | Eski Excel 97-2003 düzeni ve stiliyle yeni bir PivotTable ekler. |
| [add(String sourceData, String cellName)](#add-java.lang.String-java.lang.String-) | Belirtilen çalışma sayfası satır ve sütun konumunda, varsayılan seçeneklerle yeni bir modern PivotTable (Excel 2007'den beri) ekler. |
| [add(String sourceData, String cellName, PivotTableCreateOptions options)](#add-java.lang.String-java.lang.String-com.aspose.cells.PivotTableCreateOptions-) | Belirtilen çalışma sayfası satır ve sütun konumunda, varsayılan seçeneklerle yeni bir modern PivotTable (Excel 2007'den beri) ekler. |
| [add(String sourceData, String destCellName, String tableName)](#add-java.lang.String-java.lang.String-java.lang.String-) | Eski Excel 97-2003 düzeni ve stiliyle yeni bir PivotTable ekler. |
| [add(String sourceData, String destCellName, String tableName, boolean useSameSource)](#add-java.lang.String-java.lang.String-java.lang.String-boolean-) | Eski Excel 97-2003 düzeni ve stiliyle yeni bir PivotTable ekler. |
| [add(String sourceData, String cell, String tableName, boolean useSameSource, boolean isXlsClassic)](#add-java.lang.String-java.lang.String-java.lang.String-boolean-boolean-) | Yeni bir PivotTable ekler. |
| [add(String[] sourceData, boolean isAutoPage, PivotPageFields pageFields, int row, int column, String tableName)](#add-java.lang.String---boolean-com.aspose.cells.PivotPageFields-int-int-java.lang.String-) | Veri kaynağı olarak birden çok konsolidasyon aralığıyla koleksiyona yeni bir PivotTable Nesnesi ekler. |
| [add(String[] sourceData, boolean isAutoPage, PivotPageFields pageFields, String destCellName, String tableName)](#add-java.lang.String---boolean-com.aspose.cells.PivotPageFields-java.lang.String-java.lang.String-) | Veri kaynağı olarak birden çok konsolidasyon aralığıyla koleksiyona yeni bir PivotTable Nesnesi ekler. |
| [clear()](#clear--) | Tüm pivot tablolarını temizler. |
| [contains(Object o)](#contains-java.lang.Object-) | Örneğin bu nesneyi içerip içermediğini döndürür |
| [dispose()](#dispose--) | Yönetilmeyen kaynakların serbest bırakılması, salınması veya sıfırlanmasıyla ilgili uygulama tanımlı görevleri yürütür. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | PivotTable raporunu indeksine göre alır. |
| [get(int row, int column)](#get-int-int-) | Hücrede bulunan [PivotTable](../../com.aspose.cells/pivottable) öğesini alır. |
| [get(String name)](#get-java.lang.String-) | PivotTable raporunu pivot tablonun adıyla alır. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | CollectionBase örneğinde bulunan eleman sayısını alır. |
| [hashCode()](#hashCode--) |  |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | CollectionBase örneğindeki belirli bir öğenin dizinini belirler. |
| [iterator()](#iterator--) | CollectionBase örneği üzerinde yineleme yapan bir enumerator döndürür. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [remove(PivotTable pivotTable)](#remove-com.aspose.cells.PivotTable-) | Belirtilen PivotTable'ı ve PivotTable verilerini siler. |
| [remove(PivotTable pivotTable, boolean keepData)](#remove-com.aspose.cells.PivotTable-boolean-) | Belirtilen PivotTable'ı siler. |
| [removeAt(int index)](#removeAt-int-) | Belirtilen indeksteki PivotTable'ı ve PivotTable verilerini siler. |
| [removeAt(int index, boolean keepData)](#removeAt-int-boolean-) | Belirtilen indeksteki PivotTable'ı siler. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### add(PivotTable pivotTable, int row, int column, String tableName) {#add-com.aspose.cells.PivotTable-int-int-java.lang.String-}
```
public int add(PivotTable pivotTable, int row, int column, String tableName)
```


Başka bir PivotTable'a dayanarak yeni bir PivotTable ekler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| pivotTable | [PivotTable](../../com.aspose.cells/pivottable) | Kaynak pivotTable. |
| satır | int | PivotTable raporunun hedef aralığının sol üst köşesindeki hücrenin satır indeksi. |
| sütun | int | PivotTable raporunun hedef aralığının sol üst köşesindeki hücrenin sütun indeksi. |
| tableName | java.lang.String | Yeni PivotTable raporunun adı. |

**Returns:**
int - Yeni eklenen PivotTable indeksi.
### add(PivotTable pivotTable, String destCellName, String tableName) {#add-com.aspose.cells.PivotTable-java.lang.String-java.lang.String-}
```
public int add(PivotTable pivotTable, String destCellName, String tableName)
```


Başka bir PivotTable'a dayanarak yeni bir PivotTable ekler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| pivotTable | [PivotTable](../../com.aspose.cells/pivottable) | Kaynak pivotTable. |
| destCellName | java.lang.String | PivotTable raporunun hedef aralığının sol üst köşesindeki hücre. |
| tableName | java.lang.String | Yeni PivotTable raporunun adı. |

**Returns:**
int - Yeni eklenen PivotTable indeksi.
### add(Object o) {#add-java.lang.Object-}
```
public int add(Object o)
```


CollectionBase örneğine bir öğe ekler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| o | java.lang.Object | CollectionBase örneğine eklenecek Nesne. |

**Returns:**
int - Yeni elemanın eklendiği konum.
### add(String sourceData, int row, int column) {#add-java.lang.String-int-int-}
```
public PivotTable add(String sourceData, int row, int column)
```


Belirtilen çalışma sayfası satır ve sütun konumunda, varsayılan seçeneklerle yeni bir modern PivotTable (Excel 2007'den beri) ekler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| sourceData | java.lang.String | Yeni PivotTable için veri hücre aralığı. Örnek: Sheet1!A1:C8 |
| satır | int | PivotTable hedefi için sol üst köşenin sıfır tabanlı satır indeksi. |
| sütun | int | PivotTable hedefi için sol üst köşenin sıfır tabanlı sütun indeksi. |

**Returns:**
[PivotTable](../../com.aspose.cells/pivottable) - The newly created PivotTable instance.
### add(String sourceData, int row, int column, PivotTableCreateOptions options) {#add-java.lang.String-int-int-com.aspose.cells.PivotTableCreateOptions-}
```
public PivotTable add(String sourceData, int row, int column, PivotTableCreateOptions options)
```


Belirtilen çalışma sayfası satır ve sütun konumunda yeni bir PivotTable ekler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| sourceData | java.lang.String | Yeni PivotTable için veri hücre aralığı. Örnek: Sheet1!A1:C8 |
| satır | int | PivotTable hedefi için sol üst köşenin sıfır tabanlı satır indeksi. |
| sütun | int | PivotTable hedefi için sol üst köşenin sıfır tabanlı sütun indeksi. |
| options | [PivotTableCreateOptions](../../com.aspose.cells/pivottablecreateoptions) | PivotTable oluşturma seçenekleri. |

**Returns:**
[PivotTable](../../com.aspose.cells/pivottable) - The newly created PivotTable instance.
### add(String sourceData, int row, int column, String tableName) {#add-java.lang.String-int-int-java.lang.String-}
```
public int add(String sourceData, int row, int column, String tableName)
```


Eski Excel 97-2003 düzeni ve stiliyle yeni bir PivotTable ekler.

**Remarks**

NOT: Bu yöntem artık kullanılmamaktadır. `NewPivotTableOptions.IsXlsClassic = true` ile PivotTableCollection.Add(string, int, int, PivotTableCreateOptions) çağrısına eşdeğerdir. Lütfen bunun yerine PivotTableCollection.Add(string, int, int, PivotTableCreateOptions) aşırı yüklemesini kullanın. Bu yöntem, Eylül 2026'dan 12 ay sonra kaldırılacaktır. Verdiği rahatsızlık için özür dileriz.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| sourceData | java.lang.String | Yeni PivotTable için veri hücre aralığı. Örnek: Sheet1!A1:C8 |
| satır | int | PivotTable raporunun hedef aralığının sol üst köşesindeki hücrenin satır indeksi. |
| sütun | int | PivotTable raporunun hedef aralığının sol üst köşesindeki hücrenin sütun indeksi. |
| tableName | java.lang.String | Yeni PivotTable raporunun adı. |

**Returns:**
int - Bu pivot table listesindeki indeks.
### add(String sourceData, int row, int column, String tableName, boolean useSameSource) {#add-java.lang.String-int-int-java.lang.String-boolean-}
```
public int add(String sourceData, int row, int column, String tableName, boolean useSameSource)
```


Eski Excel 97-2003 düzeni ve stiliyle yeni bir PivotTable ekler.

**Remarks**

NOT: Bu yöntem artık kullanılmamaktadır. `NewPivotTableOptions.IsXlsClassic = true` ile PivotTableCollection.Add(string, int, int, PivotTableCreateOptions) çağrısına eşdeğerdir. Lütfen bunun yerine PivotTableCollection.Add(string, int, int, PivotTableCreateOptions) aşırı yüklemesini kullanın. Bu yöntem, Eylül 2026'dan 12 ay sonra kaldırılacaktır. Verdiği rahatsızlık için özür dileriz.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| sourceData | java.lang.String | Yeni PivotTable için veri hücre aralığı. Örnek: Sheet1!A1:C8 |
| satır | int | PivotTable raporunun hedef aralığının sol üst köşesindeki hücrenin satır indeksi. |
| sütun | int | PivotTable raporunun hedef aralığının sol üst köşesindeki hücrenin sütun indeksi. |
| tableName | java.lang.String | Yeni PivotTable raporunun adı. |
| useSameSource | boolean | Başka bir mevcut pivot table bu veri kaynağını kullandığında aynı veri kaynağının kullanılıp kullanılmayacağını gösterir. Özellik true ise bellek tasarrufu sağlar. |

**Returns:**
int - Yeni eklenen önbellek indeksi.
### add(String sourceData, int row, int column, String tableName, boolean useSameSource, boolean isXlsClassic) {#add-java.lang.String-int-int-java.lang.String-boolean-boolean-}
```
public int add(String sourceData, int row, int column, String tableName, boolean useSameSource, boolean isXlsClassic)
```


Eski Excel 97-2003 düzeni ve stiliyle yeni bir PivotTable ekler.

**Remarks**

NOT: Bu yöntem artık kullanılmıyor. PivotTableCollection.Add(string, int, int, PivotTableCreateOptions) çağrısına `NewPivotTableOptions.IsXlsClassic = true` ile eşdeğerdir. Lütfen PivotTableCollection.Add(string, int, int, PivotTableCreateOptions) aşırı yüklemesini kullanın. Bu yöntem Ekim 2026'dan 12 ay sonra kaldırılacaktır. Oluşabilecek herhangi bir rahatsızlık için özür dileriz.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| sourceData | java.lang.String | Yeni PivotTable için veri hücre aralığı. Örnek: Sheet1!A1:C8 |
| satır | int | PivotTable raporunun hedef aralığının sol üst köşesindeki hücrenin satır indeksi. |
| sütun | int | PivotTable raporunun hedef aralığının sol üst köşesindeki hücrenin sütun indeksi. |
| tableName | java.lang.String | Yeni PivotTable raporunun adı. |
| useSameSource | boolean | Başka bir mevcut pivot table bu veri kaynağını kullandığında aynı veri kaynağının kullanılıp kullanılmayacağını gösterir. Özellik true ise bellek tasarrufu sağlar. |
| isXlsClassic | boolean | Excel 97-2003'ün klasik pivot tablosunun eklenip eklenmeyeceğini gösterir. |

**Returns:**
int - Yeni eklenen önbellek indeksi.
### add(String sourceData, String cellName) {#add-java.lang.String-java.lang.String-}
```
public PivotTable add(String sourceData, String cellName)
```


Belirtilen çalışma sayfası satır ve sütun konumunda, varsayılan seçeneklerle yeni bir modern PivotTable (Excel 2007'den beri) ekler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| sourceData | java.lang.String | Yeni PivotTable için veri hücre aralığı. Örnek: Sheet1!A1:C8 |
| cellName | java.lang.String | PivotTable hedefi için sol üst köşe hücresinin adı. |

**Returns:**
[PivotTable](../../com.aspose.cells/pivottable) - The newly created PivotTable instance.
### add(String sourceData, String cellName, PivotTableCreateOptions options) {#add-java.lang.String-java.lang.String-com.aspose.cells.PivotTableCreateOptions-}
```
public PivotTable add(String sourceData, String cellName, PivotTableCreateOptions options)
```


Belirtilen çalışma sayfası satır ve sütun konumunda, varsayılan seçeneklerle yeni bir modern PivotTable (Excel 2007'den beri) ekler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| sourceData | java.lang.String | Yeni PivotTable için veri hücre aralığı. Örnek: Sheet1!A1:C8 |
| cellName | java.lang.String | PivotTable hedefi için sol üst köşe hücresinin adı. |
| options | [PivotTableCreateOptions](../../com.aspose.cells/pivottablecreateoptions) | Pivot tablo oluşturma seçenekleri. |

**Returns:**
[PivotTable](../../com.aspose.cells/pivottable) - The newly created PivotTable instance.
### add(String sourceData, String destCellName, String tableName) {#add-java.lang.String-java.lang.String-java.lang.String-}
```
public int add(String sourceData, String destCellName, String tableName)
```


Eski Excel 97-2003 düzeni ve stiliyle yeni bir PivotTable ekler.

**Remarks**

NOT: Bu yöntem artık kullanılmamaktadır. `NewPivotTableOptions.IsXlsClassic = true` ile PivotTableCollection.Add(string, int, int, PivotTableCreateOptions) çağrısına eşdeğerdir. Lütfen bunun yerine PivotTableCollection.Add(string, int, int, PivotTableCreateOptions) aşırı yüklemesini kullanın. Bu yöntem, Eylül 2026'dan 12 ay sonra kaldırılacaktır. Verdiği rahatsızlık için özür dileriz.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| sourceData | java.lang.String | Yeni PivotTable önbelleği için veri. |
| destCellName | java.lang.String | PivotTable raporunun hedef aralığının sol üst köşesindeki hücre. |
| tableName | java.lang.String | Yeni PivotTable raporunun adı. |

**Returns:**
int - Bu pivot table listesindeki indeks.
### add(String sourceData, String destCellName, String tableName, boolean useSameSource) {#add-java.lang.String-java.lang.String-java.lang.String-boolean-}
```
public int add(String sourceData, String destCellName, String tableName, boolean useSameSource)
```


Eski Excel 97-2003 düzeni ve stiliyle yeni bir PivotTable ekler.

**Remarks**

NOT: Bu yöntem artık kullanılmamaktadır. `NewPivotTableOptions.IsXlsClassic = true` ile PivotTableCollection.Add(string, int, int, PivotTableCreateOptions) çağrısına eşdeğerdir. Lütfen bunun yerine PivotTableCollection.Add(string, int, int, PivotTableCreateOptions) aşırı yüklemesini kullanın. Bu yöntem, Eylül 2026'dan 12 ay sonra kaldırılacaktır. Verdiği rahatsızlık için özür dileriz.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| sourceData | java.lang.String | Yeni PivotTable önbelleği için veri. |
| destCellName | java.lang.String | PivotTable raporunun hedef aralığının sol üst köşesindeki hücre. |
| tableName | java.lang.String | Yeni PivotTable raporunun adı. |
| useSameSource | boolean | Başka bir mevcut pivot table bu veri kaynağını kullandığında aynı veri kaynağının kullanılıp kullanılmayacağını gösterir. Özellik true ise bellek tasarrufu sağlar. |

**Returns:**
int - Yeni eklenen önbellek indeksi.
### add(String sourceData, String cell, String tableName, boolean useSameSource, boolean isXlsClassic) {#add-java.lang.String-java.lang.String-java.lang.String-boolean-boolean-}
```
public int add(String sourceData, String cell, String tableName, boolean useSameSource, boolean isXlsClassic)
```


Yeni bir PivotTable ekler.

**Remarks**

NOT: Bu yöntem artık kullanılmıyor. PivotTableCollection.Add(string, int, int, PivotTableCreateOptions) çağrısına `NewPivotTableOptions.IsXlsClassic = true` ile eşdeğerdir. Lütfen PivotTableCollection.Add(string, int, int, PivotTableCreateOptions) aşırı yüklemesini kullanın. Bu yöntem Ekim 2026'dan 12 ay sonra kaldırılacaktır. Oluşabilecek herhangi bir rahatsızlık için özür dileriz.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| sourceData | java.lang.String | Yeni PivotTable için veri hücre aralığı. Örnek: Sheet1!A1:C8 |
| hücre | java.lang.String | PivotTable raporunun hedef aralığının sol üst köşesindeki hücre. |
| tableName | java.lang.String | Yeni PivotTable raporunun adı. |
| useSameSource | boolean | Başka bir mevcut pivot tablo bu veri kaynağını kullandığında aynı veri kaynağının kullanılıp kullanılmayacağını gösterir. Özellik true ise, aynı veri kaynağı bir pivot önbelleğinde toplandığında bellek tasarrufu sağlar. |
| isXlsClassic | boolean | Excel 97-2003'ün klasik pivot tablosunun eklenip eklenmeyeceğini gösterir. |

**Returns:**
int - Yeni eklenen önbellek indeksi.
### add(String[] sourceData, boolean isAutoPage, PivotPageFields pageFields, int row, int column, String tableName) {#add-java.lang.String---boolean-com.aspose.cells.PivotPageFields-int-int-java.lang.String-}
```
public int add(String[] sourceData, boolean isAutoPage, PivotPageFields pageFields, int row, int column, String tableName)
```


Veri kaynağı olarak birden çok konsolidasyon aralığıyla koleksiyona yeni bir PivotTable Nesnesi ekler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| sourceData | java.lang.String[] | Birden fazla konsolidasyon aralığı, örneğin \{"Sheet1!A1:C8","Sheet2!A1:B8"\} |
| isAutoPage | boolean | Tek bir sayfa alanının otomatik oluşturulup oluşturulmayacağını belirler. True ise, aşağıdaki pageFields parametresi yok sayılacaktır |
| pageFields | [PivotPageFields](../../com.aspose.cells/pivotpagefields) | Pivot sayfa alanı öğeleri. |
| satır | int | PivotTable raporunun hedef aralığının sol üst köşesindeki hücrenin satır indeksi. |
| sütun | int | PivotTable raporunun hedef aralığının sol üst köşesindeki hücrenin sütun indeksi. |
| tableName | java.lang.String | Yeni PivotTable raporunun adı. |

**Returns:**
int - Yeni eklenen PivotTable indeksi.
### add(String[] sourceData, boolean isAutoPage, PivotPageFields pageFields, String destCellName, String tableName) {#add-java.lang.String---boolean-com.aspose.cells.PivotPageFields-java.lang.String-java.lang.String-}
```
public int add(String[] sourceData, boolean isAutoPage, PivotPageFields pageFields, String destCellName, String tableName)
```


Veri kaynağı olarak birden çok konsolidasyon aralığıyla koleksiyona yeni bir PivotTable Nesnesi ekler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| sourceData | java.lang.String[] | Birden fazla konsolidasyon aralığı, örneğin \{"Sheet1!A1:C8","Sheet2!A1:B8"\} |
| isAutoPage | boolean | Tek bir sayfa alanının otomatik oluşturulup oluşturulmayacağını belirler. True ise, aşağıdaki pageFields parametresi yok sayılacaktır. |
| pageFields | [PivotPageFields](../../com.aspose.cells/pivotpagefields) | Pivot sayfa alanı öğeleri. |
| destCellName | java.lang.String | destCellName Yeni PivotTable raporunun adı. |
| tableName | java.lang.String | yeni PivotTable raporunun adı. |

**Returns:**
int - Yeni eklenen PivotTable indeksi.
### clear() {#clear--}
```
public void clear()
```


Tüm pivot tablolarını temizler.

### contains(Object o) {#contains-java.lang.Object-}
```
public boolean contains(Object o)
```


Örneğin bu nesneyi içerip içermediğini döndürür

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| o | java.lang.Object | test nesnesi |

**Returns:**
boolean - Örneğin bu nesneyi içerip içermediği
### dispose() {#dispose--}
```
public void dispose()
```


Yönetilmeyen kaynakların serbest bırakılması, salınması veya sıfırlanmasıyla ilgili uygulama tanımlı görevleri yürütür.

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
### get(int index) {#get-int-}
```
public PivotTable get(int index)
```


PivotTable raporunu indeksine göre alır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| dizin | int |  |

**Returns:**
[PivotTable](../../com.aspose.cells/pivottable)
### get(int row, int column) {#get-int-int-}
```
public PivotTable get(int row, int column)
```


Hücrede bulunan [PivotTable](../../com.aspose.cells/pivottable) öğesini alır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| satır | int |  |
| sütun | int |  |

**Returns:**
[PivotTable](../../com.aspose.cells/pivottable)
### get(String name) {#get-java.lang.String-}
```
public PivotTable get(String name)
```


PivotTable raporunu pivot tablonun adıyla alır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| ad | java.lang.String |  |

**Returns:**
[PivotTable](../../com.aspose.cells/pivottable)
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getCount() {#getCount--}
```
public int getCount()
```


CollectionBase örneğinde bulunan eleman sayısını alır.

**Returns:**
int - CollectionBase örneğinde bulunan eleman sayısı.
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### indexOf(Object o) {#indexOf-java.lang.Object-}
```
public int indexOf(Object o)
```


CollectionBase örneğindeki belirli bir öğenin dizinini belirler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| o | java.lang.Object | CollectionBase örneğindeki belirli bir öğenin dizinini belirler. |

**Returns:**
int - Değer listede bulunursa dizini; aksi takdirde -1.
### iterator() {#iterator--}
```
public Iterator iterator()
```


CollectionBase örneği üzerinde yineleme yapan bir enumerator döndürür.

**Returns:**
java.util.Iterator - CollectionBase örneği için bir iterator.
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### remove(PivotTable pivotTable) {#remove-com.aspose.cells.PivotTable-}
```
public void remove(PivotTable pivotTable)
```


Belirtilen PivotTable'ı ve PivotTable verilerini siler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| pivotTable | [PivotTable](../../com.aspose.cells/pivottable) | PivotTable nesnesi |

### remove(PivotTable pivotTable, boolean keepData) {#remove-com.aspose.cells.PivotTable-boolean-}
```
public void remove(PivotTable pivotTable, boolean keepData)
```


Belirtilen PivotTable'ı siler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| pivotTable | [PivotTable](../../com.aspose.cells/pivottable) | PivotTable nesnesi |
| keepData | boolean | PivotTable verisinin tutulup tutulmayacağını belirler |

### removeAt(int index) {#removeAt-int-}
```
public void removeAt(int index)
```


Belirtilen indeksteki PivotTable'ı ve PivotTable verilerini siler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| dizin | int | PivotTable koleksiyonundaki konum indeksi |

### removeAt(int index, boolean keepData) {#removeAt-int-boolean-}
```
public void removeAt(int index, boolean keepData)
```


Belirtilen indeksteki PivotTable'ı siler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| dizin | int | PivotTable koleksiyonundaki konum indeksi |
| keepData | boolean | PivotTable verisinin tutulup tutulmayacağını belirler |

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

