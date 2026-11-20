---
title: "GridLoadOptions"
second_title: "Справочник API Aspose.Cells for Java"
description: "Представляет параметры загрузки файла."
type: docs
url: /ru/java/com.aspose.gridweb/gridloadoptions/
---

**Inheritance:**
java.lang.Object
```
public class GridLoadOptions
```

Представляет параметры загрузки файла. [Obsolete("This class will be obsoleted after stand alone dll usage of cells public api,instead you can use Aspose.Cells.LodOptions ")]
## Конструкторы

| Конструктор | Описание |
| --- | --- |
| [GridLoadOptions()](#GridLoadOptions--) | Создает параметры загрузки файла. |
## Методы

| Метод | Описание |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAutoFilter()](#getAutoFilter--) | Указывает, следует ли автоматически фильтровать данные при загрузке файлов. |
| [getCheckDataValid()](#getCheckDataValid--) | Проверьте, действительны ли данные в шаблонном файле. |
| [getCheckExcelRestriction()](#getCheckExcelRestriction--) | Проверять ли ограничения Excel‑файла, когда пользователь изменяет связанные с ячейками объекты. |
| [getClass()](#getClass--) |  |
| [getIgnoreNotPrinted()](#getIgnoreNotPrinted--) | Игнорировать данные, которые не печатаются при прямой печати файла |
| [getKeepUnparsedData()](#getKeepUnparsedData--) | Сохранять ли неразобранные данные в памяти для рабочей книги при загрузке из шаблонного файла. |
| [getOnlyAuto()](#getOnlyAuto--) | Указывает, следует ли подгонять только те строки, высота которых не настроена вручную. |
| [getParsingFormulaOnOpen()](#getParsingFormulaOnOpen--) | Указывает, следует ли разбирать формулу при чтении файла. |
| [getParsingPivotCachedRecords()](#getParsingPivotCachedRecords--) | Указывает, следует ли разбирать кэшированные записи сводных таблиц при загрузке файла. |
| [getPassword()](#getPassword--) | Получает пароль рабочей книги. |
| [getPreservePaddingSpacesInFormula()](#getPreservePaddingSpacesInFormula--) | Указывает, следует ли сохранять пробелы и переводы строк, вставленные между токенами формулы при получении и установке формул. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAutoFilter(boolean value)](#setAutoFilter-boolean-) | Указывает, следует ли автоматически фильтровать данные при загрузке файлов. |
| [setCheckDataValid(boolean value)](#setCheckDataValid-boolean-) | Проверьте, действительны ли данные в шаблонном файле. |
| [setCheckExcelRestriction(boolean value)](#setCheckExcelRestriction-boolean-) | Проверять ли ограничения Excel‑файла, когда пользователь изменяет связанные с ячейками объекты. |
| [setIgnoreNotPrinted(boolean value)](#setIgnoreNotPrinted-boolean-) | Игнорировать данные, которые не печатаются при прямой печати файла |
| [setKeepUnparsedData(boolean value)](#setKeepUnparsedData-boolean-) | Сохранять ли неразобранные данные в памяти для рабочей книги при загрузке из шаблонного файла. |
| [setOnlyAuto(boolean value)](#setOnlyAuto-boolean-) | Указывает, следует ли подгонять только те строки, высота которых не настроена вручную. |
| [setParsingFormulaOnOpen(boolean value)](#setParsingFormulaOnOpen-boolean-) | Указывает, следует ли разбирать формулу при чтении файла. |
| [setParsingPivotCachedRecords(boolean value)](#setParsingPivotCachedRecords-boolean-) | Указывает, следует ли разбирать кэшированные записи сводных таблиц при загрузке файла. |
| [setPassword(String value)](#setPassword-java.lang.String-) | Устанавливает пароль для workbook. |
| [setPreservePaddingSpacesInFormula(boolean value)](#setPreservePaddingSpacesInFormula-boolean-) | Указывает, следует ли сохранять пробелы и переводы строк, вставленные между токенами формулы при получении и установке формул. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### GridLoadOptions() {#GridLoadOptions--}
```
public GridLoadOptions()
```


Создает параметры загрузки файла.

### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| arg0 | java.lang.Object |  |

**Returns:**
boolean
### getAutoFilter() {#getAutoFilter--}
```
public boolean getAutoFilter()
```


Указывает, следует ли автоматически фильтровать данные при загрузке файлов.

**Remarks**

Иногда, хотя автотест (autofilter) установлен, соответствующие строки не скрываются в файле. Сейчас работает только для файлов SpreadSheetML.

**Returns:**
boolean
### getCheckDataValid() {#getCheckDataValid--}
```
public boolean getCheckDataValid()
```


Проверьте, действительны ли данные в шаблонном файле.

**Returns:**
boolean
### getCheckExcelRestriction() {#getCheckExcelRestriction--}
```
public boolean getCheckExcelRestriction()
```


Определяет, проверять ли ограничения файла Excel при изменении пользователем объектов, связанных с ячейками. Например, Excel не позволяет вводить строковое значение длиной более 32 КБ. Когда вы вводите значение длиной более 32 КБ, например с помощью Cell.PutValue(string), если это свойство установлено в true, будет выброшено исключение. Если свойство установлено в false, мы примем введённую строку как значение ячейки, чтобы позже вы могли вывести полное строковое значение в другие форматы файлов, такие как CSV. Однако, если вы задали значение, которое недопустимо для формата файла Excel, позже не следует сохранять workbook в формате Excel. В противном случае может возникнуть непредвиденная ошибка в сгенерированном файле Excel.

**Returns:**
boolean
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getIgnoreNotPrinted() {#getIgnoreNotPrinted--}
```
public boolean getIgnoreNotPrinted()
```


Игнорировать данные, которые не печатаются при прямой печати файла

**Remarks**

Только для файлов xlsx.

**Returns:**
boolean
### getKeepUnparsedData() {#getKeepUnparsedData--}
```
public boolean getKeepUnparsedData()
```


Определяет, сохранять ли неразобранные данные в памяти для Workbook при загрузке из шаблонного файла. По умолчанию true.

**Remarks**

В сценариях, когда пользователю необходимо только прочитать часть содержимого шаблонного файла и не требуется сохранять workbook обратно, установка этого свойства в false может повысить производительность, особенно при совместном использовании с некоторыми типами LoadFilter,

**Returns:**
boolean
### getOnlyAuto() {#getOnlyAuto--}
```
public boolean getOnlyAuto()
```


Указывает, следует ли подгонять только те строки, высота которых не настроена вручную.

**Returns:**
boolean
### getParsingFormulaOnOpen() {#getParsingFormulaOnOpen--}
```
public boolean getParsingFormulaOnOpen()
```


Указывает, следует ли разбирать формулу при чтении файла.

**Remarks**

Применяется только к файлам Excel Xlsx, Xltx, Xltm и Xlsm, поскольку формулы в этих файлах хранятся в виде строковой формулы.

**Returns:**
boolean
### getParsingPivotCachedRecords() {#getParsingPivotCachedRecords--}
```
public boolean getParsingPivotCachedRecords()
```


Указывает, следует ли разбирать кэшированные записи сводных таблиц при загрузке файла. Значение по умолчанию — false.

**Remarks**

Применяется только к файлам Excel Xlsx, Xltx, Xltm, Xlsm и xlsb.

**Returns:**
boolean
### getPassword() {#getPassword--}
```
public String getPassword()
```


Получает пароль рабочей книги.

**Returns:**
java.lang.String
### getPreservePaddingSpacesInFormula() {#getPreservePaddingSpacesInFormula--}
```
public boolean getPreservePaddingSpacesInFormula()
```


Указывает, сохранять ли пробелы и разрывы строк, вставленные между токенами формулы при получении и установке формул. Значение по умолчанию — false.

**Remarks**

После загрузки книги из шаблонного файла с этой опцией, [GridWorkbookSettings.getPreservePaddingSpaces()](../../com.aspose.gridweb/gridworkbooksettings\#getPreservePaddingSpaces--) будет установлено в то же значение, что и это свойство.

**Returns:**
boolean
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




### setAutoFilter(boolean value) {#setAutoFilter-boolean-}
```
public void setAutoFilter(boolean value)
```


Указывает, следует ли автоматически фильтровать данные при загрузке файлов.

**Remarks**

Иногда, хотя автотест (autofilter) установлен, соответствующие строки не скрываются в файле. Сейчас работает только для файлов SpreadSheetML.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setCheckDataValid(boolean value) {#setCheckDataValid-boolean-}
```
public void setCheckDataValid(boolean value)
```


Проверьте, действительны ли данные в шаблонном файле.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setCheckExcelRestriction(boolean value) {#setCheckExcelRestriction-boolean-}
```
public void setCheckExcelRestriction(boolean value)
```


Определяет, проверять ли ограничения файла Excel при изменении пользователем объектов, связанных с ячейками. Например, Excel не позволяет вводить строковое значение длиной более 32 КБ. Когда вы вводите значение длиной более 32 КБ, например с помощью Cell.PutValue(string), если это свойство установлено в true, будет выброшено исключение. Если свойство установлено в false, мы примем введённую строку как значение ячейки, чтобы позже вы могли вывести полное строковое значение в другие форматы файлов, такие как CSV. Однако, если вы задали значение, которое недопустимо для формата файла Excel, позже не следует сохранять workbook в формате Excel. В противном случае может возникнуть непредвиденная ошибка в сгенерированном файле Excel.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setIgnoreNotPrinted(boolean value) {#setIgnoreNotPrinted-boolean-}
```
public void setIgnoreNotPrinted(boolean value)
```


Игнорировать данные, которые не печатаются при прямой печати файла

**Remarks**

Только для файлов xlsx.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setKeepUnparsedData(boolean value) {#setKeepUnparsedData-boolean-}
```
public void setKeepUnparsedData(boolean value)
```


Определяет, сохранять ли неразобранные данные в памяти для Workbook при загрузке из шаблонного файла. По умолчанию true.

**Remarks**

В сценариях, когда пользователю необходимо только прочитать часть содержимого шаблонного файла и не требуется сохранять workbook обратно, установка этого свойства в false может повысить производительность, особенно при совместном использовании с некоторыми типами LoadFilter,

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setOnlyAuto(boolean value) {#setOnlyAuto-boolean-}
```
public void setOnlyAuto(boolean value)
```


Указывает, следует ли подгонять только те строки, высота которых не настроена вручную.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setParsingFormulaOnOpen(boolean value) {#setParsingFormulaOnOpen-boolean-}
```
public void setParsingFormulaOnOpen(boolean value)
```


Указывает, следует ли разбирать формулу при чтении файла.

**Remarks**

Применяется только к файлам Excel Xlsx, Xltx, Xltm и Xlsm, поскольку формулы в этих файлах хранятся в виде строковой формулы.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setParsingPivotCachedRecords(boolean value) {#setParsingPivotCachedRecords-boolean-}
```
public void setParsingPivotCachedRecords(boolean value)
```


Указывает, следует ли разбирать кэшированные записи сводных таблиц при загрузке файла. Значение по умолчанию — false.

**Remarks**

Применяется только к файлам Excel Xlsx, Xltx, Xltm, Xlsm и xlsb.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setPassword(String value) {#setPassword-java.lang.String-}
```
public void setPassword(String value)
```


Устанавливает пароль для workbook.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### setPreservePaddingSpacesInFormula(boolean value) {#setPreservePaddingSpacesInFormula-boolean-}
```
public void setPreservePaddingSpacesInFormula(boolean value)
```


Указывает, сохранять ли пробелы и разрывы строк, вставленные между токенами формулы при получении и установке формул. Значение по умолчанию — false.

**Remarks**

После загрузки книги из шаблонного файла с этой опцией, [GridWorkbookSettings.getPreservePaddingSpaces()](../../com.aspose.gridweb/gridworkbooksettings\#getPreservePaddingSpaces--) будет установлено в то же значение, что и это свойство.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

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
| Параметр | Тип | Описание |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

