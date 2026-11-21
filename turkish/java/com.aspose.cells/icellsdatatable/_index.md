---
title: "ICellsDataTable"
second_title: "Aspose.Cells for Java API Referansı"
description: "Veri tablosunu temsil eder."
type: docs
url: /tr/java/com.aspose.cells/icellsdatatable/
---
```
public interface ICellsDataTable
```

Veri tablosunu temsil eder.

**Remarks**
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [beforeFirst()](#beforeFirst--) | İmleci bu nesnenin önüne, ilk satırın hemen önüne taşı. |
| [get(int columnIndex)](#get-int-) | İndeks ile belirtilen sütunda depolanan veriyi alır. |
| [get(String columnName)](#get-java.lang.String-) | Sütun adı ile belirtilen sütunda depolanan veriyi alır. |
| [getColumns()](#getColumns--) | Sütunların adını alır. |
| [getCount()](#getCount--) | Kayıtların sayısını alır. Bilinmeyen kayıt sayısı için -1. |
| [next()](#next--) | İmleci mevcut konumundan bir satır aşağı hareket ettirir. |
### beforeFirst() {#beforeFirst--}
```
public abstract void beforeFirst()
```


İmleci bu nesnenin önüne, ilk satırın hemen önüne taşı.

### get(int columnIndex) {#get-int-}
```
public abstract Object get(int columnIndex)
```


İndeks ile belirtilen sütunda depolanan veriyi alır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| columnIndex | int | Sütunun sıfır tabanlı indeksi. |

**Returns:**
java.lang.Object - 
### get(String columnName) {#get-java.lang.String-}
```
public abstract Object get(String columnName)
```


Sütun adı ile belirtilen sütunda depolanan veriyi alır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| columnName | java.lang.String | Sütun adı. |

**Returns:**
java.lang.Object - 
### getColumns() {#getColumns--}
```
public abstract String[] getColumns()
```


Sütunların adını alır.

**Returns:**
java.lang.String[]
### getCount() {#getCount--}
```
public abstract int getCount()
```


Kayıtların sayısını alır. Bilinmeyen kayıt sayısı için -1.

**Returns:**
int
### next() {#next--}
```
public abstract boolean next()
```


İmleci mevcut konumundan bir satır aşağı hareket ettirir.

**Returns:**
boolean - yeni mevcut satır geçerliyse; daha fazla satır yoksa false
