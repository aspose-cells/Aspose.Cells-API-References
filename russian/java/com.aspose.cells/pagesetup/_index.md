---
title: "PageSetup"
second_title: "Справочник API Aspose.Cells for Java"
description: "Инкапсулирует объект, представляющий описание настройки страницы."
type: docs
url: /ru/java/com.aspose.cells/pagesetup/
---

**Inheritance:**
java.lang.Object
```
public class PageSetup
```

Инкапсулирует объект, представляющий описание настройки страницы. Объект PageSetup содержит все параметры настройки страницы.

**Example**

```
         Workbook workbook = new Workbook();
 
         WorksheetCollection sheets = workbook.getWorksheets();
 
         //Add a worksheet
         sheets.add();
         Worksheet sheet = sheets.get(1);
         PageSetup pageSetup = sheet.getPageSetup();
         pageSetup.setPrintArea("D1:K13");
 
         //do your business
```
## Методы

| Метод | Описание |
| --- | --- |
| [clearHeaderFooter()](#clearHeaderFooter--) | Очищает настройки заголовка и нижнего колонтитула. |
| [copy(PageSetup source, CopyOptions copyOptions)](#copy-com.aspose.cells.PageSetup-com.aspose.cells.CopyOptions-) | Копирует настройки page setup. |
| [customPaperSize(double width, double height)](#customPaperSize-double-double-) | Устанавливает пользовательский размер бумаги, в дюймах. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getBlackAndWhite()](#getBlackAndWhite--) | Определяет, будут ли элементы документа печататься в чёрно‑белом виде. |
| [getBottomMargin()](#getBottomMargin--) | Определяет размер нижнего поля, в сантиметрах. |
| [getBottomMarginInch()](#getBottomMarginInch--) | Определяет размер нижнего поля, в дюймах. |
| [getCenterHorizontally()](#getCenterHorizontally--) | Определяет, печатается ли лист по горизонтали по центру. |
| [getCenterVertically()](#getCenterVertically--) | Определяет, печатается ли лист по вертикали по центру. |
| [getClass()](#getClass--) |  |
| [getCommands(String headerFooterScript)](#getCommands-java.lang.String-) | Получает все команды заголовка или нижнего колонтитула. |
| [getEvenFooter(int section)](#getEvenFooter-int-) | Получает скрипт, форматирующий четный нижний колонтитул Excel‑файла. |
| [getEvenHeader(int section)](#getEvenHeader-int-) | Получает скрипт, форматирующий четный заголовок Excel‑файла. |
| [getFirstPageFooter(int section)](#getFirstPageFooter-int-) | Получает скрипт, форматирующий нижний колонтитул первой страницы Excel‑файла. |
| [getFirstPageHeader(int section)](#getFirstPageHeader-int-) | Получает скрипт, форматирующий заголовок первой страницы Excel‑файла. |
| [getFirstPageNumber()](#getFirstPageNumber--) | Представляет номер первой страницы, который будет использоваться при печати этого листа. |
| [getFitToPagesTall()](#getFitToPagesTall--) | Представляет количество страниц по высоте, до которого будет масштабироваться лист при печати. |
| [getFitToPagesWide()](#getFitToPagesWide--) | Представляет количество страниц по ширине, до которого будет масштабироваться лист при печати. |
| [getFooter(int section)](#getFooter-int-) | Получает скрипт, форматирующий нижний колонтитул Excel‑файла. |
| [getFooterMargin()](#getFooterMargin--) | Представляет расстояние от нижней части страницы до нижнего колонтитула в сантиметрах. |
| [getFooterMarginInch()](#getFooterMarginInch--) | Представляет расстояние от нижней части страницы до нижнего колонтитула в дюймах. |
| [getHeader(int section)](#getHeader-int-) | Получает скрипт, форматирующий заголовок Excel‑файла. |
| [getHeaderMargin()](#getHeaderMargin--) | Представляет расстояние от верхней части страницы до заголовка в сантиметрах. |
| [getHeaderMarginInch()](#getHeaderMarginInch--) | Представляет расстояние от верхней части страницы до заголовка в дюймах. |
| [getLeftMargin()](#getLeftMargin--) | Представляет размер левого поля в сантиметрах. |
| [getLeftMarginInch()](#getLeftMarginInch--) | Представляет размер левого поля в дюймах. |
| [getODSPageBackground()](#getODSPageBackground--) | Получает фон ODS. |
| [getOrder()](#getOrder--) | Представляет порядок, который Microsoft Excel использует для нумерации страниц при печати большого листа. |
| [getOrientation()](#getOrientation--) | Представляет ориентацию печати страницы. |
| [getPaperHeight()](#getPaperHeight--) | Получает высоту бумаги в дюймах, учитывая ориентацию страницы. |
| [getPaperSize()](#getPaperSize--) | Представляет размер бумаги. |
| [getPaperWidth()](#getPaperWidth--) | Получает ширину бумаги в дюймах, учитывая ориентацию страницы. |
| [getPicture(boolean isFirst, boolean isEven, boolean isHeader, int section)](#getPicture-boolean-boolean-boolean-int-) | Получает объект [Picture](../../com.aspose.cells/picture) заголовка / нижнего колонтитула. |
| [getPicture(boolean isHeader, int section)](#getPicture-boolean-int-) | Получает объект [Picture](../../com.aspose.cells/picture) заголовка / нижнего колонтитула. |
| [getPrintArea()](#getPrintArea--) | Представляет диапазон для печати. |
| [getPrintComments()](#getPrintComments--) | Представляет способ печати комментариев вместе с листом. |
| [getPrintCopies()](#getPrintCopies--) | Получает количество копий для печати. |
| [getPrintDraft()](#getPrintDraft--) | Представляет, будет ли лист печататься без графики. |
| [getPrintErrors()](#getPrintErrors--) | Указывает тип отображаемой ошибки печати. |
| [getPrintGridlines()](#getPrintGridlines--) | Представляет, печатаются ли линии сетки ячеек на странице. |
| [getPrintHeadings()](#getPrintHeadings--) | Представляет, печатаются ли заголовки строк и столбцов на этой странице. |
| [getPrintQuality()](#getPrintQuality--) | Представляет качество печати. |
| [getPrintTitleColumns()](#getPrintTitleColumns--) | Представляет столбцы, содержащие ячейки, которые повторяются слева от каждой страницы. |
| [getPrintTitleRows()](#getPrintTitleRows--) | Представляет строки, содержащие ячейки, которые повторяются вверху каждой страницы. |
| [getPrinterSettings()](#getPrinterSettings--) | Получает настройки принтера по умолчанию. |
| [getRightMargin()](#getRightMargin--) | Представляет размер правого поля в сантиметрах. |
| [getRightMarginInch()](#getRightMarginInch--) | Представляет размер правого поля в дюймах. |
| [getTopMargin()](#getTopMargin--) | Представляет размер верхнего поля в сантиметрах. |
| [getTopMarginInch()](#getTopMarginInch--) | Представляет размер верхнего поля в дюймах. |
| [getZoom()](#getZoom--) | Представляет коэффициент масштабирования в процентах. |
| [hashCode()](#hashCode--) |  |
| [isAutoFirstPageNumber()](#isAutoFirstPageNumber--) | Указывает, назначается ли номер первой страницы автоматически. |
| [isAutomaticPaperSize()](#isAutomaticPaperSize--) | Указывает, является ли размер бумаги автоматическим. |
| [isHFAlignMargins()](#isHFAlignMargins--) | Указывает, выравниваются ли поля верхнего и нижнего колонтитулов с полями страницы. |
| [isHFDiffFirst()](#isHFDiffFirst--) | True означает, что верхний/нижний колонтитул первой страницы отличается от остальных страниц. |
| [isHFDiffOddEven()](#isHFDiffOddEven--) | True означает, что верхний/нижний колонтитул нечётных страниц отличается от остальных нечётных страниц. |
| [isHFScaleWithDoc()](#isHFScaleWithDoc--) | Указывает, масштабируются ли верхний и нижний колонтитулы вместе с масштабированием документа. |
| [isPercentScale()](#isPercentScale--) | Если это свойство равно False, свойства FitToPagesWide и FitToPagesTall определяют, как масштабируется лист. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAutoFirstPageNumber(boolean value)](#setAutoFirstPageNumber-boolean-) | Указывает, назначается ли номер первой страницы автоматически. |
| [setBlackAndWhite(boolean value)](#setBlackAndWhite-boolean-) | Определяет, будут ли элементы документа печататься в чёрно‑белом виде. |
| [setBottomMargin(double value)](#setBottomMargin-double-) | Определяет размер нижнего поля, в сантиметрах. |
| [setBottomMarginInch(double value)](#setBottomMarginInch-double-) | Определяет размер нижнего поля, в дюймах. |
| [setCenterHorizontally(boolean value)](#setCenterHorizontally-boolean-) | Определяет, печатается ли лист по горизонтали по центру. |
| [setCenterVertically(boolean value)](#setCenterVertically-boolean-) | Определяет, печатается ли лист по вертикали по центру. |
| [setEvenFooter(int section, String footerScript)](#setEvenFooter-int-java.lang.String-) | Задает скрипт форматирования нижнего колонтитула чётных страниц Excel‑файла. |
| [setEvenHeader(int section, String headerScript)](#setEvenHeader-int-java.lang.String-) | Задает скрипт форматирования верхнего колонтитула чётных страниц Excel‑файла. |
| [setFirstPageFooter(int section, String footerScript)](#setFirstPageFooter-int-java.lang.String-) | Задает скрипт форматирования нижнего колонтитула первой страницы Excel‑файла. |
| [setFirstPageHeader(int section, String headerScript)](#setFirstPageHeader-int-java.lang.String-) | Задает скрипт форматирования верхнего колонтитула первой страницы Excel‑файла. |
| [setFirstPageNumber(int value)](#setFirstPageNumber-int-) | Представляет номер первой страницы, который будет использоваться при печати этого листа. |
| [setFitToPages(int wide, int tall)](#setFitToPages-int-int-) | Задает количество страниц, до которых будет масштабироваться лист при печати. |
| [setFitToPagesTall(int value)](#setFitToPagesTall-int-) | Представляет количество страниц по высоте, до которого будет масштабироваться лист при печати. |
| [setFitToPagesWide(int value)](#setFitToPagesWide-int-) | Представляет количество страниц по ширине, до которого будет масштабироваться лист при печати. |
| [setFooter(int section, String footerScript)](#setFooter-int-java.lang.String-) | Устанавливает скрипт форматирования нижнего колонтитула Excel‑файла. |
| [setFooterMargin(double value)](#setFooterMargin-double-) | Представляет расстояние от нижней части страницы до нижнего колонтитула в сантиметрах. |
| [setFooterMarginInch(double value)](#setFooterMarginInch-double-) | Представляет расстояние от нижней части страницы до нижнего колонтитула в дюймах. |
| [setFooterPicture(int section, byte[] footerPicture)](#setFooterPicture-int-byte---) | Устанавливает изображение в нижний колонтитул листа. |
| [setHFAlignMargins(boolean value)](#setHFAlignMargins-boolean-) | Указывает, выравниваются ли поля верхнего и нижнего колонтитулов с полями страницы. |
| [setHFDiffFirst(boolean value)](#setHFDiffFirst-boolean-) | True означает, что верхний/нижний колонтитул первой страницы отличается от остальных страниц. |
| [setHFDiffOddEven(boolean value)](#setHFDiffOddEven-boolean-) | True означает, что верхний/нижний колонтитул нечётных страниц отличается от остальных нечётных страниц. |
| [setHFScaleWithDoc(boolean value)](#setHFScaleWithDoc-boolean-) | Указывает, масштабируются ли верхний и нижний колонтитулы вместе с масштабированием документа. |
| [setHeader(int section, String headerScript)](#setHeader-int-java.lang.String-) | Устанавливает скрипт форматирования верхнего колонтитула Excel‑файла. |
| [setHeaderMargin(double value)](#setHeaderMargin-double-) | Представляет расстояние от верхней части страницы до заголовка в сантиметрах. |
| [setHeaderMarginInch(double value)](#setHeaderMarginInch-double-) | Представляет расстояние от верхней части страницы до заголовка в дюймах. |
| [setHeaderPicture(int section, byte[] headerPicture)](#setHeaderPicture-int-byte---) | Устанавливает изображение в верхний колонтитул листа. |
| [setLeftMargin(double value)](#setLeftMargin-double-) | Представляет размер левого поля в сантиметрах. |
| [setLeftMarginInch(double value)](#setLeftMarginInch-double-) | Представляет размер левого поля в дюймах. |
| [setOrder(int value)](#setOrder-int-) | Представляет порядок, который Microsoft Excel использует для нумерации страниц при печати большого листа. |
| [setOrientation(int value)](#setOrientation-int-) | Представляет ориентацию печати страницы. |
| [setPaperSize(int value)](#setPaperSize-int-) | Представляет размер бумаги. |
| [setPercentScale(boolean value)](#setPercentScale-boolean-) | Если это свойство равно False, свойства FitToPagesWide и FitToPagesTall определяют, как масштабируется лист. |
| [setPicture(boolean isFirst, boolean isEven, boolean isHeader, int section, byte[] imageData)](#setPicture-boolean-boolean-boolean-int-byte---) | Устанавливает изображение в верхний/нижний колонтитул листа. |
| [setPrintArea(String value)](#setPrintArea-java.lang.String-) | Представляет диапазон для печати. |
| [setPrintComments(int value)](#setPrintComments-int-) | Представляет способ печати комментариев вместе с листом. |
| [setPrintCopies(int value)](#setPrintCopies-int-) | Устанавливает количество копий для печати. |
| [setPrintDraft(boolean value)](#setPrintDraft-boolean-) | Представляет, будет ли лист печататься без графики. |
| [setPrintErrors(int value)](#setPrintErrors-int-) | Указывает тип отображаемой ошибки печати. |
| [setPrintGridlines(boolean value)](#setPrintGridlines-boolean-) | Представляет, печатаются ли линии сетки ячеек на странице. |
| [setPrintHeadings(boolean value)](#setPrintHeadings-boolean-) | Представляет, печатаются ли заголовки строк и столбцов на этой странице. |
| [setPrintQuality(int value)](#setPrintQuality-int-) | Представляет качество печати. |
| [setPrintTitleColumns(String value)](#setPrintTitleColumns-java.lang.String-) | Представляет столбцы, содержащие ячейки, которые повторяются слева от каждой страницы. |
| [setPrintTitleRows(String value)](#setPrintTitleRows-java.lang.String-) | Представляет строки, содержащие ячейки, которые повторяются вверху каждой страницы. |
| [setPrinterSettings(byte[] value)](#setPrinterSettings-byte---) | Устанавливает параметры принтера по умолчанию. |
| [setRightMargin(double value)](#setRightMargin-double-) | Представляет размер правого поля в сантиметрах. |
| [setRightMarginInch(double value)](#setRightMarginInch-double-) | Представляет размер правого поля в дюймах. |
| [setTopMargin(double value)](#setTopMargin-double-) | Представляет размер верхнего поля в сантиметрах. |
| [setTopMarginInch(double value)](#setTopMarginInch-double-) | Представляет размер верхнего поля в дюймах. |
| [setZoom(int value)](#setZoom-int-) | Представляет коэффициент масштабирования в процентах. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### clearHeaderFooter() {#clearHeaderFooter--}
```
public void clearHeaderFooter()
```


Очищает настройки заголовка и нижнего колонтитула.

### copy(PageSetup source, CopyOptions copyOptions) {#copy-com.aspose.cells.PageSetup-com.aspose.cells.CopyOptions-}
```
public void copy(PageSetup source, CopyOptions copyOptions)
```


Копирует настройки page setup.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| source | [PageSetup](../../com.aspose.cells/pagesetup) | Источник. |
| copyOptions | [CopyOptions](../../com.aspose.cells/copyoptions) | Опции копирования. |

### customPaperSize(double width, double height) {#customPaperSize-double-double-}
```
public void customPaperSize(double width, double height)
```


Устанавливает пользовательский размер бумаги, в дюймах.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| width | double | Ширина бумаги. |
| height | double | Высота бумаги. |

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
### getBlackAndWhite() {#getBlackAndWhite--}
```
public boolean getBlackAndWhite()
```


Определяет, будут ли элементы документа печататься в чёрно‑белом виде.

**Returns:**
boolean
### getBottomMargin() {#getBottomMargin--}
```
public double getBottomMargin()
```


Определяет размер нижнего поля, в сантиметрах.

**Returns:**
double
### getBottomMarginInch() {#getBottomMarginInch--}
```
public double getBottomMarginInch()
```


Определяет размер нижнего поля, в дюймах.

**Returns:**
double
### getCenterHorizontally() {#getCenterHorizontally--}
```
public boolean getCenterHorizontally()
```


Определяет, печатается ли лист по горизонтали по центру.

**Returns:**
boolean
### getCenterVertically() {#getCenterVertically--}
```
public boolean getCenterVertically()
```


Определяет, печатается ли лист по вертикали по центру.

**Returns:**
boolean
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getCommands(String headerFooterScript) {#getCommands-java.lang.String-}
```
public HeaderFooterCommand[] getCommands(String headerFooterScript)
```


Получает все команды заголовка или нижнего колонтитула.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| headerFooterScript | java.lang.String | Скрипт верхнего/нижнего колонтитула |

**Returns:**
com.aspose.cells.HeaderFooterCommand[] - Возвращает все команды верхнего или нижнего колонтитула.
### getEvenFooter(int section) {#getEvenFooter-int-}
```
public String getEvenFooter(int section)
```


Получает скрипт, форматирующий четный нижний колонтитул Excel‑файла.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| section | int | 0: Левая секция, 1: Центральная секция, 2: Правая секция. |

**Returns:**
java.lang.String
### getEvenHeader(int section) {#getEvenHeader-int-}
```
public String getEvenHeader(int section)
```


Получает скрипт, форматирующий четный заголовок Excel‑файла.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| section | int | 0: Левая секция, 1: Центральная секция, 2: Правая секция. |

**Returns:**
java.lang.String
### getFirstPageFooter(int section) {#getFirstPageFooter-int-}
```
public String getFirstPageFooter(int section)
```


Получает скрипт, форматирующий нижний колонтитул первой страницы Excel‑файла.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| section | int | 0: Левая секция, 1: Центральная секция, 2: Правая секция. |

**Returns:**
java.lang.String
### getFirstPageHeader(int section) {#getFirstPageHeader-int-}
```
public String getFirstPageHeader(int section)
```


Получает скрипт, форматирующий заголовок первой страницы Excel‑файла.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| section | int | 0: Левая секция, 1: Центральная секция, 2: Правая секция. |

**Returns:**
java.lang.String
### getFirstPageNumber() {#getFirstPageNumber--}
```
public int getFirstPageNumber()
```


Представляет номер первой страницы, который будет использоваться при печати этого листа.

**Returns:**
int
### getFitToPagesTall() {#getFitToPagesTall--}
```
public int getFitToPagesTall()
```


Представляет количество страниц по высоте, до которого будет масштабироваться лист при печати. Значение по умолчанию — 1.

**Remarks**

Необходимо установить FitToPagesWide в ноль, если нужно разместить все строки на одной странице.

**Returns:**
int
### getFitToPagesWide() {#getFitToPagesWide--}
```
public int getFitToPagesWide()
```


Представляет количество страниц по ширине, до которого будет масштабироваться лист при печати. Значение по умолчанию — 1.

**Remarks**

Необходимо установить FitToPagesTall в ноль, если нужно разместить все столбцы на одной странице.

**Returns:**
int
### getFooter(int section) {#getFooter-int-}
```
public String getFooter(int section)
```


Получает скрипт, форматирующий нижний колонтитул Excel‑файла.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| section | int | 0: Левая секция, 1: Центральная секция, 2: Правая секция. |

**Returns:**
java.lang.String
### getFooterMargin() {#getFooterMargin--}
```
public double getFooterMargin()
```


Представляет расстояние от нижней части страницы до нижнего колонтитула в сантиметрах.

**Returns:**
double
### getFooterMarginInch() {#getFooterMarginInch--}
```
public double getFooterMarginInch()
```


Представляет расстояние от нижней части страницы до нижнего колонтитула в дюймах.

**Returns:**
double
### getHeader(int section) {#getHeader-int-}
```
public String getHeader(int section)
```


Получает скрипт, форматирующий заголовок Excel‑файла.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| section | int | 0: Левая секция, 1: Центральная секция, 2: Правая секция. |

**Returns:**
java.lang.String
### getHeaderMargin() {#getHeaderMargin--}
```
public double getHeaderMargin()
```


Представляет расстояние от верхней части страницы до заголовка в сантиметрах.

**Returns:**
double
### getHeaderMarginInch() {#getHeaderMarginInch--}
```
public double getHeaderMarginInch()
```


Представляет расстояние от верхней части страницы до заголовка в дюймах.

**Returns:**
double
### getLeftMargin() {#getLeftMargin--}
```
public double getLeftMargin()
```


Представляет размер левого поля в сантиметрах.

**Returns:**
double
### getLeftMarginInch() {#getLeftMarginInch--}
```
public double getLeftMarginInch()
```


Представляет размер левого поля в дюймах.

**Returns:**
double
### getODSPageBackground() {#getODSPageBackground--}
```
public OdsPageBackground getODSPageBackground()
```


Получает фон ODS.

**Returns:**
[OdsPageBackground](../../com.aspose.cells/odspagebackground)
### getOrder() {#getOrder--}
```
public int getOrder()
```


Представляет порядок, который Microsoft Excel использует для нумерации страниц при печати большого листа.

См. [PrintOrderType](../../com.aspose.cells/printordertype).

**Returns:**
int
### getOrientation() {#getOrientation--}
```
public int getOrientation()
```


Представляет ориентацию печати страницы.

См. [PageOrientationType](../../com.aspose.cells/pageorientationtype).

**Returns:**
int
### getPaperHeight() {#getPaperHeight--}
```
public double getPaperHeight()
```


Получает высоту бумаги в дюймах, учитывая ориентацию страницы.

**Returns:**
double
### getPaperSize() {#getPaperSize--}
```
public int getPaperSize()
```


Представляет размер бумаги.

Смотрите [PaperSizeType](../../com.aspose.cells/papersizetype).

**Returns:**
int
### getPaperWidth() {#getPaperWidth--}
```
public double getPaperWidth()
```


Получает ширину бумаги в дюймах, учитывая ориентацию страницы.

**Returns:**
double
### getPicture(boolean isFirst, boolean isEven, boolean isHeader, int section) {#getPicture-boolean-boolean-boolean-int-}
```
public Picture getPicture(boolean isFirst, boolean isEven, boolean isHeader, int section)
```


Получает объект [Picture](../../com.aspose.cells/picture) заголовка / нижнего колонтитула.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| isFirst | boolean | Указывает, получено ли изображение верхнего/нижнего колонтитула первой страницы. |
| isEven | boolean | Указывает, получено ли изображение верхнего/нижнего колонтитула чётной страницы. |
| isHeader | boolean | Указывает, получено ли изображение верхнего/нижнего колонтитула. |
| section | int | 0: Левая секция, 1: Центральная секция, 2: Правая секция. |

**Returns:**
[Picture](../../com.aspose.cells/picture) - Returns [Picture](../../com.aspose.cells/picture) object.
### getPicture(boolean isHeader, int section) {#getPicture-boolean-int-}
```
public Picture getPicture(boolean isHeader, int section)
```


Получает объект [Picture](../../com.aspose.cells/picture) заголовка / нижнего колонтитула.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| isHeader | boolean | Указывает, находится ли он в верхнем или нижнем колонтитуле. |
| section | int | 0: Левая секция, 1: Центральная секция, 2: Правая секция. |

**Returns:**
[Picture](../../com.aspose.cells/picture) - Returns [Picture](../../com.aspose.cells/picture) object. Returns null if there is no picture.
### getPrintArea() {#getPrintArea--}
```
public String getPrintArea()
```


Представляет диапазон для печати.

**Returns:**
java.lang.String
### getPrintComments() {#getPrintComments--}
```
public int getPrintComments()
```


Представляет способ печати комментариев вместе с листом.

Смотрите [PrintCommentsType](../../com.aspose.cells/printcommentstype).

**Returns:**
int
### getPrintCopies() {#getPrintCopies--}
```
public int getPrintCopies()
```


Получает количество копий для печати.

**Returns:**
int
### getPrintDraft() {#getPrintDraft--}
```
public boolean getPrintDraft()
```


Представляет, будет ли лист печататься без графики.

**Returns:**
boolean
### getPrintErrors() {#getPrintErrors--}
```
public int getPrintErrors()
```


Указывает тип отображаемой ошибки печати.

Смотрите [PrintErrorsType](../../com.aspose.cells/printerrorstype).

**Returns:**
int
### getPrintGridlines() {#getPrintGridlines--}
```
public boolean getPrintGridlines()
```


Представляет, печатаются ли линии сетки ячеек на странице.

**Returns:**
boolean
### getPrintHeadings() {#getPrintHeadings--}
```
public boolean getPrintHeadings()
```


Представляет, печатаются ли заголовки строк и столбцов на этой странице.

**Returns:**
boolean
### getPrintQuality() {#getPrintQuality--}
```
public int getPrintQuality()
```


Представляет качество печати.

**Returns:**
int
### getPrintTitleColumns() {#getPrintTitleColumns--}
```
public String getPrintTitleColumns()
```


Представляет столбцы, содержащие ячейки, которые повторяются слева от каждой страницы.

**Example**

```
         pageSetup.setPrintTitleColumns("$A:$A");
```

**Returns:**
java.lang.String
### getPrintTitleRows() {#getPrintTitleRows--}
```
public String getPrintTitleRows()
```


Представляет строки, содержащие ячейки, которые повторяются вверху каждой страницы.

**Example**

```
         pageSetup.setPrintTitleRows("$1:$1");
```

**Returns:**
java.lang.String
### getPrinterSettings() {#getPrinterSettings--}
```
public byte[] getPrinterSettings()
```


Получает настройки принтера по умолчанию.

**Returns:**
byte[]
### getRightMargin() {#getRightMargin--}
```
public double getRightMargin()
```


Представляет размер правого поля в сантиметрах.

**Returns:**
double
### getRightMarginInch() {#getRightMarginInch--}
```
public double getRightMarginInch()
```


Представляет размер правого поля в дюймах.

**Returns:**
double
### getTopMargin() {#getTopMargin--}
```
public double getTopMargin()
```


Представляет размер верхнего поля в сантиметрах.

**Returns:**
double
### getTopMarginInch() {#getTopMarginInch--}
```
public double getTopMarginInch()
```


Представляет размер верхнего поля в дюймах.

**Returns:**
double
### getZoom() {#getZoom--}
```
public int getZoom()
```


Представляет коэффициент масштабирования в процентах. Должен быть в диапазоне от 10 до 400.

**Returns:**
int
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isAutoFirstPageNumber() {#isAutoFirstPageNumber--}
```
public boolean isAutoFirstPageNumber()
```


Указывает, назначается ли номер первой страницы автоматически.

**Returns:**
boolean
### isAutomaticPaperSize() {#isAutomaticPaperSize--}
```
public boolean isAutomaticPaperSize()
```


Указывает, является ли размер бумаги автоматическим.

**Returns:**
boolean
### isHFAlignMargins() {#isHFAlignMargins--}
```
public boolean isHFAlignMargins()
```


Указывает, выравниваются ли поля верхнего и нижнего колонтитулов с полями страницы. Если это свойство true, левый верхний и нижний колонтитул будет выравнен с левым полем, а правый — с правым полем. Эта опция включена по умолчанию.

**Returns:**
boolean
### isHFDiffFirst() {#isHFDiffFirst--}
```
public boolean isHFDiffFirst()
```


True означает, что верхний/нижний колонтитул первой страницы отличается от остальных страниц.

**Returns:**
boolean
### isHFDiffOddEven() {#isHFDiffOddEven--}
```
public boolean isHFDiffOddEven()
```


True означает, что верхний/нижний колонтитул нечётных страниц отличается от остальных нечётных страниц.

**Returns:**
boolean
### isHFScaleWithDoc() {#isHFScaleWithDoc--}
```
public boolean isHFScaleWithDoc()
```


Указывает, масштабируются ли верхний и нижний колонтитулы вместе с масштабированием документа. Применяется только к Excel 2007.

**Returns:**
boolean
### isPercentScale() {#isPercentScale--}
```
public boolean isPercentScale()
```


Если это свойство равно False, свойства FitToPagesWide и FitToPagesTall определяют, как масштабируется лист.

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




### setAutoFirstPageNumber(boolean value) {#setAutoFirstPageNumber-boolean-}
```
public void setAutoFirstPageNumber(boolean value)
```


Указывает, назначается ли номер первой страницы автоматически.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setBlackAndWhite(boolean value) {#setBlackAndWhite-boolean-}
```
public void setBlackAndWhite(boolean value)
```


Определяет, будут ли элементы документа печататься в чёрно‑белом виде.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setBottomMargin(double value) {#setBottomMargin-double-}
```
public void setBottomMargin(double value)
```


Определяет размер нижнего поля, в сантиметрах.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | double |  |

### setBottomMarginInch(double value) {#setBottomMarginInch-double-}
```
public void setBottomMarginInch(double value)
```


Определяет размер нижнего поля, в дюймах.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | double |  |

### setCenterHorizontally(boolean value) {#setCenterHorizontally-boolean-}
```
public void setCenterHorizontally(boolean value)
```


Определяет, печатается ли лист по горизонтали по центру.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setCenterVertically(boolean value) {#setCenterVertically-boolean-}
```
public void setCenterVertically(boolean value)
```


Определяет, печатается ли лист по вертикали по центру.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setEvenFooter(int section, String footerScript) {#setEvenFooter-int-java.lang.String-}
```
public void setEvenFooter(int section, String footerScript)
```


Устанавливает скрипт форматирования нижнего колонтитула чётных страниц Excel‑файла. Действует только в Excel 2007, когда IsHFDiffOddEven равно true.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| section | int | 0: Левая секция, 1: Центральная секция, 2: Правая секция. |
| footerScript | java.lang.String | Скрипт форматирования нижнего колонтитула. |

### setEvenHeader(int section, String headerScript) {#setEvenHeader-int-java.lang.String-}
```
public void setEvenHeader(int section, String headerScript)
```


Устанавливает скрипт форматирования верхнего колонтитула чётных страниц Excel‑файла. Действует только в Excel 2007, когда IsHFDiffOddEven равно true.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| section | int | 0: Левая секция, 1: Центральная секция, 2: Правая секция. |
| headerScript | java.lang.String | Скрипт форматирования верхнего колонтитула. |

### setFirstPageFooter(int section, String footerScript) {#setFirstPageFooter-int-java.lang.String-}
```
public void setFirstPageFooter(int section, String footerScript)
```


Задает скрипт форматирования нижнего колонтитула первой страницы Excel‑файла.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| section | int | 0: Левая секция, 1: Центральная секция, 2: Правая секция. |
| footerScript | java.lang.String | Скрипт форматирования нижнего колонтитула. |

### setFirstPageHeader(int section, String headerScript) {#setFirstPageHeader-int-java.lang.String-}
```
public void setFirstPageHeader(int section, String headerScript)
```


Устанавливает скрипт форматирования верхнего колонтитула первой страницы Excel‑файла. Действует только в Excel 2007, когда IsHFDiffFirst равно true.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| section | int | 0: Левая секция, 1: Центральная секция, 2: Правая секция. |
| headerScript | java.lang.String | Скрипт форматирования верхнего колонтитула. |

### setFirstPageNumber(int value) {#setFirstPageNumber-int-}
```
public void setFirstPageNumber(int value)
```


Представляет номер первой страницы, который будет использоваться при печати этого листа.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setFitToPages(int wide, int tall) {#setFitToPages-int-int-}
```
public void setFitToPages(int wide, int tall)
```


Задает количество страниц, до которых будет масштабироваться лист при печати.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| wide | int | Страниц по ширине. |
| tall | int | Страниц по высоте. |

### setFitToPagesTall(int value) {#setFitToPagesTall-int-}
```
public void setFitToPagesTall(int value)
```


Представляет количество страниц по высоте, до которого будет масштабироваться лист при печати. Значение по умолчанию — 1.

**Remarks**

Необходимо установить FitToPagesWide в ноль, если нужно разместить все строки на одной странице.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setFitToPagesWide(int value) {#setFitToPagesWide-int-}
```
public void setFitToPagesWide(int value)
```


Представляет количество страниц по ширине, до которого будет масштабироваться лист при печати. Значение по умолчанию — 1.

**Remarks**

Необходимо установить FitToPagesTall в ноль, если нужно разместить все столбцы на одной странице.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setFooter(int section, String footerScript) {#setFooter-int-java.lang.String-}
```
public void setFooter(int section, String footerScript)
```


Устанавливает скрипт форматирования нижнего колонтитула Excel‑файла.

**Remarks**

Команды скрипта:

| Команда | Описание |
| -------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------- |
| &P | Текущий номер страницы\\u9286\\u20ac |
| &N | Количество страниц\\u9286\\u20ac |
| &D | Текущая дата\\u9286\\u20ac |
| &T | Текущее время |
| &A | Имя листа |
| &F | Имя файла без пути |
| &"<FontName>" | Имя шрифта, например: &\"Arial\" |
| &"<FontName>, <FontStyle>" | Имя шрифта и стиль шрифта, например: &\"Arial,Bold\" |
| &<FontSize> | Размер шрифта. Если эта команда сопровождается простым числом, которое будет напечатано в заголовке, оно будет отделено от высоты шрифта пробелом. |
| &K<RRGGBB> | Цвет шрифта, например (RED): &KFF0000 |
| &G | Скрипт изображения |

Например: \"&Arial,Bold&8Footer Note\"

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| section | int | 0: Левая секция, 1: Центральная секция, 2: Правая секция. |
| footerScript | java.lang.String | Скрипт форматирования нижнего колонтитула. |

### setFooterMargin(double value) {#setFooterMargin-double-}
```
public void setFooterMargin(double value)
```


Представляет расстояние от нижней части страницы до нижнего колонтитула в сантиметрах.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | double |  |

### setFooterMarginInch(double value) {#setFooterMarginInch-double-}
```
public void setFooterMarginInch(double value)
```


Представляет расстояние от нижней части страницы до нижнего колонтитула в дюймах.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | double |  |

### setFooterPicture(int section, byte[] footerPicture) {#setFooterPicture-int-byte---}
```
public Picture setFooterPicture(int section, byte[] footerPicture)
```


Устанавливает изображение в нижний колонтитул листа.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| section | int | 0: Левая секция, 1: Центральная секция, 2: Правая секция. |
| footerPicture | byte[] | Данные изображения. |

**Returns:**
[Picture](../../com.aspose.cells/picture) - Returns [Picture](../../com.aspose.cells/picture) object.
### setHFAlignMargins(boolean value) {#setHFAlignMargins-boolean-}
```
public void setHFAlignMargins(boolean value)
```


Указывает, выравниваются ли поля верхнего и нижнего колонтитулов с полями страницы. Если это свойство true, левый верхний и нижний колонтитул будет выравнен с левым полем, а правый — с правым полем. Эта опция включена по умолчанию.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setHFDiffFirst(boolean value) {#setHFDiffFirst-boolean-}
```
public void setHFDiffFirst(boolean value)
```


True означает, что верхний/нижний колонтитул первой страницы отличается от остальных страниц.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setHFDiffOddEven(boolean value) {#setHFDiffOddEven-boolean-}
```
public void setHFDiffOddEven(boolean value)
```


True означает, что верхний/нижний колонтитул нечётных страниц отличается от остальных нечётных страниц.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setHFScaleWithDoc(boolean value) {#setHFScaleWithDoc-boolean-}
```
public void setHFScaleWithDoc(boolean value)
```


Указывает, масштабируются ли верхний и нижний колонтитулы вместе с масштабированием документа. Применяется только к Excel 2007.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setHeader(int section, String headerScript) {#setHeader-int-java.lang.String-}
```
public void setHeader(int section, String headerScript)
```


Устанавливает скрипт форматирования верхнего колонтитула Excel‑файла.

**Remarks**

Команды скрипта:

| Команда | Описание |
| -------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------- |
| &P | Текущий номер страницы\\u9286\\u20ac |
| &N | Количество страниц\\u9286\\u20ac |
| &D | Текущая дата\\u9286\\u20ac |
| &T | Текущее время |
| &A | Имя листа |
| &F | Имя файла без пути |
| &"<FontName>" | Имя шрифта, например: &\"Arial\" |
| &"<FontName>, <FontStyle>" | Имя шрифта и стиль шрифта, например: &\"Arial,Bold\" |
| &<FontSize> | Размер шрифта. Если эта команда сопровождается простым числом, которое будет напечатано в заголовке, оно будет отделено от высоты шрифта пробелом. |
| &K<RRGGBB> | Цвет шрифта, например (RED): &KFF0000 |
| &G | Скрипт изображения |

Например: \"&Arial,Bold&8Header Note\"

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| section | int | 0: Левая секция, 1: Центральная секция, 2: Правая секция. |
| headerScript | java.lang.String | Скрипт форматирования верхнего колонтитула. |

### setHeaderMargin(double value) {#setHeaderMargin-double-}
```
public void setHeaderMargin(double value)
```


Представляет расстояние от верхней части страницы до заголовка в сантиметрах.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | double |  |

### setHeaderMarginInch(double value) {#setHeaderMarginInch-double-}
```
public void setHeaderMarginInch(double value)
```


Представляет расстояние от верхней части страницы до заголовка в дюймах.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | double |  |

### setHeaderPicture(int section, byte[] headerPicture) {#setHeaderPicture-int-byte---}
```
public Picture setHeaderPicture(int section, byte[] headerPicture)
```


Устанавливает изображение в верхний колонтитул листа.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| section | int | 0: Левая секция, 1: Центральная секция, 2: Правая секция. |
| headerPicture | byte[] | Данные изображения. |

**Returns:**
[Picture](../../com.aspose.cells/picture) - Returns [Picture](../../com.aspose.cells/picture) object.
### setLeftMargin(double value) {#setLeftMargin-double-}
```
public void setLeftMargin(double value)
```


Представляет размер левого поля в сантиметрах.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | double |  |

### setLeftMarginInch(double value) {#setLeftMarginInch-double-}
```
public void setLeftMarginInch(double value)
```


Представляет размер левого поля в дюймах.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | double |  |

### setOrder(int value) {#setOrder-int-}
```
public void setOrder(int value)
```


Представляет порядок, который Microsoft Excel использует для нумерации страниц при печати большого листа.

См. [PrintOrderType](../../com.aspose.cells/printordertype).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setOrientation(int value) {#setOrientation-int-}
```
public void setOrientation(int value)
```


Представляет ориентацию печати страницы.

См. [PageOrientationType](../../com.aspose.cells/pageorientationtype).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setPaperSize(int value) {#setPaperSize-int-}
```
public void setPaperSize(int value)
```


Представляет размер бумаги.

Смотрите [PaperSizeType](../../com.aspose.cells/papersizetype).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setPercentScale(boolean value) {#setPercentScale-boolean-}
```
public void setPercentScale(boolean value)
```


Если это свойство равно False, свойства FitToPagesWide и FitToPagesTall определяют, как масштабируется лист.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setPicture(boolean isFirst, boolean isEven, boolean isHeader, int section, byte[] imageData) {#setPicture-boolean-boolean-boolean-int-byte---}
```
public Picture setPicture(boolean isFirst, boolean isEven, boolean isHeader, int section, byte[] imageData)
```


Устанавливает изображение в верхний/нижний колонтитул листа.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| isFirst | boolean | Указывает, устанавливается ли изображение в заголовке/нижнем колонтитуле первой страницы. |
| isEven | boolean | Указывает, устанавливается ли изображение в заголовке/нижнем колонтитуле четных страниц. |
| isHeader | boolean | Указывает, устанавливается ли изображение в заголовке/нижнем колонтитуле. |
| section | int | 0: Левая секция, 1: Центральная секция, 2: Правая секция. |
| imageData | byte[] | Данные изображения. |

**Returns:**
[Picture](../../com.aspose.cells/picture) - Returns [Picture](../../com.aspose.cells/picture) object.
### setPrintArea(String value) {#setPrintArea-java.lang.String-}
```
public void setPrintArea(String value)
```


Представляет диапазон для печати.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### setPrintComments(int value) {#setPrintComments-int-}
```
public void setPrintComments(int value)
```


Представляет способ печати комментариев вместе с листом.

Смотрите [PrintCommentsType](../../com.aspose.cells/printcommentstype).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setPrintCopies(int value) {#setPrintCopies-int-}
```
public void setPrintCopies(int value)
```


Устанавливает количество копий для печати.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setPrintDraft(boolean value) {#setPrintDraft-boolean-}
```
public void setPrintDraft(boolean value)
```


Представляет, будет ли лист печататься без графики.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setPrintErrors(int value) {#setPrintErrors-int-}
```
public void setPrintErrors(int value)
```


Указывает тип отображаемой ошибки печати.

Смотрите [PrintErrorsType](../../com.aspose.cells/printerrorstype).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setPrintGridlines(boolean value) {#setPrintGridlines-boolean-}
```
public void setPrintGridlines(boolean value)
```


Представляет, печатаются ли линии сетки ячеек на странице.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setPrintHeadings(boolean value) {#setPrintHeadings-boolean-}
```
public void setPrintHeadings(boolean value)
```


Представляет, печатаются ли заголовки строк и столбцов на этой странице.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setPrintQuality(int value) {#setPrintQuality-int-}
```
public void setPrintQuality(int value)
```


Представляет качество печати.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setPrintTitleColumns(String value) {#setPrintTitleColumns-java.lang.String-}
```
public void setPrintTitleColumns(String value)
```


Представляет столбцы, содержащие ячейки, которые повторяются слева от каждой страницы.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### setPrintTitleRows(String value) {#setPrintTitleRows-java.lang.String-}
```
public void setPrintTitleRows(String value)
```


Представляет строки, содержащие ячейки, которые повторяются вверху каждой страницы.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### setPrinterSettings(byte[] value) {#setPrinterSettings-byte---}
```
public void setPrinterSettings(byte[] value)
```


Устанавливает параметры принтера по умолчанию.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | byte[] |  |

### setRightMargin(double value) {#setRightMargin-double-}
```
public void setRightMargin(double value)
```


Представляет размер правого поля в сантиметрах.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | double |  |

### setRightMarginInch(double value) {#setRightMarginInch-double-}
```
public void setRightMarginInch(double value)
```


Представляет размер правого поля в дюймах.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | double |  |

### setTopMargin(double value) {#setTopMargin-double-}
```
public void setTopMargin(double value)
```


Представляет размер верхнего поля в сантиметрах.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | double |  |

### setTopMarginInch(double value) {#setTopMarginInch-double-}
```
public void setTopMarginInch(double value)
```


Представляет размер верхнего поля в дюймах.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | double |  |

### setZoom(int value) {#setZoom-int-}
```
public void setZoom(int value)
```


Представляет коэффициент масштабирования в процентах. Должен быть в диапазоне от 10 до 400.

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

