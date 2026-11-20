---
title: "GridTxtLoadOptions"
second_title: "Справочник API Aspose.Cells for Java"
description: "Представляет параметры загрузки текстового файла."
type: docs
url: /ru/java/com.aspose.gridweb/gridtxtloadoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.gridweb.GridLoadOptions](../../com.aspose.gridweb/gridloadoptions)
```
public class GridTxtLoadOptions extends GridLoadOptions
```

Представляет параметры загрузки текстового файла.
## Конструкторы

| Конструктор | Описание |
| --- | --- |
| [GridTxtLoadOptions()](#GridTxtLoadOptions--) | Создаёт параметры для загрузки текстового файла. |
## Методы

| Метод | Описание |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAutoFilter()](#getAutoFilter--) | Указывает, следует ли автоматически фильтровать данные при загрузке файлов. |
| [getCheckDataValid()](#getCheckDataValid--) | Проверьте, действительны ли данные в шаблонном файле. |
| [getCheckExcelRestriction()](#getCheckExcelRestriction--) | Проверять ли ограничения Excel‑файла, когда пользователь изменяет связанные с ячейками объекты. |
| [getClass()](#getClass--) |  |
| [getConvertDateTimeData()](#getConvertDateTimeData--) | Получает значение, указывающее, преобразуется ли строка в текстовом файле в данные типа дата. |
| [getConvertNumericData()](#getConvertNumericData--) | Получает значение, указывающее, преобразуется ли строка в текстовом файле в числовые данные. |
| [getEncoding()](#getEncoding--) | Получает кодировку по умолчанию. |
| [getExtendToNextSheet()](#getExtendToNextSheet--) | Расширяет ли данные на следующий лист, когда количество строк или столбцов данных превышает лимит. |
| [getIgnoreNotPrinted()](#getIgnoreNotPrinted--) | Игнорировать данные, которые не печатаются при прямой печати файла |
| [getKeepPrecision()](#getKeepPrecision--) | Указывает, следует ли не разбирать строковое значение, если его длина составляет 15. |
| [getKeepUnparsedData()](#getKeepUnparsedData--) | Сохранять ли неразобранные данные в памяти для рабочей книги при загрузке из шаблонного файла. |
| [getOnlyAuto()](#getOnlyAuto--) | Указывает, следует ли подгонять только те строки, высота которых не настроена вручную. |
| [getParsingFormulaOnOpen()](#getParsingFormulaOnOpen--) | Указывает, следует ли разбирать формулу при чтении файла. |
| [getParsingPivotCachedRecords()](#getParsingPivotCachedRecords--) | Указывает, следует ли разбирать кэшированные записи сводных таблиц при загрузке файла. |
| [getPassword()](#getPassword--) | Получает пароль рабочей книги. |
| [getPreservePaddingSpacesInFormula()](#getPreservePaddingSpacesInFormula--) | Указывает, следует ли сохранять пробелы и переводы строк, вставленные между токенами формулы при получении и установке формул. |
| [getSeparator()](#getSeparator--) | Получает символьный разделитель текстового файла. |
| [getSeparatorString()](#getSeparatorString--) | Получает строковое значение в качестве разделителя. |
| [getTextQualifier()](#getTextQualifier--) | Указывает текстовый квалификатор для значений ячеек. |
| [getTreatConsecutiveDelimitersAsOne()](#getTreatConsecutiveDelimitersAsOne--) | Определяет, следует ли рассматривать последовательные разделители как один. |
| [getTreatQuotePrefixAsValue()](#getTreatQuotePrefixAsValue--) | Указывает, следует ли учитывать начальный одинарный апостроф как часть значения ячейки. |
| [hasFormula()](#hasFormula--) | Указывает, является ли текст формулой, если он начинается с "=". |
| [hasTextQualifier()](#hasTextQualifier--) | Есть ли текстовый квалификатор для значения ячейки. |
| [hashCode()](#hashCode--) |  |
| [isMultiEncoded()](#isMultiEncoded--) | True означает, что файл содержит несколько кодировок. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAutoFilter(boolean value)](#setAutoFilter-boolean-) | Указывает, следует ли автоматически фильтровать данные при загрузке файлов. |
| [setCheckDataValid(boolean value)](#setCheckDataValid-boolean-) | Проверьте, действительны ли данные в шаблонном файле. |
| [setCheckExcelRestriction(boolean value)](#setCheckExcelRestriction-boolean-) | Проверять ли ограничения Excel‑файла, когда пользователь изменяет связанные с ячейками объекты. |
| [setConvertDateTimeData(boolean value)](#setConvertDateTimeData-boolean-) | Устанавливает значение, указывающее, преобразуется ли строка в текстовом файле в дату. |
| [setConvertNumericData(boolean value)](#setConvertNumericData-boolean-) | Устанавливает значение, указывающее, преобразуется ли строка в текстовом файле в числовые данные. |
| [setEncoding(Encoding value)](#setEncoding-com.aspose.gridweb.Encoding-) | Устанавливает кодировку по умолчанию. |
| [setExtendToNextSheet(boolean value)](#setExtendToNextSheet-boolean-) | Расширяет ли данные на следующий лист, когда количество строк или столбцов данных превышает лимит. |
| [setHasFormula(boolean value)](#setHasFormula-boolean-) | Указывает, является ли текст формулой, если он начинается с "=". |
| [setHasTextQualifier(boolean value)](#setHasTextQualifier-boolean-) | Есть ли текстовый квалификатор для значения ячейки. |
| [setIgnoreNotPrinted(boolean value)](#setIgnoreNotPrinted-boolean-) | Игнорировать данные, которые не печатаются при прямой печати файла |
| [setKeepPrecision(boolean value)](#setKeepPrecision-boolean-) | Указывает, следует ли не разбирать строковое значение, если его длина составляет 15. |
| [setKeepUnparsedData(boolean value)](#setKeepUnparsedData-boolean-) | Сохранять ли неразобранные данные в памяти для рабочей книги при загрузке из шаблонного файла. |
| [setMultiEncoded(boolean value)](#setMultiEncoded-boolean-) | True означает, что файл содержит несколько кодировок. |
| [setOnlyAuto(boolean value)](#setOnlyAuto-boolean-) | Указывает, следует ли подгонять только те строки, высота которых не настроена вручную. |
| [setParsingFormulaOnOpen(boolean value)](#setParsingFormulaOnOpen-boolean-) | Указывает, следует ли разбирать формулу при чтении файла. |
| [setParsingPivotCachedRecords(boolean value)](#setParsingPivotCachedRecords-boolean-) | Указывает, следует ли разбирать кэшированные записи сводных таблиц при загрузке файла. |
| [setPassword(String value)](#setPassword-java.lang.String-) | Устанавливает пароль для workbook. |
| [setPreservePaddingSpacesInFormula(boolean value)](#setPreservePaddingSpacesInFormula-boolean-) | Указывает, следует ли сохранять пробелы и переводы строк, вставленные между токенами формулы при получении и установке формул. |
| [setSeparator(char value)](#setSeparator-char-) | Устанавливает символьный разделитель текстового файла. |
| [setSeparatorString(String value)](#setSeparatorString-java.lang.String-) | Устанавливает строковое значение в качестве разделителя. |
| [setTextQualifier(char value)](#setTextQualifier-char-) | Указывает текстовый квалификатор для значений ячеек. |
| [setTreatConsecutiveDelimitersAsOne(boolean value)](#setTreatConsecutiveDelimitersAsOne-boolean-) | Определяет, следует ли рассматривать последовательные разделители как один. |
| [setTreatQuotePrefixAsValue(boolean value)](#setTreatQuotePrefixAsValue-boolean-) | Указывает, следует ли учитывать начальный одинарный апостроф как часть значения ячейки. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### GridTxtLoadOptions() {#GridTxtLoadOptions--}
```
public GridTxtLoadOptions()
```


Создаёт параметры для загрузки текстового файла.

**Remarks**

Тип файла по умолчанию для загрузки — CSV.

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
### getConvertDateTimeData() {#getConvertDateTimeData--}
```
public boolean getConvertDateTimeData()
```


Получает значение, указывающее, преобразуется ли строка в текстовом файле в данные типа дата.

**Returns:**
boolean
### getConvertNumericData() {#getConvertNumericData--}
```
public boolean getConvertNumericData()
```


Получает значение, указывающее, преобразуется ли строка в текстовом файле в числовые данные.

**Returns:**
boolean
### getEncoding() {#getEncoding--}
```
public Encoding getEncoding()
```


Получает кодировку по умолчанию. Применяется только для CSV‑файлов.

**Returns:**
[Encoding](../../com.aspose.gridweb/encoding)
### getExtendToNextSheet() {#getExtendToNextSheet--}
```
public boolean getExtendToNextSheet()
```


Расширяет ли данные на следующий лист, когда строки или столбцы данных превышают предел. Если это свойство истинно, дополнительные данные будут расширены на следующий лист позади текущего (если текущий лист последний, новый лист будет добавлен к текущей книге). Если это свойство ложно, данные, превышающие предел, будут игнорироваться. По умолчанию ложно;

**Returns:**
boolean
### getIgnoreNotPrinted() {#getIgnoreNotPrinted--}
```
public boolean getIgnoreNotPrinted()
```


Игнорировать данные, которые не печатаются при прямой печати файла

**Remarks**

Только для файлов xlsx.

**Returns:**
boolean
### getKeepPrecision() {#getKeepPrecision--}
```
public boolean getKeepPrecision()
```


Указывает, следует ли не разбирать строковое значение, если его длина составляет 15.

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
### getSeparator() {#getSeparator--}
```
public char getSeparator()
```


Получает символьный разделитель текстового файла.

**Returns:**
char
### getSeparatorString() {#getSeparatorString--}
```
public String getSeparatorString()
```


Получает строковое значение в качестве разделителя.

**Returns:**
java.lang.String
### getTextQualifier() {#getTextQualifier--}
```
public char getTextQualifier()
```


Указывает текстовый квалификатор для значений ячеек. Квалификатор по умолчанию — '\"'.

**Remarks**

При установке этого свойства, [hasTextQualifier()](../../com.aspose.gridweb/gridtxtloadoptions\#hasTextQualifier--) станет истинным автоматически.

**Returns:**
char
### getTreatConsecutiveDelimitersAsOne() {#getTreatConsecutiveDelimitersAsOne--}
```
public boolean getTreatConsecutiveDelimitersAsOne()
```


Определяет, следует ли рассматривать последовательные разделители как один.

**Returns:**
boolean
### getTreatQuotePrefixAsValue() {#getTreatQuotePrefixAsValue--}
```
public boolean getTreatQuotePrefixAsValue()
```


Указывает, следует ли учитывать начальный одинарный кавычка как часть значения ячейки. По умолчанию истинно. Если ложно, начальная одинарная кавычка будет удалена из соответствующего значения ячейки, и [GridTableItemStyle.getQuotePrefix()](../../com.aspose.gridweb/gridtableitemstyle\#getQuotePrefix--) будет установлена в истинно для ячейки.

**Returns:**
boolean
### hasFormula() {#hasFormula--}
```
public boolean hasFormula()
```


Указывает, является ли текст формулой, если он начинается с "=".

**Returns:**
boolean
### hasTextQualifier() {#hasTextQualifier--}
```
public boolean hasTextQualifier()
```


Есть ли текстовый квалификатор для значения ячейки. По умолчанию — true.

**Returns:**
boolean
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isMultiEncoded() {#isMultiEncoded--}
```
public boolean isMultiEncoded()
```


True означает, что файл содержит несколько кодировок.

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

### setConvertDateTimeData(boolean value) {#setConvertDateTimeData-boolean-}
```
public void setConvertDateTimeData(boolean value)
```


Устанавливает значение, указывающее, преобразуется ли строка в текстовом файле в дату.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setConvertNumericData(boolean value) {#setConvertNumericData-boolean-}
```
public void setConvertNumericData(boolean value)
```


Устанавливает значение, указывающее, преобразуется ли строка в текстовом файле в числовые данные.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setEncoding(Encoding value) {#setEncoding-com.aspose.gridweb.Encoding-}
```
public void setEncoding(Encoding value)
```


Устанавливает кодировку по умолчанию. Применяется только для файлов csv.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| value | [Encoding](../../com.aspose.gridweb/encoding) |  |

### setExtendToNextSheet(boolean value) {#setExtendToNextSheet-boolean-}
```
public void setExtendToNextSheet(boolean value)
```


Расширяет ли данные на следующий лист, когда строки или столбцы данных превышают предел. Если это свойство истинно, дополнительные данные будут расширены на следующий лист позади текущего (если текущий лист последний, новый лист будет добавлен к текущей книге). Если это свойство ложно, данные, превышающие предел, будут игнорироваться. По умолчанию ложно;

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setHasFormula(boolean value) {#setHasFormula-boolean-}
```
public void setHasFormula(boolean value)
```


Указывает, является ли текст формулой, если он начинается с "=".

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setHasTextQualifier(boolean value) {#setHasTextQualifier-boolean-}
```
public void setHasTextQualifier(boolean value)
```


Есть ли текстовый квалификатор для значения ячейки. По умолчанию — true.

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

### setKeepPrecision(boolean value) {#setKeepPrecision-boolean-}
```
public void setKeepPrecision(boolean value)
```


Указывает, следует ли не разбирать строковое значение, если его длина составляет 15.

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

### setMultiEncoded(boolean value) {#setMultiEncoded-boolean-}
```
public void setMultiEncoded(boolean value)
```


True означает, что файл содержит несколько кодировок.

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

### setSeparator(char value) {#setSeparator-char-}
```
public void setSeparator(char value)
```


Устанавливает символьный разделитель текстового файла.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | char |  |

### setSeparatorString(String value) {#setSeparatorString-java.lang.String-}
```
public void setSeparatorString(String value)
```


Устанавливает строковое значение в качестве разделителя.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### setTextQualifier(char value) {#setTextQualifier-char-}
```
public void setTextQualifier(char value)
```


Указывает текстовый квалификатор для значений ячеек. Квалификатор по умолчанию — '\"'.

**Remarks**

При установке этого свойства, [hasTextQualifier()](../../com.aspose.gridweb/gridtxtloadoptions\#hasTextQualifier--) станет истинным автоматически.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | char |  |

### setTreatConsecutiveDelimitersAsOne(boolean value) {#setTreatConsecutiveDelimitersAsOne-boolean-}
```
public void setTreatConsecutiveDelimitersAsOne(boolean value)
```


Определяет, следует ли рассматривать последовательные разделители как один.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setTreatQuotePrefixAsValue(boolean value) {#setTreatQuotePrefixAsValue-boolean-}
```
public void setTreatQuotePrefixAsValue(boolean value)
```


Указывает, следует ли учитывать начальный одинарный кавычка как часть значения ячейки. По умолчанию истинно. Если ложно, начальная одинарная кавычка будет удалена из соответствующего значения ячейки, и [GridTableItemStyle.getQuotePrefix()](../../com.aspose.gridweb/gridtableitemstyle\#getQuotePrefix--) будет установлена в истинно для ячейки.

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

