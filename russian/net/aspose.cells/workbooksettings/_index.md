---
title: WorkbookSettings
second_title: Справочник по Aspose.Cells для .NET API
description: Представляет все настройки книги.
type: docs
weight: 6500
url: /ru/net/aspose.cells/workbooksettings/
---
## WorkbookSettings class

Представляет все настройки книги.

```csharp
public class WorkbookSettings : IDisposable
```

## Характеристики

| Имя | Описание |
| --- | --- |
| [Author](../../aspose.cells/workbooksettings/author) { get; set; } | Получает и устанавливает автора файла. |
| [AutoCompressPictures](../../aspose.cells/workbooksettings/autocompresspictures) { get; set; } | Указывает логическое значение, указывающее, что приложение автоматически сжимает изображения в книге. |
| [AutoRecover](../../aspose.cells/workbooksettings/autorecover) { get; set; } | Указывает, помечен ли файл для автоматического восстановления. |
| [BuildVersion](../../aspose.cells/workbooksettings/buildversion) { get; set; } | Указывает добавочную общедоступную версию приложения. |
| [CheckCompatibility](../../aspose.cells/workbooksettings/checkcompatibility) { get; set; } | Указывает, следует ли проверять совместимость с более ранними версиями при сохранении книги. |
| [CheckCustomNumberFormat](../../aspose.cells/workbooksettings/checkcustomnumberformat) { get; set; } | Указывает, проверяется ли проверка пользовательского числового формата при установке Style.Custom. |
| [CheckExcelRestriction](../../aspose.cells/workbooksettings/checkexcelrestriction) { get; set; } | Проверять ли ограничение файла excel, когда пользователь изменяет объекты, связанные с ячейками. Например, Excel не позволяет вводить строковое значение длиннее 32 КБ. Когда вы вводите значение длиннее 32 КБ, например Cell.PutValue(string), если это свойство истинно, вы получите исключение. Если это свойство имеет значение false, мы примем введенное вами строковое значение в качестве значения ячейки, чтобы позже вы могли вывести полное строковое значение для других форматов файлов, таких как CSV. Однако, если вы установили такое значение, которое недопустимо для формата файла Excel, вам не следует сохранять книгу в формате файла Excel позже. В противном случае может возникнуть непредвиденная ошибка для сгенерированного файла Excel. |
| [Compliance](../../aspose.cells/workbooksettings/compliance) { get; set; } | Указывает версию OOXML для выходного документа. Значение по умолчанию — Ecma376_2006. |
| [CrashSave](../../aspose.cells/workbooksettings/crashsave) { get; set; } | указывает, сохраняло ли приложение последний раз файл рабочей книги после сбоя. |
| [CultureInfo](../../aspose.cells/workbooksettings/cultureinfo) { get; set; } | Получает или задает информацию о культуре системы. |
| [DataExtractLoad](../../aspose.cells/workbooksettings/dataextractload) { get; set; } | указывает, открывало ли приложение последнюю книгу для восстановления данных. |
| [Date1904](../../aspose.cells/workbooksettings/date1904) { get; set; } | Получает или задает значение, указывающее, используется ли в книге система дат 1904 года. |
| [DisplayDrawingObjects](../../aspose.cells/workbooksettings/displaydrawingobjects) { get; set; } | Указывает, следует ли и как отображать объекты в рабочей книге. |
| [EnableMacros](../../aspose.cells/workbooksettings/enablemacros) { get; set; } | Включить макросы; |
| [FirstVisibleTab](../../aspose.cells/workbooksettings/firstvisibletab) { get; set; } | Получает или задает первую видимую вкладку рабочего листа. |
| [FormulaSettings](../../aspose.cells/workbooksettings/formulasettings) { get; } | Получает настройки функций, связанных с формулой. |
| [GlobalizationSettings](../../aspose.cells/workbooksettings/globalizationsettings) { get; set; } | Получает и задает параметры глобализации. |
| [HidePivotFieldList](../../aspose.cells/workbooksettings/hidepivotfieldlist) { get; set; } | Получает и задает, следует ли скрыть список полей для сводной таблицы. |
| [IsDefaultEncrypted](../../aspose.cells/workbooksettings/isdefaultencrypted) { get; set; } | Указывает, следует ли шифровать книгу с паролем по умолчанию, если структура и окна книги заблокированы. |
| [IsEncrypted](../../aspose.cells/workbooksettings/isencrypted) { get; } | Получает значение, указывающее, требуется ли пароль для открытия этой книги. |
| [IsHidden](../../aspose.cells/workbooksettings/ishidden) { get; set; } | Указывает, скрыта ли эта книга. |
| [IsHScrollBarVisible](../../aspose.cells/workbooksettings/ishscrollbarvisible) { get; set; } | Получает или задает значение, указывающее, будет ли сгенерированная электронная таблица содержать горизонтальную полосу прокрутки. |
| [IsMinimized](../../aspose.cells/workbooksettings/isminimized) { get; set; } | Указывает, будет ли сгенерированная электронная таблица открыта в свернутом виде. |
| [IsProtected](../../aspose.cells/workbooksettings/isprotected) { get; } | Получает значение, указывающее, защищена ли структура или окно книги. |
| [IsVScrollBarVisible](../../aspose.cells/workbooksettings/isvscrollbarvisible) { get; set; } | Получает или задает значение, указывающее, будет ли сгенерированная электронная таблица содержать вертикальную полосу прокрутки. |
| [LanguageCode](../../aspose.cells/workbooksettings/languagecode) { get; set; } | Получает или задает язык пользовательского интерфейса версии книги на основе CountryCode, в котором сохранен файл. |
| [MaxColumn](../../aspose.cells/workbooksettings/maxcolumn) { get; } | Получает максимальный индекс столбца, отсчитываемый от нуля. |
| [MaxRow](../../aspose.cells/workbooksettings/maxrow) { get; } | Получает максимальный индекс строки, отсчитываемый от нуля. |
| [MaxRowsOfSharedFormula](../../aspose.cells/workbooksettings/maxrowsofsharedformula) { get; set; } | Получает и задает максимальное количество строк общей формулы. |
| [MemorySetting](../../aspose.cells/workbooksettings/memorysetting) { get; set; } | Получает или задает параметры использования памяти. Новый параметр будет использоваться по умолчанию для вновь созданных рабочих листов, но не будет действовать для существующих рабочих листов. |
| [NumberDecimalSeparator](../../aspose.cells/workbooksettings/numberdecimalseparator) { get; set; } | Получает или задает десятичный разделитель для форматирования/анализа числовых значений. По умолчанию используется десятичный разделитель текущего региона. |
| [NumberGroupSeparator](../../aspose.cells/workbooksettings/numbergroupseparator) { get; set; } | Получает или задает символ, разделяющий группы цифр слева от десятичной дроби в числовых значениях. По умолчанию используется разделитель групп текущего региона. |
| [PaperSize](../../aspose.cells/workbooksettings/papersize) { get; set; } | Получает и задает размер бумаги для печати по умолчанию. |
| [Password](../../aspose.cells/workbooksettings/password) { get; set; } | Представляет пароль для шифрования файла рабочей книги. |
| [ProtectionType](../../aspose.cells/workbooksettings/protectiontype) { get; } | Получает тип защиты книги. |
| [QuotePrefixToStyle](../../aspose.cells/workbooksettings/quoteprefixtostyle) { get; set; } | Указывает, будет ли установка свойства[`QuotePrefix`](../style/quoteprefix)при вводе строкового значения (которое начинается с одинарной кавычки) ячейка |
| [Region](../../aspose.cells/workbooksettings/region) { get; set; } | Получает или задает региональные настройки для книги. |
| [RemovePersonalInformation](../../aspose.cells/workbooksettings/removepersonalinformation) { get; set; } | Истинно, если личную информацию можно удалить из указанной книги. |
| [RepairLoad](../../aspose.cells/workbooksettings/repairload) { get; set; } | Указывает, открывало ли приложение последний раз книгу в безопасном режиме или в режиме восстановления. |
| [ResourceProvider](../../aspose.cells/workbooksettings/resourceprovider) { get; set; } | Получает и задает поставщика потока для внешнего ресурса, например, для загрузки данных изображения для изображения типа "LinkToFile". |
| [Shared](../../aspose.cells/workbooksettings/shared) { get; set; } | Получает или задает значение, указывающее, является ли рабочая книга общей. |
| [SheetTabBarWidth](../../aspose.cells/workbooksettings/sheettabbarwidth) { get; set; } | Ширина панели вкладок рабочего листа (в 1/1000 ширины окна). |
| [ShowTabs](../../aspose.cells/workbooksettings/showtabs) { get; set; } | Получите или задайте значение, указывающее, отображаются ли вкладки рабочей книги. |
| [SignificantDigits](../../aspose.cells/workbooksettings/significantdigits) { get; set; } | Получает и устанавливает количество значащих цифр. Значение по умолчанию:[`SignificantDigits`](../cellshelper/significantdigits). |
| [UpdateAdjacentCellsBorder](../../aspose.cells/workbooksettings/updateadjacentcellsborder) { get; set; } | Указывает, обновлять ли границу соседних ячеек. |
| [UpdateLinksType](../../aspose.cells/workbooksettings/updatelinkstype) { get; set; } | Получает и задает способ обновления внешних ссылок при открытии книги. |
| [WarningCallback](../../aspose.cells/workbooksettings/warningcallback) { get; set; } | Получает или устанавливает обратный вызов предупреждения. |
| [WindowHeight](../../aspose.cells/workbooksettings/windowheight) { get; set; } | Высота окна в пунктах. |
| [WindowHeightCM](../../aspose.cells/workbooksettings/windowheightcm) { get; set; } | Высота окна в сантиметрах. |
| [WindowHeightInch](../../aspose.cells/workbooksettings/windowheightinch) { get; set; } | Высота окна в дюймах. |
| [WindowLeft](../../aspose.cells/workbooksettings/windowleft) { get; set; } | Расстояние от левого края клиентской области до левого края окна в пунктах. |
| [WindowLeftCM](../../aspose.cells/workbooksettings/windowleftcm) { get; set; } | Расстояние от левого края клиентской области до левого края окна. В сантиметрах. |
| [WindowLeftInch](../../aspose.cells/workbooksettings/windowleftinch) { get; set; } | Расстояние от левого края клиентской области до левого края окна. В дюймах. |
| [WindowTop](../../aspose.cells/workbooksettings/windowtop) { get; set; } | Расстояние от верхнего края клиентской области до верхнего края окна в пунктах. |
| [WindowTopCM](../../aspose.cells/workbooksettings/windowtopcm) { get; set; } | Расстояние от верхнего края клиентской области до верхнего края окна в сантиметрах. |
| [WindowTopInch](../../aspose.cells/workbooksettings/windowtopinch) { get; set; } | Расстояние от верхнего края клиентской области до верхнего края окна в дюймах. |
| [WindowWidth](../../aspose.cells/workbooksettings/windowwidth) { get; set; } | Ширина окна в пунктах. |
| [WindowWidthCM](../../aspose.cells/workbooksettings/windowwidthcm) { get; set; } | Ширина окна в сантиметрах. |
| [WindowWidthInch](../../aspose.cells/workbooksettings/windowwidthinch) { get; set; } | Ширина окна в дюймах. |
| [WriteProtection](../../aspose.cells/workbooksettings/writeprotection) { get; } | Предоставляет доступ к параметрам защиты книги от записи. |

## Методы

| Имя | Описание |
| --- | --- |
| [Dispose](../../aspose.cells/workbooksettings/dispose)() | Освобождает ресурсы. |
| [GetThemeFont](../../aspose.cells/workbooksettings/getthemefont)(FontSchemeType) | Получает имя шрифта темы по умолчанию. |
| [SetPageOrientationType](../../aspose.cells/workbooksettings/setpageorientationtype)(PageOrientationType) | Установить тип ориентации печати для всей книги. |

### Примеры

```csharp
[C#]

Workbook workbook = new Workbook();

WorkbookSettings settings = workbook.Settings;

  //делай свое дело

[Visual Basic]
Dim workbook as Workbook = new Workbook()

Dim settings as WorkbookSettings = workbook.Settings

'делай свое дело
```

### Смотрите также

* пространство имен [Aspose.Cells](../../aspose.cells)
* сборка [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
