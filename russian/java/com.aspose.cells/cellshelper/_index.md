---
title: "CellsHelper"
second_title: "Справочник API Aspose.Cells for Java"
description: "Предоставляет вспомогательные функции."
type: docs
url: /ru/java/com.aspose.cells/cellshelper/
---

**Inheritance:**
java.lang.Object
```
public class CellsHelper
```

Предоставляет вспомогательные функции.
## Методы

| Метод | Описание |
| --- | --- |
| [addAddInFunction(String function, int minCountOfParameters, int maxCountOfParameters, int[] paramersType, int functionValueType)](#addAddInFunction-java.lang.String-int-int-int---int-) | Добавить функцию надстройки. |
| [cellIndexToName(int row, int column)](#cellIndexToName-int-int-) | Получает имя ячейки по её индексам строки и столбца. |
| [cellNameToIndex(String cellName)](#cellNameToIndex-java.lang.String-) | Получает индексы строки и столбца ячейки по её имени. |
| [columnIndexToName(int column)](#columnIndexToName-int-) | Получает имя столбца по индексу столбца. |
| [columnNameToIndex(String columnName)](#columnNameToIndex-java.lang.String-) | Получает индекс столбца по имени столбца. |
| [convertA1FormulaToR1C1(String formula, int row, int column)](#convertA1FormulaToR1C1-java.lang.String-int-int-) | Преобразует формулу A1 ячейки в формулу r1c1. |
| [convertR1C1FormulaToA1(String r1c1Formula, int row, int column)](#convertR1C1FormulaToA1-java.lang.String-int-int-) | Преобразует формулу r1c1 ячейки в формулу A1. |
| [createSafeSheetName(String nameProposal)](#createSafeSheetName-java.lang.String-) | Проверяет указанное имя листа и при необходимости создает корректное. |
| [createSafeSheetName(String nameProposal, char replaceChar)](#createSafeSheetName-java.lang.String-char-) | Проверяет указанное имя листа и при необходимости создает корректное. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAltStartPath()](#getAltStartPath--) | Получает альтернативный путь запуска, на который ссылаются некоторые внешние формульные ссылки. |
| [getCacheFolder()](#getCacheFolder--) | Получает папку для временных файлов, которые могут использоваться как кэш данных. |
| [getClass()](#getClass--) |  |
| [getCustomImplementationFactory()](#getCustomImplementationFactory--) | Получает фабрику для создания экземпляров со специальной реализацией. |
| [getDPI()](#getDPI--) | Получает DPI машины. |
| [getDateTimeFromDouble(double doubleValue, boolean date1904)](#getDateTimeFromDouble-double-boolean-) | Преобразует значение double в значение даты и времени. |
| [getDoubleFromDateTime(DateTime dateTime, boolean date1904)](#getDoubleFromDateTime-com.aspose.cells.DateTime-boolean-) | Преобразует дату и время в значение double. |
| [getLibraryPath()](#getLibraryPath--) | Получает путь к библиотеке, на который ссылаются некоторые внешние формульные ссылки. |
| [getSignificantDigits()](#getSignificantDigits--) | Получает количество значимых цифр. |
| [getSignificantDigitsType()](#getSignificantDigitsType--) | Получает тип значимых цифр по умолчанию для вывода числовых значений. |
| [getStartupPath()](#getStartupPath--) | Получает путь запуска, на который ссылаются некоторые внешние формульные ссылки. |
| [getTextWidth(String text, Font font, double scaling)](#getTextWidth-java.lang.String-com.aspose.cells.Font-double-) | Получить ширину текста в единицах точек. |
| [getUsedColors(Workbook workbook)](#getUsedColors-com.aspose.cells.Workbook-) | Получает все используемые цвета в рабочей книге. |
| [getVersion()](#getVersion--) | Получить версию релиза. |
| [hashCode()](#hashCode--) |  |
| [isCloudPlatform()](#isCloudPlatform--) | Пожалуйста, установите это свойство в True при работе на облачной платформе, такой как: Azure, AWSLambda и т.д., |
| [mergeFiles(String[] files, String cachedFile, String destFile)](#mergeFiles-java.lang.String---java.lang.String-java.lang.String-) | Объединяет несколько больших файлов xls в один файл xls. |
| [needQuoteInFormula(String sheetName)](#needQuoteInFormula-java.lang.String-) | Указывает, следует ли заключать имя листа в одинарные кавычки |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [rowIndexToName(int row)](#rowIndexToName-int-) | Получает имя строки по индексу строки. |
| [rowNameToIndex(String rowName)](#rowNameToIndex-java.lang.String-) | Получает индекс строки по имени строки. |
| [setAltStartPath(String value)](#setAltStartPath-java.lang.String-) | Устанавливает альтернативный путь запуска, на который ссылаются некоторые внешние формульные ссылки. |
| [setCacheFolder(String cache)](#setCacheFolder-java.lang.String-) | Устанавливает папку для временных файлов, которые могут использоваться как кэш данных. |
| [setCloudPlatform(boolean value)](#setCloudPlatform-boolean-) | Пожалуйста, установите это свойство в True при работе на облачной платформе, такой как: Azure, AWSLambda и т.д., |
| [setCustomImplementationFactory(CustomImplementationFactory value)](#setCustomImplementationFactory-com.aspose.cells.CustomImplementationFactory-) | Устанавливает фабрику для создания экземпляров со специальной реализацией. |
| [setDPI(double value)](#setDPI-double-) | Получает DPI машины. |
| [setLibraryPath(String value)](#setLibraryPath-java.lang.String-) | Устанавливает путь к библиотеке, на который ссылаются некоторые внешние ссылки на формулы. |
| [setSignificantDigits(int value)](#setSignificantDigits-int-) | Устанавливает количество значимых цифр. |
| [setSignificantDigitsType(int value)](#setSignificantDigitsType-int-) | Устанавливает тип значимых цифр по умолчанию для вывода числовых значений. |
| [setStartupPath(String value)](#setStartupPath-java.lang.String-) | Устанавливает путь запуска, на который ссылаются некоторые внешние ссылки на формулы. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### addAddInFunction(String function, int minCountOfParameters, int maxCountOfParameters, int[] paramersType, int functionValueType) {#addAddInFunction-java.lang.String-int-int-int---int-}
```
public static void addAddInFunction(String function, int minCountOfParameters, int maxCountOfParameters, int[] paramersType, int functionValueType)
```


Добавить функцию надстройки.

**Remarks**

ПРИМЕЧАНИЕ: Этот член теперь устарел. Вместо него, пожалуйста, используйте методы WorksheetCollection.RegisterAddInFunction(). Этот метод будет удалён через 12 месяцев, начиная с января 2022 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| функция | java.lang.String | Имя функции. |
| minCountOfParameters | int | Минимальное количество параметров, требуемых этой функцией |
| maxCountOfParameters | int | Максимальное количество параметров, разрешённых этой функцией. |
| paramersType | int[] | [ParameterType](../../com.aspose.cells/parametertype). Ожидаемый тип параметров функции |
| functionValueType | int | [ParameterType](../../com.aspose.cells/parametertype). Тип значения функции. |

### cellIndexToName(int row, int column) {#cellIndexToName-int-int-}
```
public static String cellIndexToName(int row, int column)
```


Получает имя ячейки по её индексам строки и столбца.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| строка | int | Индекс строки. |
| столбец | int | Индекс столбца. |

**Returns:**
java.lang.String - Имя ячейки.
### cellNameToIndex(String cellName) {#cellNameToIndex-java.lang.String-}
```
public static int[] cellNameToIndex(String cellName)
```


Получает индексы строки и столбца ячейки по её имени.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| cellName | java.lang.String | Имя ячейки |

**Returns:**
int[] - [0] — индекс строки, а [1] — индекс столбца.
### columnIndexToName(int column) {#columnIndexToName-int-}
```
public static String columnIndexToName(int column)
```


Получает имя столбца по индексу столбца.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| столбец | int | Индекс столбца. |

**Returns:**
java.lang.String - Имя столбца.
### columnNameToIndex(String columnName) {#columnNameToIndex-java.lang.String-}
```
public static int columnNameToIndex(String columnName)
```


Получает индекс столбца по имени столбца.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| columnName | java.lang.String | Имя столбца. |

**Returns:**
int - Индекс столбца.
### convertA1FormulaToR1C1(String formula, int row, int column) {#convertA1FormulaToR1C1-java.lang.String-int-int-}
```
public static String convertA1FormulaToR1C1(String formula, int row, int column)
```


Преобразует формулу A1 ячейки в формулу r1c1.

**Remarks**

ПРИМЕЧАНИЕ: Этот член теперь устарел. Вместо него, пожалуйста, используйте метод Worksheet.ConvertFormulaReferenceStyle(). Это свойство будет удалено через 12 месяцев, начиная с августа 2023 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| formula | java.lang.String | Формула A1. |
| строка | int | Индекс строки ячейки. |
| столбец | int | Индекс столбца ячейки. |

**Returns:**
java.lang.String - Формула R1C1.
### convertR1C1FormulaToA1(String r1c1Formula, int row, int column) {#convertR1C1FormulaToA1-java.lang.String-int-int-}
```
public static String convertR1C1FormulaToA1(String r1c1Formula, int row, int column)
```


Преобразует формулу r1c1 ячейки в формулу A1.

**Remarks**

ПРИМЕЧАНИЕ: Этот член теперь устарел. Вместо него, пожалуйста, используйте метод Worksheet.ConvertFormulaReferenceStyle(). Это свойство будет удалено через 12 месяцев, начиная с августа 2023 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| r1c1Formula | java.lang.String | Формула r1c1. |
| строка | int | Индекс строки ячейки. |
| столбец | int | Индекс столбца ячейки. |

**Returns:**
java.lang.String - Формула A1.
### createSafeSheetName(String nameProposal) {#createSafeSheetName-java.lang.String-}
```
public static String createSafeSheetName(String nameProposal)
```


Проверяет заданное имя листа и при необходимости создает корректное. Если заданное имя листа соответствует правилам имен листов Excel, возвращает его. В противном случае строка будет обрезана, если её длина превышает ограничение, а недопустимые символы будут заменены на пробел ' ', после чего возвращается восстановленное значение строки.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| nameProposal | java.lang.String | имя листа, которое будет использоваться |

**Returns:**
java.lang.String -
### createSafeSheetName(String nameProposal, char replaceChar) {#createSafeSheetName-java.lang.String-char-}
```
public static String createSafeSheetName(String nameProposal, char replaceChar)
```


Проверяет заданное имя листа и при необходимости создает корректное. Если заданное имя листа соответствует правилам имен листов Excel, возвращает его. В противном случае строка будет обрезана, если её длина превышает ограничение, а недопустимые символы будут заменены заданным символом, после чего возвращается восстановленное значение строки.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| nameProposal | java.lang.String | имя листа, которое будет использоваться |
| replaceChar | char | символ, который будет использоваться для замены недопустимых символов в заданном имени листа |

**Returns:**
java.lang.String -
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
### getAltStartPath() {#getAltStartPath--}
```
public static String getAltStartPath()
```


Получает альтернативный путь запуска, на который ссылаются некоторые внешние формульные ссылки.

**Returns:**
java.lang.String
### getCacheFolder() {#getCacheFolder--}
```
public static String getCacheFolder()
```


Получает папку для временных файлов, которые могут использоваться как кэш данных.

**Remarks**

Файлы кэша обычно используются для некоторых функций с учётом производительности памяти, например для сохранения большого набора данных в файл xls или использования режима памяти с файловым кэшем для модели ячеек.

**Returns:**
java.lang.String - Папка для файлов кэша, если она указана. Если не указана, будет возвращено null, и при необходимости будет использован временный путь системы.
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getCustomImplementationFactory() {#getCustomImplementationFactory--}
```
public static CustomImplementationFactory getCustomImplementationFactory()
```


Получает фабрику для создания экземпляров со специальной реализацией.

**Returns:**
[CustomImplementationFactory](../../com.aspose.cells/customimplementationfactory)
### getDPI() {#getDPI--}
```
public static double getDPI()
```


Получает DPI машины.

**Remarks**

**Returns:**
double
### getDateTimeFromDouble(double doubleValue, boolean date1904) {#getDateTimeFromDouble-double-boolean-}
```
public static DateTime getDateTimeFromDouble(double doubleValue, boolean date1904)
```


Преобразует значение double в значение даты и времени.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| doubleValue | double | Значение типа double. |
| date1904 | boolean | Система даты 1904. |

**Returns:**
[DateTime](../../com.aspose.cells/datetime) - 
### getDoubleFromDateTime(DateTime dateTime, boolean date1904) {#getDoubleFromDateTime-com.aspose.cells.DateTime-boolean-}
```
public static double getDoubleFromDateTime(DateTime dateTime, boolean date1904)
```


Преобразует дату и время в значение double.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| dateTime | [DateTime](../../com.aspose.cells/datetime) | Дата и время. |
| date1904 | boolean | Система даты 1904. |

**Returns:**
double -
### getLibraryPath() {#getLibraryPath--}
```
public static String getLibraryPath()
```


Получает путь к библиотеке, на который ссылаются некоторые внешние формульные ссылки.

**Returns:**
java.lang.String
### getSignificantDigits() {#getSignificantDigits--}
```
public static int getSignificantDigits()
```


Получает количество значимых цифр. Значение по умолчанию — 17.

**Remarks**

Сейчас может быть только 15 или 17. ПРИМЕЧАНИЕ: Этот член теперь устарел. Вместо него, пожалуйста, используйте [getSignificantDigitsType()](../../com.aspose.cells/cellshelper\#getSignificantDigitsType--). Это свойство будет удалено через 12 месяцев, начиная с июня 2025 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

**Returns:**
int
### getSignificantDigitsType() {#getSignificantDigitsType--}
```
public static int getSignificantDigitsType()
```


Получает тип значимых цифр по умолчанию для вывода числовых значений. Значение по умолчанию — [SignificantDigitsType.G\_17](../../com.aspose.cells/significantdigitstype\#G-17).

Смотрите [SignificantDigitsType](../../com.aspose.cells/significantdigitstype).

**Returns:**
int
### getStartupPath() {#getStartupPath--}
```
public static String getStartupPath()
```


Получает путь запуска, на который ссылаются некоторые внешние формульные ссылки.

**Returns:**
java.lang.String
### getTextWidth(String text, Font font, double scaling) {#getTextWidth-java.lang.String-com.aspose.cells.Font-double-}
```
public static double getTextWidth(String text, Font font, double scaling)
```


Получить ширину текста в единицах точек.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| текст | java.lang.String | Текст. |
| font | [Font](../../com.aspose.cells/font) | Шрифт текста. |
| масштабирование | double | Масштабирование текста. |

**Returns:**
double -
### getUsedColors(Workbook workbook) {#getUsedColors-com.aspose.cells.Workbook-}
```
public static Color[] getUsedColors(Workbook workbook)
```


Получает все используемые цвета в рабочей книге.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| workbook | [Workbook](../../com.aspose.cells/workbook) | Объект рабочей книги. |

**Returns:**
com.aspose.cells.Color[] - Используемые цвета.
### getVersion() {#getVersion--}
```
public static String getVersion()
```


Получить версию релиза.

**Returns:**
java.lang.String - Версия выпуска.
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isCloudPlatform() {#isCloudPlatform--}
```
public static boolean isCloudPlatform()
```


Пожалуйста, установите это свойство в True при работе на облачной платформе, такой как: Azure, AWSLambda и т.д.,

**Returns:**
boolean
### mergeFiles(String[] files, String cachedFile, String destFile) {#mergeFiles-java.lang.String---java.lang.String-java.lang.String-}
```
public static void mergeFiles(String[] files, String cachedFile, String destFile)
```


Объединяет несколько больших файлов xls в один файл xls.

**Remarks**

Этот метод поддерживает только объединение данных, стилей и формул в новый файл. Кэшированный файл используется для хранения некоторых временных данных.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| файлы | java.lang.String[] | Файлы. |
| cachedFile | java.lang.String | Кэшированный файл. |
| destFile | java.lang.String | Файл назначения. |

### needQuoteInFormula(String sheetName) {#needQuoteInFormula-java.lang.String-}
```
public static boolean needQuoteInFormula(String sheetName)
```


Указывает, следует ли заключать имя листа в одинарные кавычки

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| sheetName | java.lang.String | Имя листа |

**Returns:**
boolean -
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### rowIndexToName(int row) {#rowIndexToName-int-}
```
public static String rowIndexToName(int row)
```


Получает имя строки по индексу строки.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| строка | int | Индекс строки. |

**Returns:**
java.lang.String - Имя строки.
### rowNameToIndex(String rowName) {#rowNameToIndex-java.lang.String-}
```
public static int rowNameToIndex(String rowName)
```


Получает индекс строки по имени строки.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| rowName | java.lang.String | Имя строки. |

**Returns:**
int - Индекс строки.
### setAltStartPath(String value) {#setAltStartPath-java.lang.String-}
```
public static void setAltStartPath(String value)
```


Устанавливает альтернативный путь запуска, на который ссылаются некоторые внешние формульные ссылки.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### setCacheFolder(String cache) {#setCacheFolder-java.lang.String-}
```
public static void setCacheFolder(String cache)
```


Устанавливает папку для временных файлов, которые могут использоваться как кэш данных.

**Remarks**

Файлы кэша обычно используются для некоторых функций с учётом производительности памяти, например для сохранения большого набора данных в файл xls или использования режима памяти с файловым кэшем для модели ячеек.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| кеш | java.lang.String | Папка для временных файлов, которые могут использоваться в качестве кэша данных. |

### setCloudPlatform(boolean value) {#setCloudPlatform-boolean-}
```
public static void setCloudPlatform(boolean value)
```


Пожалуйста, установите это свойство в True при работе на облачной платформе, такой как: Azure, AWSLambda и т.д.,

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setCustomImplementationFactory(CustomImplementationFactory value) {#setCustomImplementationFactory-com.aspose.cells.CustomImplementationFactory-}
```
public static void setCustomImplementationFactory(CustomImplementationFactory value)
```


Устанавливает фабрику для создания экземпляров со специальной реализацией.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| value | [CustomImplementationFactory](../../com.aspose.cells/customimplementationfactory) |  |

### setDPI(double value) {#setDPI-double-}
```
public static void setDPI(double value)
```


Получает DPI машины.

**Remarks**

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | double |  |

### setLibraryPath(String value) {#setLibraryPath-java.lang.String-}
```
public static void setLibraryPath(String value)
```


Устанавливает путь к библиотеке, на который ссылаются некоторые внешние ссылки на формулы.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### setSignificantDigits(int value) {#setSignificantDigits-int-}
```
public static void setSignificantDigits(int value)
```


Устанавливает количество значимых цифр. Значение по умолчанию — 17.

**Remarks**

Сейчас может быть только 15 или 17. ПРИМЕЧАНИЕ: Этот член теперь устарел. Вместо него, пожалуйста, используйте [getSignificantDigitsType()](../../com.aspose.cells/cellshelper\#getSignificantDigitsType--). Это свойство будет удалено через 12 месяцев, начиная с июня 2025 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setSignificantDigitsType(int value) {#setSignificantDigitsType-int-}
```
public static void setSignificantDigitsType(int value)
```


Устанавливает тип значимых цифр по умолчанию для вывода числовых значений. Значение по умолчанию — [SignificantDigitsType.G\_17](../../com.aspose.cells/significantdigitstype\#G-17).

Смотрите [SignificantDigitsType](../../com.aspose.cells/significantdigitstype).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setStartupPath(String value) {#setStartupPath-java.lang.String-}
```
public static void setStartupPath(String value)
```


Устанавливает путь запуска, на который ссылаются некоторые внешние ссылки на формулы.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

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

