---
title: "PdfSaveOptions"
second_title: "Справочник API Aspose.Cells for Java"
description: "Представляет параметры сохранения PDF‑файла."
type: docs
url: /ru/java/com.aspose.cells/pdfsaveoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.SaveOptions](../../com.aspose.cells/saveoptions), [com.aspose.cells.PaginatedSaveOptions](../../com.aspose.cells/paginatedsaveoptions)
```
public class PdfSaveOptions extends PaginatedSaveOptions
```

Представляет параметры сохранения PDF‑файла.
## Конструкторы

| Конструктор | Описание |
| --- | --- |
| [PdfSaveOptions()](#PdfSaveOptions--) | Создаёт параметры для сохранения PDF‑файла. |
## Методы

| Метод | Описание |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAllColumnsInOnePagePerSheet()](#getAllColumnsInOnePagePerSheet--) | Если AllColumnsInOnePagePerSheet равно true, всё содержимое столбцов одного листа будет выводиться только на одну страницу в результате. |
| [getBookmark()](#getBookmark--) | Получает объект [PdfBookmarkEntry](../../com.aspose.cells/pdfbookmarkentry). |
| [getCachedFileFolder()](#getCachedFileFolder--) | Папка для временных файлов, которые могут использоваться в качестве кэша данных. |
| [getCalculateFormula()](#getCalculateFormula--) | Указывает, следует ли вычислять формулы перед сохранением PDF‑файла. |
| [getCheckExcelRestriction()](#getCheckExcelRestriction--) | Проверять ли ограничения Excel‑файла, когда пользователь изменяет связанные с ячейками объекты. |
| [getCheckFontCompatibility()](#getCheckFontCompatibility--) | Указывает, следует ли проверять совместимость шрифтов для каждого символа в тексте. |
| [getCheckWorkbookDefaultFont()](#getCheckWorkbookDefaultFont--) | Когда символы в Excel являются Unicode и в стиле ячейки не установлен правильный шрифт, они могут отображаться как блоки в pdf,image. |
| [getClass()](#getClass--) |  |
| [getClearData()](#getClearData--) | Очищать книгу после сохранения файла. |
| [getCompliance()](#getCompliance--) | Получает уровень соответствия стандартам PDF для выходных документов. |
| [getCreateDirectory()](#getCreateDirectory--) | Если true и каталог не существует, каталог будет автоматически создан перед сохранением файла. |
| [getCreatedTime()](#getCreatedTime--) | Получает время создания PDF‑документа. |
| [getCustomPropertiesExport()](#getCustomPropertiesExport--) | Получает значение, определяющее способ экспорта [CustomDocumentPropertyCollection](../../com.aspose.cells/customdocumentpropertycollection) в PDF‑файл. |
| [getCustomRenderSettings()](#getCustomRenderSettings--) | Получает пользовательские настройки во время рендеринга. |
| [getDefaultEditLanguage()](#getDefaultEditLanguage--) | Получает язык редактирования по умолчанию. |
| [getDefaultFont()](#getDefaultFont--) | Когда символы в Excel являются Unicode и в стиле ячейки не установлен правильный шрифт, они могут отображаться как блоки в pdf,image. |
| [getDisplayDocTitle()](#getDisplayDocTitle--) | Указывает, следует ли отображать заголовок документа в строке заголовка окна. |
| [getDrawObjectEventHandler()](#getDrawObjectEventHandler--) | Реализует этот интерфейс для получения DrawObject и Bound при рендеринге. |
| [getEmbedAttachments()](#getEmbedAttachments--) | Указывает, следует ли встраивать вложения для объектов OLE в Excel. |
| [getEmbedStandardWindowsFonts()](#getEmbedStandardWindowsFonts--) | True, чтобы встраивать шрифты TrueType. |
| [getEmfRenderSetting()](#getEmfRenderSetting--) | Настройка рендеринга метафайла Emf. |
| [getEncryptDocumentProperties()](#getEncryptDocumentProperties--) | Указывает, следует ли шифровать свойства документа при сохранении в формате .xls. |
| [getExportDocumentStructure()](#getExportDocumentStructure--) | Указывает, следует ли экспортировать структуру документа. |
| [getFontEncoding()](#getFontEncoding--) | Получает кодировку встроенных шрифтов в PDF. |
| [getGridlineColor()](#getGridlineColor--) | Получает цвет линий сетки. |
| [getGridlineType()](#getGridlineType--) | Получает тип линий сетки. |
| [getIgnoreError()](#getIgnoreError--) | Указывает, нужно ли скрывать ошибку во время рендеринга. |
| [getImageType()](#getImageType--) | Представляет тип изображения при преобразовании диаграммы и фигуры. |
| [getMergeAreas()](#getMergeAreas--) | Указывает, следует ли объединять области условного форматирования и проверки перед сохранением файла. |
| [getOnePagePerSheet()](#getOnePagePerSheet--) | Если OnePagePerSheet равно true, всё содержимое одного листа будет выводиться только на одну страницу в результате. |
| [getOptimizationType()](#getOptimizationType--) | Получает тип оптимизации PDF. |
| [getOutputBlankPageWhenNothingToPrint()](#getOutputBlankPageWhenNothingToPrint--) | Указывает, следует ли выводить пустую страницу, когда нечего печатать. |
| [getPageCount()](#getPageCount--) | Получает количество страниц для сохранения. |
| [getPageIndex()](#getPageIndex--) | Получает индекс первой страницы для сохранения, начиная с 0. |
| [getPageSavingCallback()](#getPageSavingCallback--) | Контролировать/Указывать прогресс процесса сохранения страниц. |
| [getPdfCompression()](#getPdfCompression--) | Указывает алгоритм сжатия |
| [getPrintingPageType()](#getPrintingPageType--) | Указывает, какие страницы не будут печататься. |
| [getProducer()](#getProducer--) | Получает производителя сгенерированного PDF‑документа. |
| [getRefreshChartCache()](#getRefreshChartCache--) | Указывает, кэшировать ли последние данные диаграммы. |
| [getRenderingBehavior()](#getRenderingBehavior--) | Получает специфические для Excel поведения рендеринга, которые следует применить. |
| [getSaveFormat()](#getSaveFormat--) | Получает формат сохраняемого файла. |
| [getSecurityOptions()](#getSecurityOptions--) | Установите эти параметры, когда в результате xls2pdf требуется безопасность. |
| [getSheetSet()](#getSheetSet--) | Получает листы для рендеринга. |
| [getSortExternalNames()](#getSortExternalNames--) | Указывает, сортировать ли внешние определённые имена перед сохранением файла. |
| [getSortNames()](#getSortNames--) | Указывает, сортировать ли определённые имена перед сохранением файла. |
| [getTextCrossType()](#getTextCrossType--) | Получает тип отображаемого текста, когда ширина текста превышает ширину ячейки. |
| [getUpdateSmartArt()](#getUpdateSmartArt--) | Указывает, обновлять ли настройки SmartArt. |
| [getValidateMergedAreas()](#getValidateMergedAreas--) | Указывает, проверять ли объединённые ячейки перед сохранением файла. |
| [getWarningCallback()](#getWarningCallback--) | Получает обратный вызов предупреждения. |
| [getWatermark()](#getWatermark--) | Получает водяной знак для вывода. |
| [getZoomBehavior()](#getZoomBehavior--) | Получает режим начального просмотра при открытии сгенерированного PDF‑документа. |
| [getZoomFactor()](#getZoomFactor--) | Получает процент масштабирования, используемый, когда [getZoomBehavior()](../../com.aspose.cells/pdfsaveoptions\#getZoomBehavior--) является [PdfZoomBehavior.ZOOM\_FACTOR](../../com.aspose.cells/pdfzoombehavior\#ZOOM-FACTOR). |
| [hashCode()](#hashCode--) |  |
| [isFontSubstitutionCharGranularity()](#isFontSubstitutionCharGranularity--) | Указывает, следует ли заменять шрифт символа только в случае, когда шрифт ячейки не совместим с ним. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAllColumnsInOnePagePerSheet(boolean value)](#setAllColumnsInOnePagePerSheet-boolean-) | Если AllColumnsInOnePagePerSheet равно true, всё содержимое столбцов одного листа будет выводиться только на одну страницу в результате. |
| [setBookmark(PdfBookmarkEntry value)](#setBookmark-com.aspose.cells.PdfBookmarkEntry-) | Устанавливает объект [PdfBookmarkEntry](../../com.aspose.cells/pdfbookmarkentry). |
| [setCachedFileFolder(String value)](#setCachedFileFolder-java.lang.String-) | Папка для временных файлов, которые могут использоваться в качестве кэша данных. |
| [setCalculateFormula(boolean value)](#setCalculateFormula-boolean-) | Указывает, следует ли вычислять формулы перед сохранением PDF‑файла. |
| [setCheckExcelRestriction(boolean value)](#setCheckExcelRestriction-boolean-) | Проверять ли ограничения Excel‑файла, когда пользователь изменяет связанные с ячейками объекты. |
| [setCheckFontCompatibility(boolean value)](#setCheckFontCompatibility-boolean-) | Указывает, следует ли проверять совместимость шрифтов для каждого символа в тексте. |
| [setCheckWorkbookDefaultFont(boolean value)](#setCheckWorkbookDefaultFont-boolean-) | Когда символы в Excel являются Unicode и в стиле ячейки не установлен правильный шрифт, они могут отображаться как блоки в pdf,image. |
| [setClearData(boolean value)](#setClearData-boolean-) | Очищать книгу после сохранения файла. |
| [setCompliance(int value)](#setCompliance-int-) | Устанавливает уровень соответствия стандартам PDF для выходных документов. |
| [setCreateDirectory(boolean value)](#setCreateDirectory-boolean-) | Если true и каталог не существует, каталог будет автоматически создан перед сохранением файла. |
| [setCreatedTime(DateTime value)](#setCreatedTime-com.aspose.cells.DateTime-) | Устанавливает время создания PDF‑документа. |
| [setCustomPropertiesExport(int value)](#setCustomPropertiesExport-int-) | Устанавливает значение, определяющее способ экспорта [CustomDocumentPropertyCollection](../../com.aspose.cells/customdocumentpropertycollection) в PDF‑файл. |
| [setCustomRenderSettings(CustomRenderSettings value)](#setCustomRenderSettings-com.aspose.cells.CustomRenderSettings-) | Устанавливает пользовательские параметры во время рендеринга. |
| [setDefaultEditLanguage(int value)](#setDefaultEditLanguage-int-) | Устанавливает язык редактирования по умолчанию. |
| [setDefaultFont(String value)](#setDefaultFont-java.lang.String-) | Когда символы в Excel являются Unicode и в стиле ячейки не установлен правильный шрифт, они могут отображаться как блоки в pdf,image. |
| [setDisplayDocTitle(boolean value)](#setDisplayDocTitle-boolean-) | Указывает, следует ли отображать заголовок документа в строке заголовка окна. |
| [setDrawObjectEventHandler(DrawObjectEventHandler value)](#setDrawObjectEventHandler-com.aspose.cells.DrawObjectEventHandler-) | Реализует этот интерфейс для получения DrawObject и Bound при рендеринге. |
| [setEmbedAttachments(boolean value)](#setEmbedAttachments-boolean-) | Указывает, следует ли встраивать вложения для объектов OLE в Excel. |
| [setEmbedStandardWindowsFonts(boolean value)](#setEmbedStandardWindowsFonts-boolean-) | True, чтобы встраивать шрифты TrueType. |
| [setEmfRenderSetting(int value)](#setEmfRenderSetting-int-) | Настройка рендеринга метафайла Emf. |
| [setEncryptDocumentProperties(boolean value)](#setEncryptDocumentProperties-boolean-) | Указывает, следует ли шифровать свойства документа при сохранении в формате .xls. |
| [setExportDocumentStructure(boolean value)](#setExportDocumentStructure-boolean-) | Указывает, следует ли экспортировать структуру документа. |
| [setFontEncoding(int value)](#setFontEncoding-int-) | Устанавливает кодировку встроенных шрифтов в PDF. |
| [setFontSubstitutionCharGranularity(boolean value)](#setFontSubstitutionCharGranularity-boolean-) | Указывает, следует ли заменять шрифт символа только в случае, когда шрифт ячейки не совместим с ним. |
| [setGridlineColor(Color value)](#setGridlineColor-com.aspose.cells.Color-) | Устанавливает цвет линий сетки. |
| [setGridlineType(int value)](#setGridlineType-int-) | Устанавливает тип линий сетки. |
| [setIgnoreError(boolean value)](#setIgnoreError-boolean-) | Указывает, нужно ли скрывать ошибку во время рендеринга. |
| [setImageResample(int desiredPPI, int jpegQuality)](#setImageResample-int-int-) | Устанавливает требуемое PPI (pixels per inch) для пересэмплирования изображений и качество JPEG. |
| [setImageType(ImageFormat value)](#setImageType-com.aspose.cells.ImageFormat-) | Представляет тип изображения при преобразовании диаграммы и фигуры. |
| [setMergeAreas(boolean value)](#setMergeAreas-boolean-) | Указывает, следует ли объединять области условного форматирования и проверки перед сохранением файла. |
| [setOnePagePerSheet(boolean value)](#setOnePagePerSheet-boolean-) | Если OnePagePerSheet равно true, всё содержимое одного листа будет выводиться только на одну страницу в результате. |
| [setOptimizationType(int value)](#setOptimizationType-int-) | Устанавливает тип оптимизации PDF. |
| [setOutputBlankPageWhenNothingToPrint(boolean value)](#setOutputBlankPageWhenNothingToPrint-boolean-) | Указывает, следует ли выводить пустую страницу, когда нечего печатать. |
| [setPageCount(int value)](#setPageCount-int-) | Устанавливает количество страниц для сохранения. |
| [setPageIndex(int value)](#setPageIndex-int-) | Устанавливает нулевой индекс первой страницы для сохранения. |
| [setPageSavingCallback(IPageSavingCallback value)](#setPageSavingCallback-com.aspose.cells.IPageSavingCallback-) | Контролировать/Указывать прогресс процесса сохранения страниц. |
| [setPdfCompression(int value)](#setPdfCompression-int-) | Указывает алгоритм сжатия |
| [setPrintingPageType(int value)](#setPrintingPageType-int-) | Указывает, какие страницы не будут печататься. |
| [setProducer(String value)](#setProducer-java.lang.String-) | Устанавливает производителя сгенерированного PDF‑документа. |
| [setRefreshChartCache(boolean value)](#setRefreshChartCache-boolean-) | Указывает, кэшировать ли последние данные диаграммы. |
| [setRenderingBehavior(int value)](#setRenderingBehavior-int-) | Устанавливает специфические для Excel поведения рендеринга, которые следует применить. |
| [setSecurityOptions(PdfSecurityOptions value)](#setSecurityOptions-com.aspose.cells.PdfSecurityOptions-) | Установите эти параметры, когда в результате xls2pdf требуется безопасность. |
| [setSheetSet(SheetSet value)](#setSheetSet-com.aspose.cells.SheetSet-) | Устанавливает листы для рендеринга. |
| [setSortExternalNames(boolean value)](#setSortExternalNames-boolean-) | Указывает, сортировать ли внешние определённые имена перед сохранением файла. |
| [setSortNames(boolean value)](#setSortNames-boolean-) | Указывает, сортировать ли определённые имена перед сохранением файла. |
| [setTextCrossType(int value)](#setTextCrossType-int-) | Устанавливает тип отображаемого текста, когда ширина текста превышает ширину ячейки. |
| [setUpdateSmartArt(boolean value)](#setUpdateSmartArt-boolean-) | Указывает, обновлять ли настройки SmartArt. |
| [setValidateMergedAreas(boolean value)](#setValidateMergedAreas-boolean-) | Указывает, проверять ли объединённые ячейки перед сохранением файла. |
| [setWarningCallback(IWarningCallback value)](#setWarningCallback-com.aspose.cells.IWarningCallback-) | Устанавливает обратный вызов предупреждения. |
| [setWatermark(RenderingWatermark value)](#setWatermark-com.aspose.cells.RenderingWatermark-) | Устанавливает водяной знак в вывод. |
| [setZoomBehavior(int value)](#setZoomBehavior-int-) | Устанавливает начальный режим просмотра при открытии сгенерированного PDF‑документа. |
| [setZoomFactor(int value)](#setZoomFactor-int-) | Устанавливает процент масштабирования, используемый, когда [getZoomBehavior()](../../com.aspose.cells/pdfsaveoptions\\#getZoomBehavior--) равен [PdfZoomBehavior.ZOOM\\_FACTOR](../../com.aspose.cells/pdfzoombehavior\\#ZOOM-FACTOR). |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### PdfSaveOptions() {#PdfSaveOptions--}
```
public PdfSaveOptions()
```


Создаёт параметры для сохранения PDF‑файла.

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
### getAllColumnsInOnePagePerSheet() {#getAllColumnsInOnePagePerSheet--}
```
public boolean getAllColumnsInOnePagePerSheet()
```


Если AllColumnsInOnePagePerSheet установлено в true, всё содержимое столбцов одного листа будет выводиться на одну страницу в результате. Ширина бумажного формата из pagesetup будет игнорироваться, а остальные настройки pagesetup сохранят своё действие.

**Returns:**
boolean
### getBookmark() {#getBookmark--}
```
public PdfBookmarkEntry getBookmark()
```


Получает объект [PdfBookmarkEntry](../../com.aspose.cells/pdfbookmarkentry).

**Returns:**
[PdfBookmarkEntry](../../com.aspose.cells/pdfbookmarkentry)
### getCachedFileFolder() {#getCachedFileFolder--}
```
public String getCachedFileFolder()
```


Папка для временных файлов, которые могут использоваться в качестве кэша данных.

**Remarks**

Если папка не указана, значение по умолчанию для неё — [CellsHelper.getCacheFolder()](../../com.aspose.cells/cellshelper\#getCacheFolder--). Если её значение по умолчанию равно null или пусто, либо указано как null или пусто, то при сохранении книги кэш‑файл использоваться не будет.

**Returns:**
java.lang.String
### getCalculateFormula() {#getCalculateFormula--}
```
public boolean getCalculateFormula()
```


Указывает, следует ли вычислять формулы перед сохранением PDF‑файла.

**Remarks**

Значение по умолчанию — false.

**Returns:**
boolean
### getCheckExcelRestriction() {#getCheckExcelRestriction--}
```
public boolean getCheckExcelRestriction()
```


Проверять ли ограничения файла Excel, когда пользователь изменяет связанные с ячейками объекты. Например, Excel не позволяет вводить строковое значение длиной более 32K. Когда вы вводите значение длиннее 32K, оно будет усечено.

**Returns:**
boolean
### getCheckFontCompatibility() {#getCheckFontCompatibility--}
```
public boolean getCheckFontCompatibility()
```


Указывает, следует ли проверять совместимость шрифтов для каждого символа в тексте.

**Remarks**

Значение по умолчанию — true. Отключение этого свойства может повысить производительность. Однако, если шрифт по умолчанию или указанный шрифт текста/символа нельзя использовать для рендеринга, в сгенерированном PDF могут появиться нечитаемые символы (например, блоки). В такой ситуации пользователю следует оставить это свойство включённым (true), чтобы был найден и использован альтернативный шрифт для рендеринга текста.

**Returns:**
boolean
### getCheckWorkbookDefaultFont() {#getCheckWorkbookDefaultFont--}
```
public boolean getCheckWorkbookDefaultFont()
```


Если символы в Excel являются Unicode и в стиле ячейки не установлен правильный шрифт, они могут отображаться как блоки в PDF или изображении. Установите значение true, чтобы попытаться использовать шрифт по умолчанию книги для отображения этих символов.

**Remarks**

По умолчанию — true.

**Returns:**
boolean
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getClearData() {#getClearData--}
```
public boolean getClearData()
```


Очищать книгу после сохранения файла.

**Returns:**
boolean
### getCompliance() {#getCompliance--}
```
public int getCompliance()
```


Получает уровень соответствия стандартам PDF для выходных документов.

См. [PdfCompliance](../../com.aspose.cells/pdfcompliance).

**Remarks**

По умолчанию — Pdf17.

**Returns:**
int
### getCreateDirectory() {#getCreateDirectory--}
```
public boolean getCreateDirectory()
```


Если true и каталог не существует, каталог будет автоматически создан перед сохранением файла.

**Remarks**

Значение по умолчанию — false.

**Returns:**
boolean
### getCreatedTime() {#getCreatedTime--}
```
public DateTime getCreatedTime()
```


Получает время создания PDF‑документа.

**Remarks**

Если не установлено, будет использовано время создания PDF.

**Returns:**
[DateTime](../../com.aspose.cells/datetime)
### getCustomPropertiesExport() {#getCustomPropertiesExport--}
```
public int getCustomPropertiesExport()
```


Получает значение, определяющее способ экспорта [CustomDocumentPropertyCollection](../../com.aspose.cells/customdocumentpropertycollection) в PDF‑файл. Значение по умолчанию — None.

См. [PdfCustomPropertiesExport](../../com.aspose.cells/pdfcustompropertiesexport).

**Returns:**
int
### getCustomRenderSettings() {#getCustomRenderSettings--}
```
public CustomRenderSettings getCustomRenderSettings()
```


Получает пользовательские настройки во время рендеринга.

**Returns:**
[CustomRenderSettings](../../com.aspose.cells/customrendersettings)
### getDefaultEditLanguage() {#getDefaultEditLanguage--}
```
public int getDefaultEditLanguage()
```


Получает язык редактирования по умолчанию.

См. [DefaultEditLanguage](../../com.aspose.cells/defaulteditlanguage).

**Remarks**

Это может отображать/рендерить разные макеты абзацев текста при установленном различном языке редактирования. По умолчанию — [DefaultEditLanguage.AUTO](../../com.aspose.cells/defaulteditlanguage\#AUTO).

**Returns:**
int
### getDefaultFont() {#getDefaultFont--}
```
public String getDefaultFont()
```


Если символы в Excel являются Unicode и в стиле ячейки не установлен правильный шрифт, они могут отображаться как блоки в PDF или изображении. Установите DefaultFont, например MingLiu или MS Gothic, чтобы отобразить эти символы. Если это свойство не задано, Aspose.Cells будет использовать системный шрифт по умолчанию для отображения этих Unicode‑символов.

**Returns:**
java.lang.String
### getDisplayDocTitle() {#getDisplayDocTitle--}
```
public boolean getDisplayDocTitle()
```


Указывает, следует ли отображать заголовок документа в строке заголовка окна.

**Remarks**

Если false, строка заголовка будет отображать имя PDF‑файла. Значение по умолчанию — false.

**Returns:**
boolean
### getDrawObjectEventHandler() {#getDrawObjectEventHandler--}
```
public DrawObjectEventHandler getDrawObjectEventHandler()
```


Реализует этот интерфейс для получения DrawObject и Bound при рендеринге.

**Returns:**
[DrawObjectEventHandler](../../com.aspose.cells/drawobjecteventhandler)
### getEmbedAttachments() {#getEmbedAttachments--}
```
public boolean getEmbedAttachments()
```


Указывает, следует ли встраивать вложения для объектов OLE в Excel.

**Remarks**

Значение по умолчанию — false. Значение должно быть false, когда включена совместимость PDF/A или включено шифрование PDF.

**Returns:**
boolean
### getEmbedStandardWindowsFonts() {#getEmbedStandardWindowsFonts--}
```
public boolean getEmbedStandardWindowsFonts()
```


True — встраивать шрифты TrueType. Это влияет только на символы ASCII 32‑127. Шрифты для кодов символов выше 127 всегда встраиваются. Шрифты всегда встраиваются для стандарта PDF/A‑1a, PDF/A‑1b. По умолчанию — true.

**Returns:**
boolean
### getEmfRenderSetting() {#getEmfRenderSetting--}
```
public int getEmfRenderSetting()
```


Настройка рендеринга метафайла Emf.

См. [EmfRenderSetting](../../com.aspose.cells/emfrendersetting).

**Remarks**

Метaфайлы EMF, идентифицированные как "EMF+ Dual", могут содержать как записи EMF+, так и записи EMF. Любой тип записей может использоваться для рендеринга изображения, только записи EMF+, или только записи EMF. Когда установлен [EmfRenderSetting.EMF\_PLUS\_PREFER](../../com.aspose.cells/emfrendersetting\#EMF-PLUS-PREFER), записи EMF+ будут обрабатываться при рендеринге страницы, в противном случае будут обрабатываться только записи EMF. Значение по умолчанию — [EmfRenderSetting.EMF\_ONLY](../../com.aspose.cells/emfrendersetting\#EMF-ONLY).

**Returns:**
int
### getEncryptDocumentProperties() {#getEncryptDocumentProperties--}
```
public boolean getEncryptDocumentProperties()
```


Указывает, следует ли шифровать свойства документа при сохранении в файл .xls. Значение по умолчанию — true.

**Remarks**

Только для файлов .xls, .xlsx, .xlsb и .xlsm.

**Returns:**
boolean
### getExportDocumentStructure() {#getExportDocumentStructure--}
```
public boolean getExportDocumentStructure()
```


Указывает, следует ли экспортировать структуру документа.

**Returns:**
boolean
### getFontEncoding() {#getFontEncoding--}
```
public int getFontEncoding()
```


Получает кодировку встроенных шрифтов в PDF.

См. [PdfFontEncoding](../../com.aspose.cells/pdffontencoding).

**Remarks**

Значение по умолчанию — [PdfFontEncoding.IDENTITY](../../com.aspose.cells/pdffontencoding\\#IDENTITY)

**Returns:**
int
### getGridlineColor() {#getGridlineColor--}
```
public Color getGridlineColor()
```


Получает цвет линий сетки.

**Remarks**

Он будет игнорировать настройки цвета линий сетки в исходном файле.

**Returns:**
[Color](../../com.aspose.cells/color)
### getGridlineType() {#getGridlineType--}
```
public int getGridlineType()
```


Получает тип линий сетки.

См. [GridlineType](../../com.aspose.cells/gridlinetype).

**Remarks**

По умолчанию — тип Dotted.

**Returns:**
int
### getIgnoreError() {#getIgnoreError--}
```
public boolean getIgnoreError()
```


Указывает, нужно ли скрывать ошибку во время рендеринга. Ошибка может быть связана с формой, изображением, рендерингом диаграммы и т.д.

**Returns:**
boolean
### getImageType() {#getImageType--}
```
public ImageFormat getImageType()
```


Представляет тип изображения при преобразовании диаграммы и фигуры.

**Remarks**

NOTE: Этот член теперь устарел. Вместо этого Chart и Shape всегда рендерятся как векторные элементы (например, точка, линия) для обеспечения качества рендеринга. Это свойство будет удалено через 12 месяцев, начиная с июня 2022 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

**Returns:**
[ImageFormat](../../com.aspose.cells/imageformat)
### getMergeAreas() {#getMergeAreas--}
```
public boolean getMergeAreas()
```


Указывает, следует ли объединять области условного форматирования и проверки перед сохранением файла.

**Remarks**

Значение по умолчанию — false.

**Returns:**
boolean
### getOnePagePerSheet() {#getOnePagePerSheet--}
```
public boolean getOnePagePerSheet()
```


Если OnePagePerSheet равно true, всё содержимое одного листа будет выводиться только на одну страницу в результате. Размер бумаги в pagesetup будет недействительным, а остальные настройки pagesetup по‑прежнему будут применяться.

**Returns:**
boolean
### getOptimizationType() {#getOptimizationType--}
```
public int getOptimizationType()
```


Получает тип оптимизации PDF.

См. [PdfOptimizationType](../../com.aspose.cells/pdfoptimizationtype).

**Remarks**

Значение по умолчанию — [PdfOptimizationType.STANDARD](../../com.aspose.cells/pdfoptimizationtype\\#STANDARD)

**Returns:**
int
### getOutputBlankPageWhenNothingToPrint() {#getOutputBlankPageWhenNothingToPrint--}
```
public boolean getOutputBlankPageWhenNothingToPrint()
```


Указывает, следует ли выводить пустую страницу, когда нечего печатать.

**Remarks**

По умолчанию — true.

**Returns:**
boolean
### getPageCount() {#getPageCount--}
```
public int getPageCount()
```


Получает количество страниц для сохранения.

**Remarks**

По умолчанию это System.Int32.MaxValue, что означает, что все страницы будут отрисованы.

**Example**

В следующем примере показано, как отрисовать диапазон страниц (3 и 4) в файле Microsoft Excel в PDF.

```
         //Open an Excel file
         Workbook wb = new Workbook("Book1.xlsx");
 
         PdfSaveOptions options = new PdfSaveOptions();
 
         //Print only Page 3 and Page 4 in the output PDF
         //Starting page index (0-based index)
         options.setPageIndex(3);
         //Number of pages to be printed
         options.setPageCount(2);
 
         //Save the PDF file
         wb.save("output.pdf", options);
```

**Returns:**
int
### getPageIndex() {#getPageIndex--}
```
public int getPageIndex()
```


Получает индекс первой страницы для сохранения, начиная с 0.

**Remarks**

По умолчанию 0.

**Example**

В следующем примере показано, как отрисовать диапазон страниц (3 и 4) в файле Microsoft Excel в PDF.

```
         //Open an Excel file
         Workbook wb = new Workbook("Book1.xlsx");
 
         PdfSaveOptions options = new PdfSaveOptions();
 
         //Print only Page 3 and Page 4 in the output PDF
         //Starting page index (0-based index)
         options.setPageIndex(3);
         //Number of pages to be printed
         options.setPageCount(2);
 
         //Save the PDF file
         wb.save("output.pdf", options);
```

**Returns:**
int
### getPageSavingCallback() {#getPageSavingCallback--}
```
public IPageSavingCallback getPageSavingCallback()
```


Контролировать/Указывать прогресс процесса сохранения страниц.

**Returns:**
[IPageSavingCallback](../../com.aspose.cells/ipagesavingcallback)
### getPdfCompression() {#getPdfCompression--}
```
public int getPdfCompression()
```


Указывает алгоритм сжатия

См. [PdfCompressionCore](../../com.aspose.cells/pdfcompressioncore).

**Returns:**
int
### getPrintingPageType() {#getPrintingPageType--}
```
public int getPrintingPageType()
```


Указывает, какие страницы не будут печататься.

См. [PrintingPageType](../../com.aspose.cells/printingpagetype).

**Remarks**

Если содержимое листа разреженное, некоторые страницы могут быть полностью пустыми в выходном pdf‑файле. Если вы не хотите этих пустых страниц, можете использовать эту опцию, чтобы их опустить.

**Example**

В следующем коде пропускаются пустые страницы или страницы, содержащие только стилистическое содержимое, например фон ячеек, границы.

```
         Workbook wb = new Workbook("Book1.xlsx");
 
         PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
 
         //ignore blank pages
         pdfSaveOptions.setPrintingPageType(PrintingPageType.IGNORE_BLANK);
 
         wb.save("output_ignore_blank_page.pdf", pdfSaveOptions);
 
 
         //ignore blank pages and pages which only contains some style content like cell background
         pdfSaveOptions.setPrintingPageType(PrintingPageType.IGNORE_STYLE);
 
         wb.save("output_ignore_blank_and_style_page.pdf", pdfSaveOptions);
```

**Returns:**
int
### getProducer() {#getProducer--}
```
public String getProducer()
```


Получает производителя сгенерированного PDF‑документа.

**Remarks**

Если значение null или действительная LICENSE не установлена, будет использована строка Aspose.Cells vVERSION.

**Returns:**
java.lang.String
### getRefreshChartCache() {#getRefreshChartCache--}
```
public boolean getRefreshChartCache()
```


Указывает, кэшировать ли последние данные диаграммы.

**Returns:**
boolean
### getRenderingBehavior() {#getRenderingBehavior--}
```
public int getRenderingBehavior()
```


Получает специфические для Excel поведения рендеринга, которые следует применить.

См. [ExcelRenderingBehavior](../../com.aspose.cells/excelrenderingbehavior).

**Remarks**

Значение по умолчанию — [ExcelRenderingBehavior.ALL](../../com.aspose.cells/excelrenderingbehavior\\#ALL).

**Returns:**
int
### getSaveFormat() {#getSaveFormat--}
```
public int getSaveFormat()
```


Получает формат сохраняемого файла.

Смотрите [SaveFormat](../../com.aspose.cells/saveformat).

**Returns:**
int
### getSecurityOptions() {#getSecurityOptions--}
```
public PdfSecurityOptions getSecurityOptions()
```


Установите эти параметры, когда в результате xls2pdf требуется безопасность.

**Example**

Следующий код устанавливает разрешение по высоте для печати в выходном PDF.

```
         Workbook wb = new Workbook();
         wb.getWorksheets().get(0).getCells().get("A1").setValue("Aspose");
 
         PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
 
 
         PdfSecurityOptions pdfSecurityOptions = new PdfSecurityOptions();
 
         //set owner password
         pdfSecurityOptions.setOwnerPassword("YourOwnerPassword");
 
         //set user password
         pdfSecurityOptions.setUserPassword("YourUserPassword");
 
         //set print permisson
         pdfSecurityOptions.setPrintPermission(true);
 
         //set high resolution for print
         pdfSecurityOptions.setFullQualityPrintPermission(true);
 
 
         pdfSaveOptions.setSecurityOptions(pdfSecurityOptions);
 
         wb.save("output.pdf", pdfSaveOptions);
```

**Returns:**
[PdfSecurityOptions](../../com.aspose.cells/pdfsecurityoptions)
### getSheetSet() {#getSheetSet--}
```
public SheetSet getSheetSet()
```


Получает листы для рендеринга. По умолчанию — все видимые листы в рабочей книге: [SheetSet.getVisible()](../../com.aspose.cells/sheetset\#getVisible--).

**Example**

В следующем коде отрисовывается только активный лист в pdf.

```
         Workbook workbook = new Workbook("Book1.xlsx");
 
         int activeSheetIndex = workbook.getWorksheets().getActiveSheetIndex();
 
         PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
         //set active sheet index to sheet set.
         pdfSaveOptions.setSheetSet(new SheetSet(new int[] { activeSheetIndex }));
         workbook.save("output.pdf", pdfSaveOptions);
```

**Returns:**
[SheetSet](../../com.aspose.cells/sheetset)
### getSortExternalNames() {#getSortExternalNames--}
```
public boolean getSortExternalNames()
```


Указывает, сортировать ли внешние определённые имена перед сохранением файла.

**Returns:**
boolean
### getSortNames() {#getSortNames--}
```
public boolean getSortNames()
```


Указывает, сортировать ли определённые имена перед сохранением файла.

**Returns:**
boolean
### getTextCrossType() {#getTextCrossType--}
```
public int getTextCrossType()
```


Получает тип отображаемого текста, когда ширина текста превышает ширину ячейки.

См. [TextCrossType](../../com.aspose.cells/textcrosstype).

**Returns:**
int
### getUpdateSmartArt() {#getUpdateSmartArt--}
```
public boolean getUpdateSmartArt()
```


Указывает, следует ли обновлять настройки Smart Art. Значение по умолчанию — false.

**Remarks**

Влияет только после вызова метода Shape.GetResultOfSmartArt() и если кэшированные фигуры существуют в файле шаблона.

**Returns:**
boolean
### getValidateMergedAreas() {#getValidateMergedAreas--}
```
public boolean getValidateMergedAreas()
```


Указывает, проверять ли объединённые ячейки перед сохранением файла.

**Remarks**

Значение по умолчанию — false.

**Returns:**
boolean
### getWarningCallback() {#getWarningCallback--}
```
public IWarningCallback getWarningCallback()
```


Получает обратный вызов предупреждения.

**Returns:**
[IWarningCallback](../../com.aspose.cells/iwarningcallback)
### getWatermark() {#getWatermark--}
```
public RenderingWatermark getWatermark()
```


Получает водяной знак для вывода.

**Example**

Следующий код устанавливает водяной знак в выходном PDF.

```
         //prepare a workbook with 3 pages.
         Workbook wb = new Workbook();
         wb.getWorksheets().get(0).getCells().get("A1").putValue("Page1");
         int index = wb.getWorksheets().add();
         wb.getWorksheets().get(index).getCells().get("A1").putValue("Page2");
         index = wb.getWorksheets().add();
         wb.getWorksheets().get(index).getCells().get("A1").putValue("Page3");
         wb.getWorksheets().get(index).getPageSetup().setPaperSize(PaperSizeType.PAPER_A_3);
 
         //create a font for watermark, and specify bold, italic, color
         RenderingFont font = new RenderingFont("Calibri", 68);
         font.setItalic(true);
         font.setBold(true);
         font.setColor(Color.getBlue());
 
         //create a watermark from text and the specified font
         RenderingWatermark watermark = new RenderingWatermark("Watermark", font);
 
         //specify horizontal and vertical alignment
         watermark.setHAlignment(TextAlignmentType.CENTER);
         watermark.setVAlignment(TextAlignmentType.CENTER);
 
         //specify rotation
         watermark.setRotation(30);
 
         //specify opacity
         watermark.setOpacity(0.6f);
 
         //specify the scale to page(e.g. 100, 50) in percent.
         watermark.setScaleToPagePercent(50);
 
         //spcify watermark for rendering to pdf.
         PdfSaveOptions options = new PdfSaveOptions();
         options.setWatermark(watermark);
 
         wb.save("output_watermark.pdf", options);
```

**Returns:**
[RenderingWatermark](../../com.aspose.cells/renderingwatermark)
### getZoomBehavior() {#getZoomBehavior--}
```
public int getZoomBehavior()
```


Получает начальный режим просмотра при открытии сгенерированного PDF‑документа. Значение по умолчанию — [PdfZoomBehavior.NONE](../../com.aspose.cells/pdfzoombehavior\\#NONE).

См. [PdfZoomBehavior](../../com.aspose.cells/pdfzoombehavior).

**Returns:**
int
### getZoomFactor() {#getZoomFactor--}
```
public int getZoomFactor()
```


Получает процент масштабирования, используемый, когда [getZoomBehavior()](../../com.aspose.cells/pdfsaveoptions\#getZoomBehavior--) является [PdfZoomBehavior.ZOOM\_FACTOR](../../com.aspose.cells/pdfzoombehavior\#ZOOM-FACTOR).

**Remarks**

Это свойство игнорируется, если только [getZoomBehavior()](../../com.aspose.cells/pdfsaveoptions\\#getZoomBehavior--) не равен [PdfZoomBehavior.ZOOM\\_FACTOR](../../com.aspose.cells/pdfzoombehavior\\#ZOOM-FACTOR).

**Returns:**
int
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isFontSubstitutionCharGranularity() {#isFontSubstitutionCharGranularity--}
```
public boolean isFontSubstitutionCharGranularity()
```


Указывает, следует ли заменять шрифт символа только в случае, когда шрифт ячейки не совместим с ним.

**Remarks**

По умолчанию false. Сначала будет использован шрифт по умолчанию из Workbook и PdfSaveOption/system для шрифта ячеек.

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




### setAllColumnsInOnePagePerSheet(boolean value) {#setAllColumnsInOnePagePerSheet-boolean-}
```
public void setAllColumnsInOnePagePerSheet(boolean value)
```


Если AllColumnsInOnePagePerSheet установлено в true, всё содержимое столбцов одного листа будет выводиться на одну страницу в результате. Ширина бумажного формата из pagesetup будет игнорироваться, а остальные настройки pagesetup сохранят своё действие.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setBookmark(PdfBookmarkEntry value) {#setBookmark-com.aspose.cells.PdfBookmarkEntry-}
```
public void setBookmark(PdfBookmarkEntry value)
```


Устанавливает объект [PdfBookmarkEntry](../../com.aspose.cells/pdfbookmarkentry).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| value | [PdfBookmarkEntry](../../com.aspose.cells/pdfbookmarkentry) |  |

### setCachedFileFolder(String value) {#setCachedFileFolder-java.lang.String-}
```
public void setCachedFileFolder(String value)
```


Папка для временных файлов, которые могут использоваться в качестве кэша данных.

**Remarks**

Если папка не указана, значение по умолчанию для неё — [CellsHelper.getCacheFolder()](../../com.aspose.cells/cellshelper\#getCacheFolder--). Если её значение по умолчанию равно null или пусто, либо указано как null или пусто, то при сохранении книги кэш‑файл использоваться не будет.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### setCalculateFormula(boolean value) {#setCalculateFormula-boolean-}
```
public void setCalculateFormula(boolean value)
```


Указывает, следует ли вычислять формулы перед сохранением PDF‑файла.

**Remarks**

Значение по умолчанию — false.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setCheckExcelRestriction(boolean value) {#setCheckExcelRestriction-boolean-}
```
public void setCheckExcelRestriction(boolean value)
```


Проверять ли ограничения файла Excel, когда пользователь изменяет связанные с ячейками объекты. Например, Excel не позволяет вводить строковое значение длиной более 32K. Когда вы вводите значение длиннее 32K, оно будет усечено.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setCheckFontCompatibility(boolean value) {#setCheckFontCompatibility-boolean-}
```
public void setCheckFontCompatibility(boolean value)
```


Указывает, следует ли проверять совместимость шрифтов для каждого символа в тексте.

**Remarks**

Значение по умолчанию — true. Отключение этого свойства может повысить производительность. Однако, если шрифт по умолчанию или указанный шрифт текста/символа нельзя использовать для рендеринга, в сгенерированном PDF могут появиться нечитаемые символы (например, блоки). В такой ситуации пользователю следует оставить это свойство включённым (true), чтобы был найден и использован альтернативный шрифт для рендеринга текста.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setCheckWorkbookDefaultFont(boolean value) {#setCheckWorkbookDefaultFont-boolean-}
```
public void setCheckWorkbookDefaultFont(boolean value)
```


Если символы в Excel являются Unicode и в стиле ячейки не установлен правильный шрифт, они могут отображаться как блоки в PDF или изображении. Установите значение true, чтобы попытаться использовать шрифт по умолчанию книги для отображения этих символов.

**Remarks**

По умолчанию — true.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setClearData(boolean value) {#setClearData-boolean-}
```
public void setClearData(boolean value)
```


Очищать книгу после сохранения файла.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setCompliance(int value) {#setCompliance-int-}
```
public void setCompliance(int value)
```


Устанавливает уровень соответствия стандартам PDF для выходных документов.

См. [PdfCompliance](../../com.aspose.cells/pdfcompliance).

**Remarks**

По умолчанию — Pdf17.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setCreateDirectory(boolean value) {#setCreateDirectory-boolean-}
```
public void setCreateDirectory(boolean value)
```


Если true и каталог не существует, каталог будет автоматически создан перед сохранением файла.

**Remarks**

Значение по умолчанию — false.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setCreatedTime(DateTime value) {#setCreatedTime-com.aspose.cells.DateTime-}
```
public void setCreatedTime(DateTime value)
```


Устанавливает время создания PDF‑документа.

**Remarks**

Если не установлено, будет использовано время создания PDF.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| value | [DateTime](../../com.aspose.cells/datetime) |  |

### setCustomPropertiesExport(int value) {#setCustomPropertiesExport-int-}
```
public void setCustomPropertiesExport(int value)
```


Устанавливает значение, определяющее способ экспорта [CustomDocumentPropertyCollection](../../com.aspose.cells/customdocumentpropertycollection) в PDF‑файл. Значение по умолчанию — None.

См. [PdfCustomPropertiesExport](../../com.aspose.cells/pdfcustompropertiesexport).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setCustomRenderSettings(CustomRenderSettings value) {#setCustomRenderSettings-com.aspose.cells.CustomRenderSettings-}
```
public void setCustomRenderSettings(CustomRenderSettings value)
```


Устанавливает пользовательские параметры во время рендеринга.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| value | [CustomRenderSettings](../../com.aspose.cells/customrendersettings) |  |

### setDefaultEditLanguage(int value) {#setDefaultEditLanguage-int-}
```
public void setDefaultEditLanguage(int value)
```


Устанавливает язык редактирования по умолчанию.

См. [DefaultEditLanguage](../../com.aspose.cells/defaulteditlanguage).

**Remarks**

Это может отображать/рендерить разные макеты абзацев текста при установленном различном языке редактирования. По умолчанию — [DefaultEditLanguage.AUTO](../../com.aspose.cells/defaulteditlanguage\#AUTO).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setDefaultFont(String value) {#setDefaultFont-java.lang.String-}
```
public void setDefaultFont(String value)
```


Если символы в Excel являются Unicode и в стиле ячейки не установлен правильный шрифт, они могут отображаться как блоки в PDF или изображении. Установите DefaultFont, например MingLiu или MS Gothic, чтобы отобразить эти символы. Если это свойство не задано, Aspose.Cells будет использовать системный шрифт по умолчанию для отображения этих Unicode‑символов.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### setDisplayDocTitle(boolean value) {#setDisplayDocTitle-boolean-}
```
public void setDisplayDocTitle(boolean value)
```


Указывает, следует ли отображать заголовок документа в строке заголовка окна.

**Remarks**

Если false, строка заголовка будет отображать имя PDF‑файла. Значение по умолчанию — false.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setDrawObjectEventHandler(DrawObjectEventHandler value) {#setDrawObjectEventHandler-com.aspose.cells.DrawObjectEventHandler-}
```
public void setDrawObjectEventHandler(DrawObjectEventHandler value)
```


Реализует этот интерфейс для получения DrawObject и Bound при рендеринге.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| value | [DrawObjectEventHandler](../../com.aspose.cells/drawobjecteventhandler) |  |

### setEmbedAttachments(boolean value) {#setEmbedAttachments-boolean-}
```
public void setEmbedAttachments(boolean value)
```


Указывает, следует ли встраивать вложения для объектов OLE в Excel.

**Remarks**

Значение по умолчанию — false. Значение должно быть false, когда включена совместимость PDF/A или включено шифрование PDF.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setEmbedStandardWindowsFonts(boolean value) {#setEmbedStandardWindowsFonts-boolean-}
```
public void setEmbedStandardWindowsFonts(boolean value)
```


True — встраивать шрифты TrueType. Это влияет только на символы ASCII 32‑127. Шрифты для кодов символов выше 127 всегда встраиваются. Шрифты всегда встраиваются для стандарта PDF/A‑1a, PDF/A‑1b. По умолчанию — true.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setEmfRenderSetting(int value) {#setEmfRenderSetting-int-}
```
public void setEmfRenderSetting(int value)
```


Настройка рендеринга метафайла Emf.

См. [EmfRenderSetting](../../com.aspose.cells/emfrendersetting).

**Remarks**

Метaфайлы EMF, идентифицированные как "EMF+ Dual", могут содержать как записи EMF+, так и записи EMF. Любой тип записей может использоваться для рендеринга изображения, только записи EMF+, или только записи EMF. Когда установлен [EmfRenderSetting.EMF\_PLUS\_PREFER](../../com.aspose.cells/emfrendersetting\#EMF-PLUS-PREFER), записи EMF+ будут обрабатываться при рендеринге страницы, в противном случае будут обрабатываться только записи EMF. Значение по умолчанию — [EmfRenderSetting.EMF\_ONLY](../../com.aspose.cells/emfrendersetting\#EMF-ONLY).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setEncryptDocumentProperties(boolean value) {#setEncryptDocumentProperties-boolean-}
```
public void setEncryptDocumentProperties(boolean value)
```


Указывает, следует ли шифровать свойства документа при сохранении в файл .xls. Значение по умолчанию — true.

**Remarks**

Только для файлов .xls, .xlsx, .xlsb и .xlsm.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setExportDocumentStructure(boolean value) {#setExportDocumentStructure-boolean-}
```
public void setExportDocumentStructure(boolean value)
```


Указывает, следует ли экспортировать структуру документа.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setFontEncoding(int value) {#setFontEncoding-int-}
```
public void setFontEncoding(int value)
```


Устанавливает кодировку встроенных шрифтов в PDF.

См. [PdfFontEncoding](../../com.aspose.cells/pdffontencoding).

**Remarks**

Значение по умолчанию — [PdfFontEncoding.IDENTITY](../../com.aspose.cells/pdffontencoding\\#IDENTITY)

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setFontSubstitutionCharGranularity(boolean value) {#setFontSubstitutionCharGranularity-boolean-}
```
public void setFontSubstitutionCharGranularity(boolean value)
```


Указывает, следует ли заменять шрифт символа только в случае, когда шрифт ячейки не совместим с ним.

**Remarks**

По умолчанию false. Сначала будет использован шрифт по умолчанию из Workbook и PdfSaveOption/system для шрифта ячеек.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setGridlineColor(Color value) {#setGridlineColor-com.aspose.cells.Color-}
```
public void setGridlineColor(Color value)
```


Устанавливает цвет линий сетки.

**Remarks**

Он будет игнорировать настройки цвета линий сетки в исходном файле.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| value | [Color](../../com.aspose.cells/color) |  |

### setGridlineType(int value) {#setGridlineType-int-}
```
public void setGridlineType(int value)
```


Устанавливает тип линий сетки.

См. [GridlineType](../../com.aspose.cells/gridlinetype).

**Remarks**

По умолчанию — тип Dotted.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setIgnoreError(boolean value) {#setIgnoreError-boolean-}
```
public void setIgnoreError(boolean value)
```


Указывает, нужно ли скрывать ошибку во время рендеринга. Ошибка может быть связана с формой, изображением, рендерингом диаграммы и т.д.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setImageResample(int desiredPPI, int jpegQuality) {#setImageResample-int-int-}
```
public void setImageResample(int desiredPPI, int jpegQuality)
```


Устанавливает желаемое PPI (точек на дюйм) для ресэмплинга изображений и качество JPEG. Все изображения будут преобразованы в JPEG с указанным качеством, а изображения с PPI выше заданного будут ресэмплированы.

**Example**

Следующий код устанавливает желаемое PPI равным 96 и качество JPEG равным 80 для изображений в выходном PDF.

```
         //load the source file with images.
         Workbook wb = new Workbook("Book1.xlsx");
 
         PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
 
         //set desired PPI as 96 and jpeg quality as 80.
         pdfSaveOptions.setImageResample(96, 80);
 
         wb.save("output.pdf", pdfSaveOptions);
```

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| desiredPPI | int | Желаемое количество пикселей на дюйм. 220 — высокое качество. 150 — качество для экрана. 96 — качество для электронной почты. |
| jpegQuality | int | 0 – 100 % качества JPEG. |

### setImageType(ImageFormat value) {#setImageType-com.aspose.cells.ImageFormat-}
```
public void setImageType(ImageFormat value)
```


Представляет тип изображения при преобразовании диаграммы и фигуры.

**Remarks**

NOTE: Этот член теперь устарел. Вместо этого Chart и Shape всегда рендерятся как векторные элементы (например, точка, линия) для обеспечения качества рендеринга. Это свойство будет удалено через 12 месяцев, начиная с июня 2022 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| value | [ImageFormat](../../com.aspose.cells/imageformat) |  |

### setMergeAreas(boolean value) {#setMergeAreas-boolean-}
```
public void setMergeAreas(boolean value)
```


Указывает, следует ли объединять области условного форматирования и проверки перед сохранением файла.

**Remarks**

Значение по умолчанию — false.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setOnePagePerSheet(boolean value) {#setOnePagePerSheet-boolean-}
```
public void setOnePagePerSheet(boolean value)
```


Если OnePagePerSheet равно true, всё содержимое одного листа будет выводиться только на одну страницу в результате. Размер бумаги в pagesetup будет недействительным, а остальные настройки pagesetup по‑прежнему будут применяться.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setOptimizationType(int value) {#setOptimizationType-int-}
```
public void setOptimizationType(int value)
```


Устанавливает тип оптимизации PDF.

См. [PdfOptimizationType](../../com.aspose.cells/pdfoptimizationtype).

**Remarks**

Значение по умолчанию — [PdfOptimizationType.STANDARD](../../com.aspose.cells/pdfoptimizationtype\\#STANDARD)

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setOutputBlankPageWhenNothingToPrint(boolean value) {#setOutputBlankPageWhenNothingToPrint-boolean-}
```
public void setOutputBlankPageWhenNothingToPrint(boolean value)
```


Указывает, следует ли выводить пустую страницу, когда нечего печатать.

**Remarks**

По умолчанию — true.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setPageCount(int value) {#setPageCount-int-}
```
public void setPageCount(int value)
```


Устанавливает количество страниц для сохранения.

**Remarks**

По умолчанию это System.Int32.MaxValue, что означает, что все страницы будут отрисованы.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setPageIndex(int value) {#setPageIndex-int-}
```
public void setPageIndex(int value)
```


Устанавливает нулевой индекс первой страницы для сохранения.

**Remarks**

По умолчанию 0.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setPageSavingCallback(IPageSavingCallback value) {#setPageSavingCallback-com.aspose.cells.IPageSavingCallback-}
```
public void setPageSavingCallback(IPageSavingCallback value)
```


Контролировать/Указывать прогресс процесса сохранения страниц.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| value | [IPageSavingCallback](../../com.aspose.cells/ipagesavingcallback) |  |

### setPdfCompression(int value) {#setPdfCompression-int-}
```
public void setPdfCompression(int value)
```


Указывает алгоритм сжатия

См. [PdfCompressionCore](../../com.aspose.cells/pdfcompressioncore).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setPrintingPageType(int value) {#setPrintingPageType-int-}
```
public void setPrintingPageType(int value)
```


Указывает, какие страницы не будут печататься.

См. [PrintingPageType](../../com.aspose.cells/printingpagetype).

**Remarks**

Если содержимое листа разреженное, некоторые страницы могут быть полностью пустыми в выходном pdf‑файле. Если вы не хотите этих пустых страниц, можете использовать эту опцию, чтобы их опустить.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setProducer(String value) {#setProducer-java.lang.String-}
```
public void setProducer(String value)
```


Устанавливает производителя сгенерированного PDF‑документа.

**Remarks**

Если значение null или действительная LICENSE не установлена, будет использована строка Aspose.Cells vVERSION.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### setRefreshChartCache(boolean value) {#setRefreshChartCache-boolean-}
```
public void setRefreshChartCache(boolean value)
```


Указывает, кэшировать ли последние данные диаграммы.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setRenderingBehavior(int value) {#setRenderingBehavior-int-}
```
public void setRenderingBehavior(int value)
```


Устанавливает специфические для Excel поведения рендеринга, которые следует применить.

См. [ExcelRenderingBehavior](../../com.aspose.cells/excelrenderingbehavior).

**Remarks**

Значение по умолчанию — [ExcelRenderingBehavior.ALL](../../com.aspose.cells/excelrenderingbehavior\\#ALL).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setSecurityOptions(PdfSecurityOptions value) {#setSecurityOptions-com.aspose.cells.PdfSecurityOptions-}
```
public void setSecurityOptions(PdfSecurityOptions value)
```


Установите эти параметры, когда в результате xls2pdf требуется безопасность.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| value | [PdfSecurityOptions](../../com.aspose.cells/pdfsecurityoptions) |  |

### setSheetSet(SheetSet value) {#setSheetSet-com.aspose.cells.SheetSet-}
```
public void setSheetSet(SheetSet value)
```


Устанавливает листы для отображения. По умолчанию — все видимые листы в рабочей книге: [SheetSet.getVisible()](../../com.aspose.cells/sheetset\#getVisible--).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| value | [SheetSet](../../com.aspose.cells/sheetset) |  |

### setSortExternalNames(boolean value) {#setSortExternalNames-boolean-}
```
public void setSortExternalNames(boolean value)
```


Указывает, сортировать ли внешние определённые имена перед сохранением файла.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setSortNames(boolean value) {#setSortNames-boolean-}
```
public void setSortNames(boolean value)
```


Указывает, сортировать ли определённые имена перед сохранением файла.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setTextCrossType(int value) {#setTextCrossType-int-}
```
public void setTextCrossType(int value)
```


Устанавливает тип отображаемого текста, когда ширина текста превышает ширину ячейки.

См. [TextCrossType](../../com.aspose.cells/textcrosstype).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setUpdateSmartArt(boolean value) {#setUpdateSmartArt-boolean-}
```
public void setUpdateSmartArt(boolean value)
```


Указывает, следует ли обновлять настройки Smart Art. Значение по умолчанию — false.

**Remarks**

Влияет только после вызова метода Shape.GetResultOfSmartArt() и если кэшированные фигуры существуют в файле шаблона.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setValidateMergedAreas(boolean value) {#setValidateMergedAreas-boolean-}
```
public void setValidateMergedAreas(boolean value)
```


Указывает, проверять ли объединённые ячейки перед сохранением файла.

**Remarks**

Значение по умолчанию — false.

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

### setWatermark(RenderingWatermark value) {#setWatermark-com.aspose.cells.RenderingWatermark-}
```
public void setWatermark(RenderingWatermark value)
```


Устанавливает водяной знак в вывод.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| value | [RenderingWatermark](../../com.aspose.cells/renderingwatermark) |  |

### setZoomBehavior(int value) {#setZoomBehavior-int-}
```
public void setZoomBehavior(int value)
```


Устанавливает режим начального просмотра при открытии сгенерированного PDF‑документа. Значение по умолчанию — [PdfZoomBehavior.NONE](../../com.aspose.cells/pdfzoombehavior\#NONE).

См. [PdfZoomBehavior](../../com.aspose.cells/pdfzoombehavior).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setZoomFactor(int value) {#setZoomFactor-int-}
```
public void setZoomFactor(int value)
```


Устанавливает процент масштабирования, используемый, когда [getZoomBehavior()](../../com.aspose.cells/pdfsaveoptions\\#getZoomBehavior--) равен [PdfZoomBehavior.ZOOM\\_FACTOR](../../com.aspose.cells/pdfzoombehavior\\#ZOOM-FACTOR).

**Remarks**

Это свойство игнорируется, если только [getZoomBehavior()](../../com.aspose.cells/pdfsaveoptions\\#getZoomBehavior--) не равен [PdfZoomBehavior.ZOOM\\_FACTOR](../../com.aspose.cells/pdfzoombehavior\\#ZOOM-FACTOR).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

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

