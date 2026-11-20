---
title: "WorkbookSettings"
second_title: "Справочник API Aspose.Cells for Java"
description: "Представляет все настройки рабочей книги."
type: docs
url: /ru/java/com.aspose.cells/workbooksettings/
---

**Inheritance:**
java.lang.Object
```
public class WorkbookSettings
```

Представляет все настройки рабочей книги.

**Example**

```
         Workbook workbook = new Workbook();
 
         WorkbookSettings settings = workbook.getSettings();
 
         //do your business
```
## Методы

| Метод | Описание |
| --- | --- |
| [dispose()](#dispose--) | Освобождает ресурсы. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAuthor()](#getAuthor--) | Получает автора файла. |
| [getAutoCompressPictures()](#getAutoCompressPictures--) | Указывает логическое значение, которое показывает, что приложение автоматически сжимает изображения в рабочей книге. |
| [getAutoRecover()](#getAutoRecover--) | Указывает, помечен ли файл для автоматического восстановления. |
| [getBuildVersion()](#getBuildVersion--) | Указывает инкрементальный публичный релиз приложения. |
| [getCheckCompatibility()](#getCheckCompatibility--) | Указывает, проверять ли совместимость с более ранними версиями при сохранении рабочей книги. |
| [getCheckCustomNumberFormat()](#getCheckCustomNumberFormat--) | Указывает, проверять ли пользовательский числовой формат при установке Style.Custom. |
| [getCheckExcelRestriction()](#getCheckExcelRestriction--) | Проверять ли ограничения Excel‑файла, когда пользователь изменяет связанные с ячейками объекты. |
| [getClass()](#getClass--) |  |
| [getCompliance()](#getCompliance--) | Указывает версию OOXML для выходного документа. |
| [getCrashSave()](#getCrashSave--) | Указывает, сохранял ли приложение последний раз файл рабочей книги после сбоя. |
| [getDataExtractLoad()](#getDataExtractLoad--) | Указывает, открыл ли приложение последний раз рабочую книгу для восстановления данных. |
| [getDate1904()](#getDate1904--) | Получает значение, которое показывает, использует ли рабочая книга систему дат 1904 года. |
| [getDefaultImageResolution()](#getDefaultImageResolution--) | Получает разрешение изображения по умолчанию. |
| [getDefaultStyleSettings()](#getDefaultStyleSettings--) | Получает настройки значений по умолчанию свойств, связанных со стилем, для этой рабочей книги. |
| [getDiscardImageEditData()](#getDiscardImageEditData--) | Указывает, следует ли отбрасывать редактируемые данные изображения. |
| [getDisplayDrawingObjects()](#getDisplayDrawingObjects--) | Указывает, показывать ли объекты в рабочей книге и как. |
| [getEnableMacros()](#getEnableMacros--) | Включить макросы; |
| [getFirstVisibleTab()](#getFirstVisibleTab--) | Получает первую видимую вкладку листа. |
| [getFormulaSettings()](#getFormulaSettings--) | Получает настройки функций, связанных с формулами. |
| [getGlobalizationSettings()](#getGlobalizationSettings--) | Получает настройки глобализации. |
| [getHidePivotFieldList()](#getHidePivotFieldList--) | Получает, скрывать ли список полей для сводной таблицы. |
| [getLanguageCode()](#getLanguageCode--) | Получает язык пользовательского интерфейса версии рабочей книги, основанный на CountryCode, в котором файл был сохранён. |
| [getLocale()](#getLocale--) | Получает локаль, используемую этой рабочей книгой. |
| [getMaxColumn()](#getMaxColumn--) | Получает максимальный индекс столбца, начиная с нуля. |
| [getMaxRow()](#getMaxRow--) | Получает максимальный индекс строки, начиная с нуля. |
| [getMaxRowsOfSharedFormula()](#getMaxRowsOfSharedFormula--) | Получает максимальный номер строки общей формулы. |
| [getMaxUniqueItemsPerField()](#getMaxUniqueItemsPerField--) | Получает ограничение уникальных элементов на поле |
| [getMemorySetting()](#getMemorySetting--) | Получает параметры использования памяти. |
| [getNumberDecimalSeparator()](#getNumberDecimalSeparator--) | Получает десятичный разделитель для форматирования/разбора числовых значений. |
| [getNumberGroupSeparator()](#getNumberGroupSeparator--) | Получает символ, разделяющий группы цифр слева от десятичной точки в числовых значениях. |
| [getPaperSize()](#getPaperSize--) | Получает размер бумаги по умолчанию для печати. |
| [getPassword()](#getPassword--) | Представляет пароль шифрования файла Workbook. |
| [getPropertiesFollowChartPoint()](#getPropertiesFollowChartPoint--) | Указывает, следуют ли свойства точек данных и подписи данных во всех диаграммах этой книги их ссылке. |
| [getProtectionType()](#getProtectionType--) | Получает тип защиты книги. |
| [getQuotePrefixToStyle()](#getQuotePrefixToStyle--) | Указывает, применяется ли свойство [Style.getQuotePrefix()](../../com.aspose.cells/style\#getQuotePrefix--) при вводе строкового значения (которое начинается с одинарной кавычки) в ячейку |
| [getRegion()](#getRegion--) | Получает региональные настройки книги. |
| [getRemovePersonalInformation()](#getRemovePersonalInformation--) | Истина, если личную информацию можно удалить из указанной книги. |
| [getRepairLoad()](#getRepairLoad--) | Указывает, открыла ли приложение книгу в безопасном или режиме восстановления в последний раз. |
| [getResourceProvider()](#getResourceProvider--) | Получает поставщика потоков для внешнего ресурса, например загрузки данных изображения для картинки типа "LinkToFile". |
| [getShapeDisplayType()](#getShapeDisplayType--) | Получает способ отображения фигур приложением в этой книге |
| [getShared()](#getShared--) | Получает значение, указывающее, является ли книга общей. |
| [getSheetTabBarWidth()](#getSheetTabBarWidth--) | Ширина панели вкладок листов (в 1/1000 ширины окна). |
| [getShowTabs()](#getShowTabs--) | Получает значение, указывающее, отображаются ли вкладки книги. |
| [getSignificantDigits()](#getSignificantDigits--) | Получает количество значимых цифр. |
| [getSignificantDigitsType()](#getSignificantDigitsType--) | Получает тип значимых цифр для вывода числовых значений в этой книге. |
| [getSmartTagOptions()](#getSmartTagOptions--) | Получает параметры смарт-тега. |
| [getStreamProvider()](#getStreamProvider--) | Получает поставщика потоков для внешнего ресурса. |
| [getThemeFont(int type)](#getThemeFont-int-) | Получает название шрифта темы по умолчанию. |
| [getUpdateAdjacentCellsBorder()](#getUpdateAdjacentCellsBorder--) | Указывает, обновлять ли границу соседних ячеек. |
| [getUpdateLinksType()](#getUpdateLinksType--) | Получает способ обновления внешних ссылок при открытии книги. |
| [getWarningCallback()](#getWarningCallback--) | Получает обратный вызов предупреждения. |
| [getWindowHeight()](#getWindowHeight--) | Высота окна в пунктах. |
| [getWindowHeightCM()](#getWindowHeightCM--) | Высота окна в сантиметрах. |
| [getWindowHeightInch()](#getWindowHeightInch--) | Высота окна в единицах дюйма. |
| [getWindowLeft()](#getWindowLeft--) | Расстояние от левого края клиентской области до левого края окна в единицах пункта. |
| [getWindowLeftCM()](#getWindowLeftCM--) | Расстояние от левого края клиентской области до левого края окна. |
| [getWindowLeftInch()](#getWindowLeftInch--) | Расстояние от левого края клиентской области до левого края окна. |
| [getWindowTop()](#getWindowTop--) | Расстояние от верхнего края клиентской области до верхнего края окна в единицах пункта. |
| [getWindowTopCM()](#getWindowTopCM--) | Расстояние от верхнего края клиентской области до верхнего края окна в единицах сантиметра. |
| [getWindowTopInch()](#getWindowTopInch--) | Расстояние от верхнего края клиентской области до верхнего края окна в единицах дюйма. |
| [getWindowWidth()](#getWindowWidth--) | Ширина окна в единицах пункта. |
| [getWindowWidthCM()](#getWindowWidthCM--) | Ширина окна в единицах сантиметра. |
| [getWindowWidthInch()](#getWindowWidthInch--) | Ширина окна в единицах дюйма. |
| [getWpsCompatibility()](#getWpsCompatibility--) | Указывает, следует ли быть совместимым с WPS. |
| [getWriteProtection()](#getWriteProtection--) | Обеспечивает доступ к параметрам защиты записи книги. |
| [hashCode()](#hashCode--) |  |
| [isDefaultEncrypted()](#isDefaultEncrypted--) | Указывает, следует ли шифровать книгу паролем по умолчанию, если структура и окна книги заблокированы. |
| [isEncrypted()](#isEncrypted--) | Получает значение, указывающее, требуется ли пароль для открытия этой книги. |
| [isHScrollBarVisible()](#isHScrollBarVisible--) | Получает значение, указывающее, будет ли сгенерированная таблица содержать горизонтальную полосу прокрутки. |
| [isHidden()](#isHidden--) | Указывает, скрыта ли эта книга. |
| [isMinimized()](#isMinimized--) | Представляет, будет ли сгенерированная таблица открыта в свернутом виде. |
| [isProtected()](#isProtected--) | Получает значение, указывающее, защищены ли структура или окно книги. |
| [isVScrollBarVisible()](#isVScrollBarVisible--) | Получает значение, указывающее, будет ли сгенерированная таблица содержать вертикальную полосу прокрутки. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAuthor(String value)](#setAuthor-java.lang.String-) | Устанавливает автора файла. |
| [setAutoCompressPictures(boolean value)](#setAutoCompressPictures-boolean-) | Указывает логическое значение, которое показывает, что приложение автоматически сжимает изображения в рабочей книге. |
| [setAutoRecover(boolean value)](#setAutoRecover-boolean-) | Указывает, помечен ли файл для автоматического восстановления. |
| [setBuildVersion(String value)](#setBuildVersion-java.lang.String-) | Указывает инкрементальный публичный релиз приложения. |
| [setCheckCompatibility(boolean value)](#setCheckCompatibility-boolean-) | Указывает, проверять ли совместимость с более ранними версиями при сохранении рабочей книги. |
| [setCheckCustomNumberFormat(boolean value)](#setCheckCustomNumberFormat-boolean-) | Указывает, проверять ли пользовательский числовой формат при установке Style.Custom. |
| [setCheckExcelRestriction(boolean value)](#setCheckExcelRestriction-boolean-) | Проверять ли ограничения Excel‑файла, когда пользователь изменяет связанные с ячейками объекты. |
| [setCompliance(int value)](#setCompliance-int-) | Указывает версию OOXML для выходного документа. |
| [setCrashSave(boolean value)](#setCrashSave-boolean-) | Указывает, сохранял ли приложение последний раз файл рабочей книги после сбоя. |
| [setDataExtractLoad(boolean value)](#setDataExtractLoad-boolean-) | Указывает, открыл ли приложение последний раз рабочую книгу для восстановления данных. |
| [setDate1904(boolean value)](#setDate1904-boolean-) | Устанавливает значение, указывающее, использует ли книга систему дат 1904 года. |
| [setDefaultEncrypted(boolean value)](#setDefaultEncrypted-boolean-) | Указывает, следует ли шифровать книгу паролем по умолчанию, если структура и окна книги заблокированы. |
| [setDefaultImageResolution(int value)](#setDefaultImageResolution-int-) | Устанавливает разрешение изображения по умолчанию. |
| [setDiscardImageEditData(boolean value)](#setDiscardImageEditData-boolean-) | Указывает, следует ли отбрасывать редактируемые данные изображения. |
| [setDisplayDrawingObjects(int value)](#setDisplayDrawingObjects-int-) | Указывает, показывать ли объекты в рабочей книге и как. |
| [setEnableMacros(boolean value)](#setEnableMacros-boolean-) | Включить макросы; |
| [setFirstVisibleTab(int value)](#setFirstVisibleTab-int-) | Устанавливает первую видимую вкладку листа. |
| [setGlobalizationSettings(GlobalizationSettings value)](#setGlobalizationSettings-com.aspose.cells.GlobalizationSettings-) | Устанавливает параметры глобализации. |
| [setHScrollBarVisible(boolean value)](#setHScrollBarVisible-boolean-) | Устанавливает значение, указывающее, будет ли сгенерированная таблица содержать горизонтальную полосу прокрутки. |
| [setHidden(boolean value)](#setHidden-boolean-) | Указывает, скрыта ли эта книга. |
| [setHidePivotFieldList(boolean value)](#setHidePivotFieldList-boolean-) | Устанавливает, скрывать ли список полей для сводной таблицы. |
| [setLanguageCode(int value)](#setLanguageCode-int-) | Устанавливает язык пользовательского интерфейса версии Workbook на основе CountryCode, в которой был сохранён файл. |
| [setLocale(Locale value)](#setLocale-java.util.Locale-) | Устанавливает локаль, используемую этой книгой. |
| [setMaxRowsOfSharedFormula(int value)](#setMaxRowsOfSharedFormula-int-) | Устанавливает максимальный номер строки общей формулы. |
| [setMaxUniqueItemsPerField(int value)](#setMaxUniqueItemsPerField-int-) | Устанавливает ограничение уникальных элементов на поле. |
| [setMemorySetting(int value)](#setMemorySetting-int-) | Устанавливает параметры использования памяти. |
| [setMinimized(boolean value)](#setMinimized-boolean-) | Представляет, будет ли сгенерированная таблица открыта в свернутом виде. |
| [setNumberDecimalSeparator(char value)](#setNumberDecimalSeparator-char-) | Устанавливает десятичный разделитель для форматирования/парсинга числовых значений. |
| [setNumberGroupSeparator(char value)](#setNumberGroupSeparator-char-) | Устанавливает символ, разделяющий группы цифр слева от десятичной точки в числовых значениях. |
| [setPageOrientationType(int pageOrientationType)](#setPageOrientationType-int-) | Устанавливает тип ориентации печати для всей книги. |
| [setPaperSize(int value)](#setPaperSize-int-) | Устанавливает размер бумаги по умолчанию для печати. |
| [setPassword(String value)](#setPassword-java.lang.String-) | Представляет пароль шифрования файла Workbook. |
| [setPropertiesFollowChartPoint(boolean value)](#setPropertiesFollowChartPoint-boolean-) | Указывает, следуют ли свойства точек данных и подписи данных во всех диаграммах этой книги их ссылке. |
| [setQuotePrefixToStyle(boolean value)](#setQuotePrefixToStyle-boolean-) | Указывает, применяется ли свойство [Style.getQuotePrefix()](../../com.aspose.cells/style\#getQuotePrefix--) при вводе строкового значения (которое начинается с одинарной кавычки) в ячейку |
| [setRegion(int value)](#setRegion-int-) | Устанавливает региональные настройки для книги. |
| [setRemovePersonalInformation(boolean value)](#setRemovePersonalInformation-boolean-) | Истина, если личную информацию можно удалить из указанной книги. |
| [setRepairLoad(boolean value)](#setRepairLoad-boolean-) | Указывает, открыла ли приложение книгу в безопасном или режиме восстановления в последний раз. |
| [setResourceProvider(IStreamProvider value)](#setResourceProvider-com.aspose.cells.IStreamProvider-) | Устанавливает поставщика потоков для внешних ресурсов, например загрузку данных изображения для картинки типа "LinkToFile". |
| [setShapeDisplayType(int value)](#setShapeDisplayType-int-) | Устанавливает, как приложение отображает фигуры в этой книге. |
| [setShared(boolean value)](#setShared-boolean-) | Устанавливает значение, указывающее, является ли книга общей. |
| [setSheetTabBarWidth(int value)](#setSheetTabBarWidth-int-) | Ширина панели вкладок листов (в 1/1000 ширины окна). |
| [setShowTabs(boolean value)](#setShowTabs-boolean-) | Устанавливает значение, отображаются ли вкладки книги. |
| [setSignificantDigits(int value)](#setSignificantDigits-int-) | Устанавливает количество значимых цифр. |
| [setSignificantDigitsType(int value)](#setSignificantDigitsType-int-) | Устанавливает тип значимых цифр для вывода числовых значений в этой книге. |
| [setStreamProvider(IStreamProvider value)](#setStreamProvider-com.aspose.cells.IStreamProvider-) | Устанавливает поставщика потоков для внешнего ресурса. |
| [setUpdateAdjacentCellsBorder(boolean value)](#setUpdateAdjacentCellsBorder-boolean-) | Указывает, обновлять ли границу соседних ячеек. |
| [setUpdateLinksType(int value)](#setUpdateLinksType-int-) | Устанавливает, как обновлять внешние ссылки при открытии книги. |
| [setVScrollBarVisible(boolean value)](#setVScrollBarVisible-boolean-) | Устанавливает значение, указывающее, будет ли сгенерированная таблица содержать вертикальную полосу прокрутки. |
| [setWarningCallback(IWarningCallback value)](#setWarningCallback-com.aspose.cells.IWarningCallback-) | Устанавливает обратный вызов предупреждения. |
| [setWindowHeight(double value)](#setWindowHeight-double-) | Высота окна в пунктах. |
| [setWindowHeightCM(double value)](#setWindowHeightCM-double-) | Высота окна в сантиметрах. |
| [setWindowHeightInch(double value)](#setWindowHeightInch-double-) | Высота окна в единицах дюйма. |
| [setWindowLeft(double value)](#setWindowLeft-double-) | Расстояние от левого края клиентской области до левого края окна в единицах пункта. |
| [setWindowLeftCM(double value)](#setWindowLeftCM-double-) | Расстояние от левого края клиентской области до левого края окна. |
| [setWindowLeftInch(double value)](#setWindowLeftInch-double-) | Расстояние от левого края клиентской области до левого края окна. |
| [setWindowTop(double value)](#setWindowTop-double-) | Расстояние от верхнего края клиентской области до верхнего края окна в единицах пункта. |
| [setWindowTopCM(double value)](#setWindowTopCM-double-) | Расстояние от верхнего края клиентской области до верхнего края окна в единицах сантиметра. |
| [setWindowTopInch(double value)](#setWindowTopInch-double-) | Расстояние от верхнего края клиентской области до верхнего края окна в единицах дюйма. |
| [setWindowWidth(double value)](#setWindowWidth-double-) | Ширина окна в единицах пункта. |
| [setWindowWidthCM(double value)](#setWindowWidthCM-double-) | Ширина окна в единицах сантиметра. |
| [setWindowWidthInch(double value)](#setWindowWidthInch-double-) | Ширина окна в единицах дюйма. |
| [setWpsCompatibility(boolean value)](#setWpsCompatibility-boolean-) | Указывает, следует ли быть совместимым с WPS. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### dispose() {#dispose--}
```
public void dispose()
```


Освобождает ресурсы.

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
### getAuthor() {#getAuthor--}
```
public String getAuthor()
```


Получает автора файла.

**Remarks**

Не установлено, сначала проверьте [BuiltInDocumentPropertyCollection.getAuthor()](../../com.aspose.cells/builtindocumentpropertycollection\#getAuthor--), затем проверьте пользователя среды Environment.

**Returns:**
java.lang.String
### getAutoCompressPictures() {#getAutoCompressPictures--}
```
public boolean getAutoCompressPictures()
```


Указывает логическое значение, которое показывает, что приложение автоматически сжимает изображения в рабочей книге.

**Returns:**
boolean
### getAutoRecover() {#getAutoRecover--}
```
public boolean getAutoRecover()
```


Указывает, помечен ли файл для автоматического восстановления.

**Returns:**
boolean
### getBuildVersion() {#getBuildVersion--}
```
public String getBuildVersion()
```


Указывает инкрементальный публичный релиз приложения.

**Returns:**
java.lang.String
### getCheckCompatibility() {#getCheckCompatibility--}
```
public boolean getCheckCompatibility()
```


Указывает, проверять ли совместимость с более ранними версиями при сохранении рабочей книги.

**Remarks**

Значение по умолчанию — true. Только для файлов Excel97-2003 xls или xlt.

**Returns:**
boolean
### getCheckCustomNumberFormat() {#getCheckCustomNumberFormat--}
```
public boolean getCheckCustomNumberFormat()
```


Указывает, проверять ли пользовательский числовой формат при установке Style.Custom.

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
### getCompliance() {#getCompliance--}
```
public int getCompliance()
```


Указывает версию OOXML для выходного документа. Значение по умолчанию — Ecma376\_2006.

См. [OoxmlCompliance](../../com.aspose.cells/ooxmlcompliance).

**Remarks**

Только для файлов .xlsx.

**Returns:**
int
### getCrashSave() {#getCrashSave--}
```
public boolean getCrashSave()
```


Указывает, сохранял ли приложение последний раз файл рабочей книги после сбоя.

**Returns:**
boolean
### getDataExtractLoad() {#getDataExtractLoad--}
```
public boolean getDataExtractLoad()
```


Указывает, открыл ли приложение последний раз рабочую книгу для восстановления данных.

**Returns:**
boolean
### getDate1904() {#getDate1904--}
```
public boolean getDate1904()
```


Получает значение, которое показывает, использует ли рабочая книга систему дат 1904 года.

**Returns:**
boolean
### getDefaultImageResolution() {#getDefaultImageResolution--}
```
public int getDefaultImageResolution()
```


Получает разрешение изображения по умолчанию.

**Returns:**
int
### getDefaultStyleSettings() {#getDefaultStyleSettings--}
```
public DefaultStyleSettings getDefaultStyleSettings()
```


Получает настройки значений по умолчанию свойств, связанных со стилем, для этой рабочей книги.

**Returns:**
[DefaultStyleSettings](../../com.aspose.cells/defaultstylesettings)
### getDiscardImageEditData() {#getDiscardImageEditData--}
```
public boolean getDiscardImageEditData()
```


Указывает, следует ли отбрасывать редактируемые данные изображения.

**Returns:**
boolean
### getDisplayDrawingObjects() {#getDisplayDrawingObjects--}
```
public int getDisplayDrawingObjects()
```


Указывает, показывать ли объекты в рабочей книге и как.

См. [DisplayDrawingObjects](../../com.aspose.cells/displaydrawingobjects).

**Returns:**
int
### getEnableMacros() {#getEnableMacros--}
```
public boolean getEnableMacros()
```


Включить макросы;

**Remarks**

Сейчас это работает только при копировании листа в другой лист в книге.

**Returns:**
boolean
### getFirstVisibleTab() {#getFirstVisibleTab--}
```
public int getFirstVisibleTab()
```


Получает первую видимую вкладку листа.

**Returns:**
int
### getFormulaSettings() {#getFormulaSettings--}
```
public FormulaSettings getFormulaSettings()
```


Получает настройки функций, связанных с формулами.

**Returns:**
[FormulaSettings](../../com.aspose.cells/formulasettings)
### getGlobalizationSettings() {#getGlobalizationSettings--}
```
public GlobalizationSettings getGlobalizationSettings()
```


Получает настройки глобализации.

**Returns:**
[GlobalizationSettings](../../com.aspose.cells/globalizationsettings)
### getHidePivotFieldList() {#getHidePivotFieldList--}
```
public boolean getHidePivotFieldList()
```


Получает, скрывать ли список полей для сводной таблицы.

**Returns:**
boolean
### getLanguageCode() {#getLanguageCode--}
```
public int getLanguageCode()
```


Получает язык пользовательского интерфейса версии рабочей книги, основанный на CountryCode, в котором файл был сохранён.

Смотрите [CountryCode](../../com.aspose.cells/countrycode).

**Returns:**
int
### getLocale() {#getLocale--}
```
public Locale getLocale()
```


Получает локаль, используемую этой рабочей книгой.

**Remarks**

Возвращает null, если не установлена ни локаль, ни [getRegion()](../../com.aspose.cells/workbooksettings\#getRegion--).

**Returns:**
java.util.Locale
### getMaxColumn() {#getMaxColumn--}
```
public int getMaxColumn()
```


Получает максимальный индекс столбца, начиная с нуля.

**Remarks**

Возвращает 255, если формат файла — Excel97-2003;

**Returns:**
int
### getMaxRow() {#getMaxRow--}
```
public int getMaxRow()
```


Получает максимальный индекс строки, начиная с нуля.

**Remarks**

Возвращает 65535, если формат файла — Excel97-2003;

**Returns:**
int
### getMaxRowsOfSharedFormula() {#getMaxRowsOfSharedFormula--}
```
public int getMaxRowsOfSharedFormula()
```


Получает максимальный номер строки общей формулы.

**Remarks**

Если число слишком велико, автофильтр работает очень медленно в MS Excel 2013.

**Returns:**
int
### getMaxUniqueItemsPerField() {#getMaxUniqueItemsPerField--}
```
public int getMaxUniqueItemsPerField()
```


Получает ограничение уникальных элементов на поле

**Remarks**

**Returns:**
int
### getMemorySetting() {#getMemorySetting--}
```
public int getMemorySetting()
```


Получает параметры использования памяти. Новый параметр будет принят в качестве параметра по умолчанию для только что созданных листов, но не будет применяться к существующим листам.

Смотрите [MemorySetting](../../com.aspose.cells/memorysetting).

**Remarks**

Для получения более подробной информации о режиме памяти, пожалуйста, смотрите [Cells.getMemorySetting()](../../com.aspose.cells/cells\#getMemorySetting--).

**Returns:**
int
### getNumberDecimalSeparator() {#getNumberDecimalSeparator--}
```
public char getNumberDecimalSeparator()
```


Получает десятичный разделитель для форматирования/парсинга числовых значений. По умолчанию используется десятичный разделитель текущего региона.

**Returns:**
char
### getNumberGroupSeparator() {#getNumberGroupSeparator--}
```
public char getNumberGroupSeparator()
```


Получает символ, разделяющий группы цифр слева от десятичной точки в числовых значениях. По умолчанию используется разделитель групп текущего региона.

**Returns:**
char
### getPaperSize() {#getPaperSize--}
```
public int getPaperSize()
```


Получает размер бумаги по умолчанию для печати.

Смотрите [PaperSizeType](../../com.aspose.cells/papersizetype).

**Remarks**

Если настройка размера бумаги отсутствует, MS Excel будет использовать настройки принтера по умолчанию.

**Returns:**
int
### getPassword() {#getPassword--}
```
public String getPassword()
```


Представляет пароль шифрования файла Workbook.

**Returns:**
java.lang.String
### getPropertiesFollowChartPoint() {#getPropertiesFollowChartPoint--}
```
public boolean getPropertiesFollowChartPoint()
```


Указывает, следуют ли свойства точек данных и подписи данных во всех диаграммах этой книги их ссылке.

**Returns:**
boolean
### getProtectionType() {#getProtectionType--}
```
public int getProtectionType()
```


Получает тип защиты книги.

Смотрите [ProtectionType](../../com.aspose.cells/protectiontype).

**Returns:**
int
### getQuotePrefixToStyle() {#getQuotePrefixToStyle--}
```
public boolean getQuotePrefixToStyle()
```


Указывает, применяется ли свойство [Style.getQuotePrefix()](../../com.aspose.cells/style\#getQuotePrefix--) при вводе строкового значения (которое начинается с одинарной кавычки) в ячейку

**Returns:**
boolean
### getRegion() {#getRegion--}
```
public int getRegion()
```


Получает региональные настройки книги.

Смотрите [CountryCode](../../com.aspose.cells/countrycode).

**Remarks**

1. Региональные настройки, используемые компонентом Aspose.Cells для книги, загруженной из шаблонного файла: i). Для файла XLS определены поля для региональных настроек, и MS Excel сохраняет данные региональных настроек в файл при сохранении XLS. Поэтому мы используем сохранённый регион из шаблонного файла для книги. Если вы не хотите использовать регион, сохранённый в файле XLS, пожалуйста, сбросьте его на требуемый (например, CountryCode.Default) после загрузки шаблонного файла. И мы также сохраняем пользовательское значение (с помощью этого метода) в файл при сохранении XLS. ii). Для других форматов файлов, таких как XLSX, XLSB и т.д., в спецификации формата нет поля для региональных настроек. Поэтому мы используем региональные настройки среды приложения для книги. И пользовательское значение (с помощью этого метода) не может быть сохранено в генерируемых файлах этих форматов. 2. Для отображения в MS Excel: применённые здесь региональные настройки могут действовать только во время выполнения с компонентом Aspose.Cells и не влияют при просмотре сгенерированного файла в MS Excel. Даже для сгенерированного XLS‑файла, в котором данные региональных настроек сохранены, при просмотре/редактировании его в MS Excel регион, используемый для форматирования, всегда является региональными настройками по умолчанию среды, где запущен MS Excel, а не тем, что сохранён в файле. Это поведение MS Excel и его нельзя изменить кодом.

**Returns:**
int
### getRemovePersonalInformation() {#getRemovePersonalInformation--}
```
public boolean getRemovePersonalInformation()
```


Истина, если личную информацию можно удалить из указанной книги.

**Remarks**

**Returns:**
boolean
### getRepairLoad() {#getRepairLoad--}
```
public boolean getRepairLoad()
```


Указывает, открыла ли приложение книгу в безопасном или режиме восстановления в последний раз.

**Returns:**
boolean
### getResourceProvider() {#getResourceProvider--}
```
public IStreamProvider getResourceProvider()
```


Получает поставщика потоков для внешнего ресурса, например загрузки данных изображения для картинки типа "LinkToFile".

**Returns:**
[IStreamProvider](../../com.aspose.cells/istreamprovider)
### getShapeDisplayType() {#getShapeDisplayType--}
```
public int getShapeDisplayType()
```


Получает способ отображения фигур приложением в этой книге

Смотрите [ShapeDisplayType](../../com.aspose.cells/shapedisplaytype).

**Returns:**
int
### getShared() {#getShared--}
```
public boolean getShared()
```


Получает значение, указывающее, является ли книга общей.

**Remarks**

Значение по умолчанию — false.

**Returns:**
boolean
### getSheetTabBarWidth() {#getSheetTabBarWidth--}
```
public int getSheetTabBarWidth()
```


Ширина панели вкладок листов (в 1/1000 ширины окна).

**Returns:**
int
### getShowTabs() {#getShowTabs--}
```
public boolean getShowTabs()
```


Получает значение, указывающее, отображаются ли вкладки книги.

**Remarks**

Значение по умолчанию — true.

**Example**

Следующий код скрывает вкладки листов и кнопки прокрутки вкладок в электронной таблице.

```
         // Hide the spreadsheet tabs.
         workbook.getSettings().setShowTabs(false);
```

**Returns:**
boolean
### getSignificantDigits() {#getSignificantDigits--}
```
public int getSignificantDigits()
```


Получает количество значимых цифр. Значение по умолчанию — [CellsHelper.getSignificantDigits()](../../com.aspose.cells/cellshelper\#getSignificantDigits--).

**Remarks**

Сейчас может быть только 15 или 17. ПРИМЕЧАНИЕ: Этот член теперь устарел. Вместо него используйте [getSignificantDigitsType()](../../com.aspose.cells/workbooksettings\#getSignificantDigitsType--). Это свойство будет удалено через 12 месяцев, начиная с июня 2025 года. Компания Aspose просит прощения за любые причинённые неудобства.

**Returns:**
int
### getSignificantDigitsType() {#getSignificantDigitsType--}
```
public int getSignificantDigitsType()
```


Получает тип значимых цифр для вывода числовых значений в этой книге. Значение по умолчанию — [CellsHelper.getSignificantDigitsType()](../../com.aspose.cells/cellshelper\#getSignificantDigitsType--).

Смотрите [SignificantDigitsType](../../com.aspose.cells/significantdigitstype).

**Returns:**
int
### getSmartTagOptions() {#getSmartTagOptions--}
```
public SmartTagOptions getSmartTagOptions()
```


Получает параметры смарт-тега.

**Returns:**
[SmartTagOptions](../../com.aspose.cells/smarttagoptions)
### getStreamProvider() {#getStreamProvider--}
```
public IStreamProvider getStreamProvider()
```


Получает поставщика потоков для внешнего ресурса.

**Remarks**

ПРИМЕЧАНИЕ: Этот член теперь устарел. Вместо него используйте свойство ResourceProvider. Это свойство будет удалено через 12 месяцев, начиная с июня 2022 года. Компания Aspose просит прощения за любые причинённые неудобства.

**Returns:**
[IStreamProvider](../../com.aspose.cells/istreamprovider)
### getThemeFont(int type) {#getThemeFont-int-}
```
public String getThemeFont(int type)
```


Получает название шрифта темы по умолчанию.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| type | int | [FontSchemeType](../../com.aspose.cells/fontschemetype). Тип схемы шрифта. |

**Returns:**
java.lang.String -
### getUpdateAdjacentCellsBorder() {#getUpdateAdjacentCellsBorder--}
```
public boolean getUpdateAdjacentCellsBorder()
```


Указывает, обновлять ли границу соседних ячеек.

**Remarks**

Значение по умолчанию — false. Например: если нижняя граница ячейки A1 обновлена, верхняя граница ячейки A2 также должна быть изменена.

**Returns:**
boolean
### getUpdateLinksType() {#getUpdateLinksType--}
```
public int getUpdateLinksType()
```


Получает способ обновления внешних ссылок при открытии книги.

Смотрите [UpdateLinksType](../../com.aspose.cells/updatelinkstype).

**Returns:**
int
### getWarningCallback() {#getWarningCallback--}
```
public IWarningCallback getWarningCallback()
```


Получает обратный вызов предупреждения.

**Returns:**
[IWarningCallback](../../com.aspose.cells/iwarningcallback)
### getWindowHeight() {#getWindowHeight--}
```
public double getWindowHeight()
```


Высота окна в пунктах.

**Returns:**
double
### getWindowHeightCM() {#getWindowHeightCM--}
```
public double getWindowHeightCM()
```


Высота окна в сантиметрах.

**Returns:**
double
### getWindowHeightInch() {#getWindowHeightInch--}
```
public double getWindowHeightInch()
```


Высота окна в единицах дюйма.

**Returns:**
double
### getWindowLeft() {#getWindowLeft--}
```
public double getWindowLeft()
```


Расстояние от левого края клиентской области до левого края окна в единицах пункта.

**Returns:**
double
### getWindowLeftCM() {#getWindowLeftCM--}
```
public double getWindowLeftCM()
```


Расстояние от левого края клиентской области до левого края окна. В сантиметрах.

**Returns:**
double
### getWindowLeftInch() {#getWindowLeftInch--}
```
public double getWindowLeftInch()
```


Расстояние от левого края клиентской области до левого края окна. В дюймах.

**Returns:**
double
### getWindowTop() {#getWindowTop--}
```
public double getWindowTop()
```


Расстояние от верхнего края клиентской области до верхнего края окна в единицах пункта.

**Returns:**
double
### getWindowTopCM() {#getWindowTopCM--}
```
public double getWindowTopCM()
```


Расстояние от верхнего края клиентской области до верхнего края окна в единицах сантиметра.

**Returns:**
double
### getWindowTopInch() {#getWindowTopInch--}
```
public double getWindowTopInch()
```


Расстояние от верхнего края клиентской области до верхнего края окна в единицах дюйма.

**Returns:**
double
### getWindowWidth() {#getWindowWidth--}
```
public double getWindowWidth()
```


Ширина окна в единицах пункта.

**Returns:**
double
### getWindowWidthCM() {#getWindowWidthCM--}
```
public double getWindowWidthCM()
```


Ширина окна в единицах сантиметра.

**Returns:**
double
### getWindowWidthInch() {#getWindowWidthInch--}
```
public double getWindowWidthInch()
```


Ширина окна в единицах дюйма.

**Returns:**
double
### getWpsCompatibility() {#getWpsCompatibility--}
```
public boolean getWpsCompatibility()
```


Указывает, следует ли быть совместимым с WPS.

**Returns:**
boolean
### getWriteProtection() {#getWriteProtection--}
```
public WriteProtection getWriteProtection()
```


Обеспечивает доступ к параметрам защиты записи книги.

**Returns:**
[WriteProtection](../../com.aspose.cells/writeprotection)
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isDefaultEncrypted() {#isDefaultEncrypted--}
```
public boolean isDefaultEncrypted()
```


Указывает, следует ли шифровать книгу паролем по умолчанию, если структура и окна книги заблокированы.

**Remarks**

Сейчас значение по умолчанию — false. Это то же самое, что в MS Excel 2013.

**Returns:**
boolean
### isEncrypted() {#isEncrypted--}
```
public boolean isEncrypted()
```


Получает значение, указывающее, требуется ли пароль для открытия этой книги.

**Returns:**
boolean
### isHScrollBarVisible() {#isHScrollBarVisible--}
```
public boolean isHScrollBarVisible()
```


Получает значение, указывающее, будет ли сгенерированная таблица содержать горизонтальную полосу прокрутки.

**Remarks**

Значение по умолчанию — true.

**Example**

Следующий код делает горизонтальную полосу прокрутки невидимой в электронной таблице.

```
         // Hide the horizontal scroll bar of the Excel file.
         settings.setHScrollBarVisible(false);
```

**Returns:**
boolean
### isHidden() {#isHidden--}
```
public boolean isHidden()
```


Указывает, скрыта ли эта книга.

**Returns:**
boolean
### isMinimized() {#isMinimized--}
```
public boolean isMinimized()
```


Представляет, будет ли сгенерированная таблица открыта в свернутом виде.

**Returns:**
boolean
### isProtected() {#isProtected--}
```
public boolean isProtected()
```


Получает значение, указывающее, защищены ли структура или окно книги.

**Returns:**
boolean
### isVScrollBarVisible() {#isVScrollBarVisible--}
```
public boolean isVScrollBarVisible()
```


Получает значение, указывающее, будет ли сгенерированная таблица содержать вертикальную полосу прокрутки.

**Remarks**

Значение по умолчанию — true.

**Example**

Следующий код делает вертикальную полосу прокрутки невидимой в электронной таблице.

```
         	// Hide the vertical scroll bar of the Excel file.
         settings.setVScrollBarVisible(false);
```

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




### setAuthor(String value) {#setAuthor-java.lang.String-}
```
public void setAuthor(String value)
```


Устанавливает автора файла.

**Remarks**

Не установлено, сначала проверьте [BuiltInDocumentPropertyCollection.getAuthor()](../../com.aspose.cells/builtindocumentpropertycollection\#getAuthor--), затем проверьте пользователя среды Environment.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### setAutoCompressPictures(boolean value) {#setAutoCompressPictures-boolean-}
```
public void setAutoCompressPictures(boolean value)
```


Указывает логическое значение, которое показывает, что приложение автоматически сжимает изображения в рабочей книге.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setAutoRecover(boolean value) {#setAutoRecover-boolean-}
```
public void setAutoRecover(boolean value)
```


Указывает, помечен ли файл для автоматического восстановления.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setBuildVersion(String value) {#setBuildVersion-java.lang.String-}
```
public void setBuildVersion(String value)
```


Указывает инкрементальный публичный релиз приложения.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### setCheckCompatibility(boolean value) {#setCheckCompatibility-boolean-}
```
public void setCheckCompatibility(boolean value)
```


Указывает, проверять ли совместимость с более ранними версиями при сохранении рабочей книги.

**Remarks**

Значение по умолчанию — true. Только для файлов Excel97-2003 xls или xlt.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setCheckCustomNumberFormat(boolean value) {#setCheckCustomNumberFormat-boolean-}
```
public void setCheckCustomNumberFormat(boolean value)
```


Указывает, проверять ли пользовательский числовой формат при установке Style.Custom.

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

### setCompliance(int value) {#setCompliance-int-}
```
public void setCompliance(int value)
```


Указывает версию OOXML для выходного документа. Значение по умолчанию — Ecma376\_2006.

См. [OoxmlCompliance](../../com.aspose.cells/ooxmlcompliance).

**Remarks**

Только для файлов .xlsx.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setCrashSave(boolean value) {#setCrashSave-boolean-}
```
public void setCrashSave(boolean value)
```


Указывает, сохранял ли приложение последний раз файл рабочей книги после сбоя.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setDataExtractLoad(boolean value) {#setDataExtractLoad-boolean-}
```
public void setDataExtractLoad(boolean value)
```


Указывает, открыл ли приложение последний раз рабочую книгу для восстановления данных.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setDate1904(boolean value) {#setDate1904-boolean-}
```
public void setDate1904(boolean value)
```


Устанавливает значение, указывающее, использует ли книга систему дат 1904 года.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setDefaultEncrypted(boolean value) {#setDefaultEncrypted-boolean-}
```
public void setDefaultEncrypted(boolean value)
```


Указывает, следует ли шифровать книгу паролем по умолчанию, если структура и окна книги заблокированы.

**Remarks**

Сейчас значение по умолчанию — false. Это то же самое, что в MS Excel 2013.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setDefaultImageResolution(int value) {#setDefaultImageResolution-int-}
```
public void setDefaultImageResolution(int value)
```


Устанавливает разрешение изображения по умолчанию.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setDiscardImageEditData(boolean value) {#setDiscardImageEditData-boolean-}
```
public void setDiscardImageEditData(boolean value)
```


Указывает, следует ли отбрасывать редактируемые данные изображения.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setDisplayDrawingObjects(int value) {#setDisplayDrawingObjects-int-}
```
public void setDisplayDrawingObjects(int value)
```


Указывает, показывать ли объекты в рабочей книге и как.

См. [DisplayDrawingObjects](../../com.aspose.cells/displaydrawingobjects).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setEnableMacros(boolean value) {#setEnableMacros-boolean-}
```
public void setEnableMacros(boolean value)
```


Включить макросы;

**Remarks**

Сейчас это работает только при копировании листа в другой лист в книге.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setFirstVisibleTab(int value) {#setFirstVisibleTab-int-}
```
public void setFirstVisibleTab(int value)
```


Устанавливает первую видимую вкладку листа.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setGlobalizationSettings(GlobalizationSettings value) {#setGlobalizationSettings-com.aspose.cells.GlobalizationSettings-}
```
public void setGlobalizationSettings(GlobalizationSettings value)
```


Устанавливает параметры глобализации.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| value | [GlobalizationSettings](../../com.aspose.cells/globalizationsettings) |  |

### setHScrollBarVisible(boolean value) {#setHScrollBarVisible-boolean-}
```
public void setHScrollBarVisible(boolean value)
```


Устанавливает значение, указывающее, будет ли сгенерированная таблица содержать горизонтальную полосу прокрутки.

**Remarks**

Значение по умолчанию — true.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setHidden(boolean value) {#setHidden-boolean-}
```
public void setHidden(boolean value)
```


Указывает, скрыта ли эта книга.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setHidePivotFieldList(boolean value) {#setHidePivotFieldList-boolean-}
```
public void setHidePivotFieldList(boolean value)
```


Устанавливает, скрывать ли список полей для сводной таблицы.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setLanguageCode(int value) {#setLanguageCode-int-}
```
public void setLanguageCode(int value)
```


Устанавливает язык пользовательского интерфейса версии Workbook на основе CountryCode, в которой был сохранён файл.

Смотрите [CountryCode](../../com.aspose.cells/countrycode).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setLocale(Locale value) {#setLocale-java.util.Locale-}
```
public void setLocale(Locale value)
```


Устанавливает локаль, используемую этой книгой.

**Remarks**

Возвращает null, если не установлена ни локаль, ни [getRegion()](../../com.aspose.cells/workbooksettings\#getRegion--).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.util.Locale |  |

### setMaxRowsOfSharedFormula(int value) {#setMaxRowsOfSharedFormula-int-}
```
public void setMaxRowsOfSharedFormula(int value)
```


Устанавливает максимальный номер строки общей формулы.

**Remarks**

Если число слишком велико, автофильтр работает очень медленно в MS Excel 2013.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setMaxUniqueItemsPerField(int value) {#setMaxUniqueItemsPerField-int-}
```
public void setMaxUniqueItemsPerField(int value)
```


Устанавливает ограничение уникальных элементов на поле.

**Remarks**

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setMemorySetting(int value) {#setMemorySetting-int-}
```
public void setMemorySetting(int value)
```


Устанавливает параметры использования памяти. Новый параметр будет принят в качестве параметра по умолчанию для только что созданных листов, но не будет применяться к существующим листам.

Смотрите [MemorySetting](../../com.aspose.cells/memorysetting).

**Remarks**

Для получения более подробной информации о режиме памяти, пожалуйста, смотрите [Cells.getMemorySetting()](../../com.aspose.cells/cells\#getMemorySetting--).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setMinimized(boolean value) {#setMinimized-boolean-}
```
public void setMinimized(boolean value)
```


Представляет, будет ли сгенерированная таблица открыта в свернутом виде.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setNumberDecimalSeparator(char value) {#setNumberDecimalSeparator-char-}
```
public void setNumberDecimalSeparator(char value)
```


Устанавливает десятичный разделитель для форматирования/парсинга числовых значений. По умолчанию используется десятичный разделитель текущего региона.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | char |  |

### setNumberGroupSeparator(char value) {#setNumberGroupSeparator-char-}
```
public void setNumberGroupSeparator(char value)
```


Устанавливает символ, разделяющий группы цифр слева от десятичной точки в числовых значениях. По умолчанию используется разделитель групп текущего региона.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | char |  |

### setPageOrientationType(int pageOrientationType) {#setPageOrientationType-int-}
```
public void setPageOrientationType(int pageOrientationType)
```


Устанавливает тип ориентации печати для всей книги.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| pageOrientationType | int | [PageOrientationType](../../com.aspose.cells/pageorientationtype). Тип ориентации страницы |

### setPaperSize(int value) {#setPaperSize-int-}
```
public void setPaperSize(int value)
```


Устанавливает размер бумаги по умолчанию для печати.

Смотрите [PaperSizeType](../../com.aspose.cells/papersizetype).

**Remarks**

Если настройка размера бумаги отсутствует, MS Excel будет использовать настройки принтера по умолчанию.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setPassword(String value) {#setPassword-java.lang.String-}
```
public void setPassword(String value)
```


Представляет пароль шифрования файла Workbook.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### setPropertiesFollowChartPoint(boolean value) {#setPropertiesFollowChartPoint-boolean-}
```
public void setPropertiesFollowChartPoint(boolean value)
```


Указывает, следуют ли свойства точек данных и подписи данных во всех диаграммах этой книги их ссылке.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setQuotePrefixToStyle(boolean value) {#setQuotePrefixToStyle-boolean-}
```
public void setQuotePrefixToStyle(boolean value)
```


Указывает, применяется ли свойство [Style.getQuotePrefix()](../../com.aspose.cells/style\#getQuotePrefix--) при вводе строкового значения (которое начинается с одинарной кавычки) в ячейку

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setRegion(int value) {#setRegion-int-}
```
public void setRegion(int value)
```


Устанавливает региональные настройки для книги.

Смотрите [CountryCode](../../com.aspose.cells/countrycode).

**Remarks**

1. Региональные настройки, используемые компонентом Aspose.Cells для книги, загруженной из шаблонного файла: i). Для файла XLS определены поля для региональных настроек, и MS Excel сохраняет данные региональных настроек в файл при сохранении XLS. Поэтому мы используем сохранённый регион из шаблонного файла для книги. Если вы не хотите использовать регион, сохранённый в файле XLS, пожалуйста, сбросьте его на требуемый (например, CountryCode.Default) после загрузки шаблонного файла. И мы также сохраняем пользовательское значение (с помощью этого метода) в файл при сохранении XLS. ii). Для других форматов файлов, таких как XLSX, XLSB и т.д., в спецификации формата нет поля для региональных настроек. Поэтому мы используем региональные настройки среды приложения для книги. И пользовательское значение (с помощью этого метода) не может быть сохранено в генерируемых файлах этих форматов. 2. Для отображения в MS Excel: применённые здесь региональные настройки могут действовать только во время выполнения с компонентом Aspose.Cells и не влияют при просмотре сгенерированного файла в MS Excel. Даже для сгенерированного XLS‑файла, в котором данные региональных настроек сохранены, при просмотре/редактировании его в MS Excel регион, используемый для форматирования, всегда является региональными настройками по умолчанию среды, где запущен MS Excel, а не тем, что сохранён в файле. Это поведение MS Excel и его нельзя изменить кодом.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setRemovePersonalInformation(boolean value) {#setRemovePersonalInformation-boolean-}
```
public void setRemovePersonalInformation(boolean value)
```


Истина, если личную информацию можно удалить из указанной книги.

**Remarks**

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setRepairLoad(boolean value) {#setRepairLoad-boolean-}
```
public void setRepairLoad(boolean value)
```


Указывает, открыла ли приложение книгу в безопасном или режиме восстановления в последний раз.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setResourceProvider(IStreamProvider value) {#setResourceProvider-com.aspose.cells.IStreamProvider-}
```
public void setResourceProvider(IStreamProvider value)
```


Устанавливает поставщика потоков для внешних ресурсов, например загрузку данных изображения для картинки типа "LinkToFile".

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| value | [IStreamProvider](../../com.aspose.cells/istreamprovider) |  |

### setShapeDisplayType(int value) {#setShapeDisplayType-int-}
```
public void setShapeDisplayType(int value)
```


Устанавливает, как приложение отображает фигуры в этой книге.

Смотрите [ShapeDisplayType](../../com.aspose.cells/shapedisplaytype).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setShared(boolean value) {#setShared-boolean-}
```
public void setShared(boolean value)
```


Устанавливает значение, указывающее, является ли книга общей.

**Remarks**

Значение по умолчанию — false.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setSheetTabBarWidth(int value) {#setSheetTabBarWidth-int-}
```
public void setSheetTabBarWidth(int value)
```


Ширина панели вкладок листов (в 1/1000 ширины окна).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setShowTabs(boolean value) {#setShowTabs-boolean-}
```
public void setShowTabs(boolean value)
```


Устанавливает значение, отображаются ли вкладки книги.

**Remarks**

Значение по умолчанию — true.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setSignificantDigits(int value) {#setSignificantDigits-int-}
```
public void setSignificantDigits(int value)
```


Устанавливает количество значимых цифр. Значение по умолчанию — [CellsHelper.getSignificantDigits()](../../com.aspose.cells/cellshelper\#getSignificantDigits--).

**Remarks**

Сейчас может быть только 15 или 17. ПРИМЕЧАНИЕ: Этот член теперь устарел. Вместо него используйте [getSignificantDigitsType()](../../com.aspose.cells/workbooksettings\#getSignificantDigitsType--). Это свойство будет удалено через 12 месяцев, начиная с июня 2025 года. Компания Aspose просит прощения за любые причинённые неудобства.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setSignificantDigitsType(int value) {#setSignificantDigitsType-int-}
```
public void setSignificantDigitsType(int value)
```


Устанавливает тип значимых цифр для вывода числовых значений в этой рабочей книге. Значение по умолчанию — [CellsHelper.getSignificantDigitsType()](../../com.aspose.cells/cellshelper\#getSignificantDigitsType--).

Смотрите [SignificantDigitsType](../../com.aspose.cells/significantdigitstype).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setStreamProvider(IStreamProvider value) {#setStreamProvider-com.aspose.cells.IStreamProvider-}
```
public void setStreamProvider(IStreamProvider value)
```


Устанавливает поставщика потоков для внешнего ресурса.

**Remarks**

ПРИМЕЧАНИЕ: Этот член теперь устарел. Вместо него используйте свойство ResourceProvider. Это свойство будет удалено через 12 месяцев, начиная с июня 2022 года. Компания Aspose просит прощения за любые причинённые неудобства.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| value | [IStreamProvider](../../com.aspose.cells/istreamprovider) |  |

### setUpdateAdjacentCellsBorder(boolean value) {#setUpdateAdjacentCellsBorder-boolean-}
```
public void setUpdateAdjacentCellsBorder(boolean value)
```


Указывает, обновлять ли границу соседних ячеек.

**Remarks**

Значение по умолчанию — false. Например: если нижняя граница ячейки A1 обновлена, верхняя граница ячейки A2 также должна быть изменена.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setUpdateLinksType(int value) {#setUpdateLinksType-int-}
```
public void setUpdateLinksType(int value)
```


Устанавливает, как обновлять внешние ссылки при открытии книги.

Смотрите [UpdateLinksType](../../com.aspose.cells/updatelinkstype).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setVScrollBarVisible(boolean value) {#setVScrollBarVisible-boolean-}
```
public void setVScrollBarVisible(boolean value)
```


Устанавливает значение, указывающее, будет ли сгенерированная таблица содержать вертикальную полосу прокрутки.

**Remarks**

Значение по умолчанию — true.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setWarningCallback(IWarningCallback value) {#setWarningCallback-com.aspose.cells.IWarningCallback-}
```
public void setWarningCallback(IWarningCallback value)
```


Устанавливает обратный вызов предупреждения.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| value | [IWarningCallback](../../com.aspose.cells/iwarningcallback) |  |

### setWindowHeight(double value) {#setWindowHeight-double-}
```
public void setWindowHeight(double value)
```


Высота окна в пунктах.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | double |  |

### setWindowHeightCM(double value) {#setWindowHeightCM-double-}
```
public void setWindowHeightCM(double value)
```


Высота окна в сантиметрах.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | double |  |

### setWindowHeightInch(double value) {#setWindowHeightInch-double-}
```
public void setWindowHeightInch(double value)
```


Высота окна в единицах дюйма.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | double |  |

### setWindowLeft(double value) {#setWindowLeft-double-}
```
public void setWindowLeft(double value)
```


Расстояние от левого края клиентской области до левого края окна в единицах пункта.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | double |  |

### setWindowLeftCM(double value) {#setWindowLeftCM-double-}
```
public void setWindowLeftCM(double value)
```


Расстояние от левого края клиентской области до левого края окна. В сантиметрах.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | double |  |

### setWindowLeftInch(double value) {#setWindowLeftInch-double-}
```
public void setWindowLeftInch(double value)
```


Расстояние от левого края клиентской области до левого края окна. В дюймах.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | double |  |

### setWindowTop(double value) {#setWindowTop-double-}
```
public void setWindowTop(double value)
```


Расстояние от верхнего края клиентской области до верхнего края окна в единицах пункта.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | double |  |

### setWindowTopCM(double value) {#setWindowTopCM-double-}
```
public void setWindowTopCM(double value)
```


Расстояние от верхнего края клиентской области до верхнего края окна в единицах сантиметра.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | double |  |

### setWindowTopInch(double value) {#setWindowTopInch-double-}
```
public void setWindowTopInch(double value)
```


Расстояние от верхнего края клиентской области до верхнего края окна в единицах дюйма.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | double |  |

### setWindowWidth(double value) {#setWindowWidth-double-}
```
public void setWindowWidth(double value)
```


Ширина окна в единицах пункта.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | double |  |

### setWindowWidthCM(double value) {#setWindowWidthCM-double-}
```
public void setWindowWidthCM(double value)
```


Ширина окна в единицах сантиметра.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | double |  |

### setWindowWidthInch(double value) {#setWindowWidthInch-double-}
```
public void setWindowWidthInch(double value)
```


Ширина окна в единицах дюйма.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | double |  |

### setWpsCompatibility(boolean value) {#setWpsCompatibility-boolean-}
```
public void setWpsCompatibility(boolean value)
```


Указывает, следует ли быть совместимым с WPS.

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

