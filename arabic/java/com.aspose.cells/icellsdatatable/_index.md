---
title: "ICellsDataTable"
second_title: "Aspose.Cells for Java API Reference"
description: "يمثل جدول البيانات."
type: docs
url: /ar/java/com.aspose.cells/icellsdatatable/
---
```
public interface ICellsDataTable
```

يمثل جدول البيانات.

**Remarks**
## الطرق

| طريقة | الوصف |
| --- | --- |
| [beforeFirst()](#beforeFirst--) | حرك المؤشر إلى مقدمة هذا الكائن، مباشرةً قبل الصف الأول. |
| [get(int columnIndex)](#get-int-) | يحصل على البيانات المخزنة في العمود المحدد بالفهرس. |
| [get(String columnName)](#get-java.lang.String-) | يحصل على البيانات المخزنة في العمود المحدد باسم العمود. |
| [getColumns()](#getColumns--) | يحصل على اسم الأعمدة. |
| [getCount()](#getCount--) | يحصل على عدد السجلات. -1 للعدد غير المعروف للسجلات. |
| [next()](#next--) | يحرك المؤشر لأسفل صف واحد من موقعه الحالي. |
### beforeFirst() {#beforeFirst--}
```
public abstract void beforeFirst()
```


حرك المؤشر إلى مقدمة هذا الكائن، مباشرةً قبل الصف الأول.

### get(int columnIndex) {#get-int-}
```
public abstract Object get(int columnIndex)
```


يحصل على البيانات المخزنة في العمود المحدد بالفهرس.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| columnIndex | int | الفهرس الصفري للعمود. |

**Returns:**
java.lang.Object - 
### get(String columnName) {#get-java.lang.String-}
```
public abstract Object get(String columnName)
```


يحصل على البيانات المخزنة في العمود المحدد باسم العمود.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| columnName | java.lang.String | اسم العمود. |

**Returns:**
java.lang.Object - 
### getColumns() {#getColumns--}
```
public abstract String[] getColumns()
```


يحصل على اسم الأعمدة.

**Returns:**
java.lang.String[]
### getCount() {#getCount--}
```
public abstract int getCount()
```


يحصل على عدد السجلات. -1 للعدد غير المعروف للسجلات.

**Returns:**
int
### next() {#next--}
```
public abstract boolean next()
```


يحرك المؤشر لأسفل صف واحد من موقعه الحالي.

**Returns:**
boolean - إذا كان الصف الحالي الجديد صالحًا؛ false إذا لم تعد هناك صفوف أخرى
