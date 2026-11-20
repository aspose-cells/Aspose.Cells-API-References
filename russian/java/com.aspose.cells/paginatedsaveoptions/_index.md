---
title: "PaginatedSaveOptions"
second_title: "Справочник API Aspose.Cells for Java"
description: "Представляет параметры пагинации."
type: docs
url: /ru/java/com.aspose.cells/paginatedsaveoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.SaveOptions](../../com.aspose.cells/saveoptions)
```
public abstract class PaginatedSaveOptions extends SaveOptions
```

Представляет параметры пагинации.
## Конструкторы

| Конструктор | Описание |
| --- | --- |
| [PaginatedSaveOptions()](#PaginatedSaveOptions--) |  |
## Методы

| Метод | Описание |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAllColumnsInOnePagePerSheet()](#getAllColumnsInOnePagePerSheet--) | Если AllColumnsInOnePagePerSheet равно true, всё содержимое столбцов одного листа будет выводиться только на одну страницу в результате. |
| [getCachedFileFolder()](#getCachedFileFolder--) | Папка для временных файлов, которые могут использоваться в качестве кэша данных. |
| [getCheckExcelRestriction()](#getCheckExcelRestriction--) | Проверять ли ограничения Excel‑файла, когда пользователь изменяет связанные с ячейками объекты. |
| [getCheckFontCompatibility()](#getCheckFontCompatibility--) | Указывает, следует ли проверять совместимость шрифтов для каждого символа в тексте. |
| [getCheckWorkbookDefaultFont()](#getCheckWorkbookDefaultFont--) | Когда символы в Excel являются Unicode и в стиле ячейки не установлен правильный шрифт, они могут отображаться как блоки в pdf,image. |
| [getClass()](#getClass--) |  |
| [getClearData()](#getClearData--) | Очищать книгу после сохранения файла. |
| [getCreateDirectory()](#getCreateDirectory--) | Если true и каталог не существует, каталог будет автоматически создан перед сохранением файла. |
| [getCustomRenderSettings()](#getCustomRenderSettings--) | Получает пользовательские настройки во время рендеринга. |
| [getDefaultEditLanguage()](#getDefaultEditLanguage--) | Получает язык редактирования по умолчанию. |
| [getDefaultFont()](#getDefaultFont--) | Когда символы в Excel являются Unicode и в стиле ячейки не установлен правильный шрифт, они могут отображаться как блоки в pdf,image. |
| [getDrawObjectEventHandler()](#getDrawObjectEventHandler--) | Реализует этот интерфейс для получения DrawObject и Bound при рендеринге. |
| [getEmfRenderSetting()](#getEmfRenderSetting--) | Настройка рендеринга метафайла Emf. |
| [getEncryptDocumentProperties()](#getEncryptDocumentProperties--) | Указывает, следует ли шифровать свойства документа при сохранении в формате .xls. |
| [getGridlineColor()](#getGridlineColor--) | Получает цвет линий сетки. |
| [getGridlineType()](#getGridlineType--) | Получает тип линий сетки. |
| [getIgnoreError()](#getIgnoreError--) | Указывает, нужно ли скрывать ошибку во время рендеринга. |
| [getMergeAreas()](#getMergeAreas--) | Указывает, следует ли объединять области условного форматирования и проверки перед сохранением файла. |
| [getOnePagePerSheet()](#getOnePagePerSheet--) | Если OnePagePerSheet равно true, всё содержимое одного листа будет выводиться только на одну страницу в результате. |
| [getOutputBlankPageWhenNothingToPrint()](#getOutputBlankPageWhenNothingToPrint--) | Указывает, следует ли выводить пустую страницу, когда нечего печатать. |
| [getPageCount()](#getPageCount--) | Получает количество страниц для сохранения. |
| [getPageIndex()](#getPageIndex--) | Получает индекс первой страницы для сохранения, начиная с 0. |
| [getPageSavingCallback()](#getPageSavingCallback--) | Контролировать/Указывать прогресс процесса сохранения страниц. |
| [getPrintingPageType()](#getPrintingPageType--) | Указывает, какие страницы не будут печататься. |
| [getRefreshChartCache()](#getRefreshChartCache--) | Указывает, кэшировать ли последние данные диаграммы. |
| [getRenderingBehavior()](#getRenderingBehavior--) | Получает специфические для Excel поведения рендеринга, которые следует применить. |
| [getSaveFormat()](#getSaveFormat--) | Получает формат сохраняемого файла. |
| [getSheetSet()](#getSheetSet--) | Получает листы для рендеринга. |
| [getSortExternalNames()](#getSortExternalNames--) | Указывает, сортировать ли внешние определённые имена перед сохранением файла. |
| [getSortNames()](#getSortNames--) | Указывает, сортировать ли определённые имена перед сохранением файла. |
| [getTextCrossType()](#getTextCrossType--) | Получает тип отображаемого текста, когда ширина текста превышает ширину ячейки. |
| [getUpdateSmartArt()](#getUpdateSmartArt--) | Указывает, обновлять ли настройки SmartArt. |
| [getValidateMergedAreas()](#getValidateMergedAreas--) | Указывает, проверять ли объединённые ячейки перед сохранением файла. |
| [getWarningCallback()](#getWarningCallback--) | Получает обратный вызов предупреждения. |
| [hashCode()](#hashCode--) |  |
| [isFontSubstitutionCharGranularity()](#isFontSubstitutionCharGranularity--) | Указывает, следует ли заменять шрифт символа только в случае, когда шрифт ячейки не совместим с ним. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAllColumnsInOnePagePerSheet(boolean value)](#setAllColumnsInOnePagePerSheet-boolean-) | Если AllColumnsInOnePagePerSheet равно true, всё содержимое столбцов одного листа будет выводиться только на одну страницу в результате. |
| [setCachedFileFolder(String value)](#setCachedFileFolder-java.lang.String-) | Папка для временных файлов, которые могут использоваться в качестве кэша данных. |
| [setCheckExcelRestriction(boolean value)](#setCheckExcelRestriction-boolean-) | Проверять ли ограничения Excel‑файла, когда пользователь изменяет связанные с ячейками объекты. |
| [setCheckFontCompatibility(boolean value)](#setCheckFontCompatibility-boolean-) | Указывает, следует ли проверять совместимость шрифтов для каждого символа в тексте. |
| [setCheckWorkbookDefaultFont(boolean value)](#setCheckWorkbookDefaultFont-boolean-) | Когда символы в Excel являются Unicode и в стиле ячейки не установлен правильный шрифт, они могут отображаться как блоки в pdf,image. |
| [setClearData(boolean value)](#setClearData-boolean-) | Очищать книгу после сохранения файла. |
| [setCreateDirectory(boolean value)](#setCreateDirectory-boolean-) | Если true и каталог не существует, каталог будет автоматически создан перед сохранением файла. |
| [setCustomRenderSettings(CustomRenderSettings value)](#setCustomRenderSettings-com.aspose.cells.CustomRenderSettings-) | Устанавливает пользовательские параметры во время рендеринга. |
| [setDefaultEditLanguage(int value)](#setDefaultEditLanguage-int-) | Устанавливает язык редактирования по умолчанию. |
| [setDefaultFont(String value)](#setDefaultFont-java.lang.String-) | Когда символы в Excel являются Unicode и в стиле ячейки не установлен правильный шрифт, они могут отображаться как блоки в pdf,image. |
| [setDrawObjectEventHandler(DrawObjectEventHandler value)](#setDrawObjectEventHandler-com.aspose.cells.DrawObjectEventHandler-) | Реализует этот интерфейс для получения DrawObject и Bound при рендеринге. |
| [setEmfRenderSetting(int value)](#setEmfRenderSetting-int-) | Настройка рендеринга метафайла Emf. |
| [setEncryptDocumentProperties(boolean value)](#setEncryptDocumentProperties-boolean-) | Указывает, следует ли шифровать свойства документа при сохранении в формате .xls. |
| [setFontSubstitutionCharGranularity(boolean value)](#setFontSubstitutionCharGranularity-boolean-) | Указывает, следует ли заменять шрифт символа только в случае, когда шрифт ячейки не совместим с ним. |
| [setGridlineColor(Color value)](#setGridlineColor-com.aspose.cells.Color-) | Устанавливает цвет линий сетки. |
| [setGridlineType(int value)](#setGridlineType-int-) | Устанавливает тип линий сетки. |
| [setIgnoreError(boolean value)](#setIgnoreError-boolean-) | Указывает, нужно ли скрывать ошибку во время рендеринга. |
| [setMergeAreas(boolean value)](#setMergeAreas-boolean-) | Указывает, следует ли объединять области условного форматирования и проверки перед сохранением файла. |
| [setOnePagePerSheet(boolean value)](#setOnePagePerSheet-boolean-) | Если OnePagePerSheet равно true, всё содержимое одного листа будет выводиться только на одну страницу в результате. |
| [setOutputBlankPageWhenNothingToPrint(boolean value)](#setOutputBlankPageWhenNothingToPrint-boolean-) | Указывает, следует ли выводить пустую страницу, когда нечего печатать. |
| [setPageCount(int value)](#setPageCount-int-) | Устанавливает количество страниц для сохранения. |
| [setPageIndex(int value)](#setPageIndex-int-) | Устанавливает нулевой индекс первой страницы для сохранения. |
| [setPageSavingCallback(IPageSavingCallback value)](#setPageSavingCallback-com.aspose.cells.IPageSavingCallback-) | Контролировать/Указывать прогресс процесса сохранения страниц. |
| [setPrintingPageType(int value)](#setPrintingPageType-int-) | Указывает, какие страницы не будут печататься. |
| [setRefreshChartCache(boolean value)](#setRefreshChartCache-boolean-) | Указывает, кэшировать ли последние данные диаграммы. |
| [setRenderingBehavior(int value)](#setRenderingBehavior-int-) | Устанавливает специфические для Excel поведения рендеринга, которые следует применить. |
| [setSheetSet(SheetSet value)](#setSheetSet-com.aspose.cells.SheetSet-) | Устанавливает листы для рендеринга. |
| [setSortExternalNames(boolean value)](#setSortExternalNames-boolean-) | Указывает, сортировать ли внешние определённые имена перед сохранением файла. |
| [setSortNames(boolean value)](#setSortNames-boolean-) | Указывает, сортировать ли определённые имена перед сохранением файла. |
| [setTextCrossType(int value)](#setTextCrossType-int-) | Устанавливает тип отображаемого текста, когда ширина текста превышает ширину ячейки. |
| [setUpdateSmartArt(boolean value)](#setUpdateSmartArt-boolean-) | Указывает, обновлять ли настройки SmartArt. |
| [setValidateMergedAreas(boolean value)](#setValidateMergedAreas-boolean-) | Указывает, проверять ли объединённые ячейки перед сохранением файла. |
| [setWarningCallback(IWarningCallback value)](#setWarningCallback-com.aspose.cells.IWarningCallback-) | Устанавливает обратный вызов предупреждения. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### PaginatedSaveOptions() {#PaginatedSaveOptions--}
```
public PaginatedSaveOptions()
```


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
### getCachedFileFolder() {#getCachedFileFolder--}
```
public String getCachedFileFolder()
```


Папка для временных файлов, которые могут использоваться в качестве кэша данных.

**Remarks**

Если папка не указана, значение по умолчанию для неё — [CellsHelper.getCacheFolder()](../../com.aspose.cells/cellshelper\#getCacheFolder--). Если её значение по умолчанию равно null или пусто, либо указано как null или пусто, то при сохранении книги кэш‑файл использоваться не будет.

**Returns:**
java.lang.String
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
### getCreateDirectory() {#getCreateDirectory--}
```
public boolean getCreateDirectory()
```


Если true и каталог не существует, каталог будет автоматически создан перед сохранением файла.

**Remarks**

Значение по умолчанию — false.

**Returns:**
boolean
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
### getDrawObjectEventHandler() {#getDrawObjectEventHandler--}
```
public DrawObjectEventHandler getDrawObjectEventHandler()
```


Реализует этот интерфейс для получения DrawObject и Bound при рендеринге.

**Returns:**
[DrawObjectEventHandler](../../com.aspose.cells/drawobjecteventhandler)
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

### setDrawObjectEventHandler(DrawObjectEventHandler value) {#setDrawObjectEventHandler-com.aspose.cells.DrawObjectEventHandler-}
```
public void setDrawObjectEventHandler(DrawObjectEventHandler value)
```


Реализует этот интерфейс для получения DrawObject и Bound при рендеринге.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| value | [DrawObjectEventHandler](../../com.aspose.cells/drawobjecteventhandler) |  |

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

