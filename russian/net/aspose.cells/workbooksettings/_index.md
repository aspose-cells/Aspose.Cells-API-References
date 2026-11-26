---
title: "Класс WorkbookSettings"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.WorkbookSettings. Представляет все настройки рабочей книги"
type: docs
url: /ru/net/aspose.cells/workbooksettings/
---
## WorkbookSettings class

Представляет все настройки книги.

```csharp
public class WorkbookSettings : IDisposable
```

## Свойства

| Имя | Описание |
| --- | --- |
| [Author](../../aspose.cells/workbooksettings/author/) { get; set; } | Получает и задаёт автора файла. |
| [AutoCompressPictures](../../aspose.cells/workbooksettings/autocompresspictures/) { get; set; } | Указывает логическое значение, которое определяет, автоматически сжимает ли приложение изображения в рабочей книге. |
| [AutoRecover](../../aspose.cells/workbooksettings/autorecover/) { get; set; } | Указывает, помечен ли файл для автоматического восстановления. |
| [BuildVersion](../../aspose.cells/workbooksettings/buildversion/) { get; set; } | Указывает инкрементальный публичный релиз приложения. |
| [CheckCompatibility](../../aspose.cells/workbooksettings/checkcompatibility/) { get; set; } | Указывает, проверять ли совместимость с более ранними версиями при сохранении рабочей книги. |
| [CheckCustomNumberFormat](../../aspose.cells/workbooksettings/checkcustomnumberformat/) { get; set; } | Указывает, проверять ли пользовательский числовой формат при установке Style.Custom. |
| [CheckExcelRestriction](../../aspose.cells/workbooksettings/checkexcelrestriction/) { get; set; } | Проверять ли ограничения файла Excel, когда пользователь изменяет связанные с ячейками объекты. Например, Excel не позволяет вводить строковое значение длиной более 32 КБ. Когда вы вводите значение длиннее 32 КБ, например через Cell.PutValue(string), если это свойство равно true, вы получите исключение. Если свойство равно false, мы примем введённую строку как значение ячейки, чтобы позже вы могли вывести полное строковое значение в другие форматы файлов, такие как CSV. Однако, если вы задали значение, недопустимое для формата файла Excel, позже не следует сохранять рабочую книгу в формате Excel. В противном случае может возникнуть непредвиденная ошибка в сгенерированном файле Excel. |
| [Compliance](../../aspose.cells/workbooksettings/compliance/) { get; set; } | Указывает версию OOXML для выходного документа. Значение по умолчанию — Ecma376_2006. |
| [CrashSave](../../aspose.cells/workbooksettings/crashsave/) { get; set; } | Указывает, сохранял ли приложение файл рабочей книги после сбоя. |
| [CultureInfo](../../aspose.cells/workbooksettings/cultureinfo/) { get; set; } | Получает или задает информацию о системной культуре. |
| [DataExtractLoad](../../aspose.cells/workbooksettings/dataextractload/) { get; set; } | Указывает, открыл ли приложение рабочую книгу для восстановления данных в последний раз. |
| [Date1904](../../aspose.cells/workbooksettings/date1904/) { get; set; } | Получает или задает значение, указывающее, использует ли рабочая книга систему дат 1904 года. |
| [DefaultImageResolution](../../aspose.cells/workbooksettings/defaultimageresolution/) { get; set; } | Получает и задает разрешение изображения по умолчанию. |
| [DefaultStyleSettings](../../aspose.cells/workbooksettings/defaultstylesettings/) { get; } | Получает настройки значений по умолчанию свойств, связанных со стилем, для этой рабочей книги. |
| [DiscardImageEditData](../../aspose.cells/workbooksettings/discardimageeditdata/) { get; set; } | Указывает, отбрасывать ли редактируемые данные изображения. |
| [DisplayDrawingObjects](../../aspose.cells/workbooksettings/displaydrawingobjects/) { get; set; } | Указывает, показывать ли объекты в рабочей книге и как их отображать. |
| [EnableMacros](../../aspose.cells/workbooksettings/enablemacros/) { get; set; } | Включить макросы; |
| [FirstVisibleTab](../../aspose.cells/workbooksettings/firstvisibletab/) { get; set; } | Получает или задает первую видимую вкладку листа. |
| [FormulaSettings](../../aspose.cells/workbooksettings/formulasettings/) { get; } | Получает настройки функций, связанных с формулами. |
| [GlobalizationSettings](../../aspose.cells/workbooksettings/globalizationsettings/) { get; set; } | Получает и задает параметры глобализации. |
| [HidePivotFieldList](../../aspose.cells/workbooksettings/hidepivotfieldlist/) { get; set; } | Получает и задает, скрывать ли список полей для сводной таблицы. |
| [IsDefaultEncrypted](../../aspose.cells/workbooksettings/isdefaultencrypted/) { get; set; } | Указывает, шифровать ли рабочую книгу паролем по умолчанию, если структура и окна рабочей книги заблокированы. |
| [IsEncrypted](../../aspose.cells/workbooksettings/isencrypted/) { get; } | Получает значение, указывающее, требуется ли пароль для открытия этой рабочей книги. |
| [IsHidden](../../aspose.cells/workbooksettings/ishidden/) { get; set; } | Указывает, скрыта ли эта рабочая книга. |
| [IsHScrollBarVisible](../../aspose.cells/workbooksettings/ishscrollbarvisible/) { get; set; } | Получает или задает значение, указывающее, будет ли у сгенерированной таблицы горизонтальная полоса прокрутки. |
| [IsMinimized](../../aspose.cells/workbooksettings/isminimized/) { get; set; } | Отражает, будет ли сгенерированная таблица открыта в свернутом виде. |
| [IsProtected](../../aspose.cells/workbooksettings/isprotected/) { get; } | Получает значение, указывающее, защищены ли структура или окно рабочей книги. |
| [IsVScrollBarVisible](../../aspose.cells/workbooksettings/isvscrollbarvisible/) { get; set; } | Получает или задает значение, указывающее, будет ли сгенерированная таблица содержать вертикальную полосу прокрутки. |
| [LanguageCode](../../aspose.cells/workbooksettings/languagecode/) { get; set; } | Получает или задает язык пользовательского интерфейса версии Workbook, основанный на CountryCode, который сохранил файл. |
| [MaxColumn](../../aspose.cells/workbooksettings/maxcolumn/) { get; } | Получает максимальный индекс столбца, начиная с нуля. |
| [MaxRow](../../aspose.cells/workbooksettings/maxrow/) { get; } | Получает максимальный индекс строки, начиная с нуля. |
| [MaxRowsOfSharedFormula](../../aspose.cells/workbooksettings/maxrowsofsharedformula/) { get; set; } | Получает и задает максимальный номер строки общей формулы. |
| [MaxUniqueItemsPerField](../../aspose.cells/workbooksettings/maxuniqueitemsperfield/) { get; set; } | Получает и задает ограничение уникальных элементов на поле |
| [MemorySetting](../../aspose.cells/workbooksettings/memorysetting/) { get; set; } | Получает или задает параметры использования памяти. Новый параметр будет использоваться как параметр по умолчанию для только что созданных листов, но не будет применяться к существующим листам. |
| [NumberDecimalSeparator](../../aspose.cells/workbooksettings/numberdecimalseparator/) { get; set; } | Получает или задает десятичный разделитель для форматирования/парсинга числовых значений. По умолчанию используется десятичный разделитель текущего региона. |
| [NumberGroupSeparator](../../aspose.cells/workbooksettings/numbergroupseparator/) { get; set; } | Получает или задает символ, разделяющий группы цифр слева от десятичного разделителя в числовых значениях. По умолчанию используется разделитель групп текущего региона. |
| [PaperSize](../../aspose.cells/workbooksettings/papersize/) { get; set; } | Получает и задает размер бумаги по умолчанию для печати. |
| [Password](../../aspose.cells/workbooksettings/password/) { get; set; } | Представляет пароль шифрования файла Workbook. |
| [PropertiesFollowChartPoint](../../aspose.cells/workbooksettings/propertiesfollowchartpoint/) { get; set; } | Указывает, следуют ли свойства точек данных и подписи данных во всех диаграммах этой книги их ссылкам. |
| [ProtectionType](../../aspose.cells/workbooksettings/protectiontype/) { get; } | Получает тип защиты книги. |
| [QuotePrefixToStyle](../../aspose.cells/workbooksettings/quoteprefixtostyle/) { get; set; } | Указывает, будет ли установлено свойство [`QuotePrefix`](../style/quoteprefix/) при вводе строкового значения (которое начинается с одинарной кавычки) в ячейку |
| [Region](../../aspose.cells/workbooksettings/region/) { get; set; } | Получает или задает региональные настройки для книги. |
| [RemovePersonalInformation](../../aspose.cells/workbooksettings/removepersonalinformation/) { get; set; } | Истина, если из указанной книги можно удалить персональные данные. |
| [RepairLoad](../../aspose.cells/workbooksettings/repairload/) { get; set; } | Указывает, открыла ли приложение книгу в безопасном или режиме восстановления в последний раз. |
| [ResourceProvider](../../aspose.cells/workbooksettings/resourceprovider/) { get; set; } | Получает и задает поставщика потоков для внешних ресурсов, например загрузку данных изображения для картинки типа "LinkToFile". |
| [ShapeDisplayType](../../aspose.cells/workbooksettings/shapedisplaytype/) { get; set; } | Получает и задает способ отображения фигур приложением в этой книге |
| [Shared](../../aspose.cells/workbooksettings/shared/) { get; set; } | Получает или задает значение, указывающее, является ли книга общей. |
| [SheetTabBarWidth](../../aspose.cells/workbooksettings/sheettabbarwidth/) { get; set; } | Ширина панели вкладок листа (в 1/1000 ширины окна). |
| [ShowTabs](../../aspose.cells/workbooksettings/showtabs/) { get; set; } | Получает или задает значение, отображаются ли вкладки книги. |
| [SignificantDigits](../../aspose.cells/workbooksettings/significantdigits/) { get; set; } | (**Obsolete.**) Получает и задает количество значимых цифр. Значение по умолчанию — [`SignificantDigits`](../cellshelper/significantdigits/). |
| [SignificantDigitsType](../../aspose.cells/workbooksettings/significantdigitstype/) { get; set; } | Получает и задает тип значимых цифр для вывода числовых значений в этой книге. Значение по умолчанию — [`SignificantDigitsType`](../cellshelper/significantdigitstype/). |
| [SmartTagOptions](../../aspose.cells/workbooksettings/smarttagoptions/) { get; } | Получает параметры смарт-тега. |
| [StreamProvider](../../aspose.cells/workbooksettings/streamprovider/) { get; set; } | (**Obsolete.**) Получает и задает поставщика потока для внешнего ресурса. |
| [UpdateAdjacentCellsBorder](../../aspose.cells/workbooksettings/updateadjacentcellsborder/) { get; set; } | Указывает, следует ли обновлять границу соседних ячеек. |
| [UpdateLinksType](../../aspose.cells/workbooksettings/updatelinkstype/) { get; set; } | Получает и задает, как обновлять внешние ссылки при открытии книги. |
| [WarningCallback](../../aspose.cells/workbooksettings/warningcallback/) { get; set; } | Получает или задаёт обратный вызов предупреждения. |
| [WindowHeight](../../aspose.cells/workbooksettings/windowheight/) { get; set; } | Высота окна в пунктах. |
| [WindowHeightCM](../../aspose.cells/workbooksettings/windowheightcm/) { get; set; } | Высота окна в сантиметрах. |
| [WindowHeightInch](../../aspose.cells/workbooksettings/windowheightinch/) { get; set; } | Высота окна в дюймах. |
| [WindowLeft](../../aspose.cells/workbooksettings/windowleft/) { get; set; } | Расстояние от левого края клиентской области до левого края окна в пунктах. |
| [WindowLeftCM](../../aspose.cells/workbooksettings/windowleftcm/) { get; set; } | Расстояние от левого края клиентской области до левого края окна в сантиметрах. |
| [WindowLeftInch](../../aspose.cells/workbooksettings/windowleftinch/) { get; set; } | Расстояние от левого края клиентской области до левого края окна в дюймах. |
| [WindowTop](../../aspose.cells/workbooksettings/windowtop/) { get; set; } | Расстояние от верхнего края клиентской области до верхнего края окна в пунктах. |
| [WindowTopCM](../../aspose.cells/workbooksettings/windowtopcm/) { get; set; } | Расстояние от верхнего края клиентской области до верхнего края окна в сантиметрах. |
| [WindowTopInch](../../aspose.cells/workbooksettings/windowtopinch/) { get; set; } | Расстояние от верхнего края клиентской области до верхнего края окна в дюймах. |
| [WindowWidth](../../aspose.cells/workbooksettings/windowwidth/) { get; set; } | Ширина окна в пунктах. |
| [WindowWidthCM](../../aspose.cells/workbooksettings/windowwidthcm/) { get; set; } | Ширина окна в сантиметрах. |
| [WindowWidthInch](../../aspose.cells/workbooksettings/windowwidthinch/) { get; set; } | Ширина окна в дюймах. |
| [WpsCompatibility](../../aspose.cells/workbooksettings/wpscompatibility/) { get; set; } | Указывает, следует ли быть совместимым с WPS. |
| [WriteProtection](../../aspose.cells/workbooksettings/writeprotection/) { get; } | Предоставляет доступ к параметрам защиты книги от записи. |

## Методы

| Имя | Описание |
| --- | --- |
| [Dispose](../../aspose.cells/workbooksettings/dispose/)() | Освобождает ресурсы. |
| [GetThemeFont](../../aspose.cells/workbooksettings/getthemefont/)(FontSchemeType) | Получает имя шрифта темы по умолчанию. |
| [SetPageOrientationType](../../aspose.cells/workbooksettings/setpageorientationtype/)(PageOrientationType) | Устанавливает тип ориентации печати для всей книги. |

### Примеры

```csharp
using Aspose.Cells;
using System;
using System.Globalization;

public class WorkbookSettingsDemo
{
    public static void RunDemo()
    {
        // Создать новую книгу
        Workbook workbook = new Workbook();
        Worksheet sheet = workbook.Worksheets[0];

        // Добавьте некоторые образцы данных.
        sheet.Cells["A1"].PutValue("Sample Data");
        sheet.Cells["A2"].PutValue(123);
        sheet.Cells["A3"].PutValue(DateTime.Now);

        // Доступ к WorkbookSettings
        WorkbookSettings settings = workbook.Settings;

        // Установить различные параметры
        settings.Author = "John Doe";
        settings.CheckCustomNumberFormat = true;
        settings.EnableMacros = false;
        settings.Date1904 = false;
        settings.DisplayDrawingObjects = DisplayDrawingObjects.DisplayShapes;
        settings.SheetTabBarWidth = 1000;
        settings.ShowTabs = true;
        settings.FirstVisibleTab = 0;
        settings.IsHScrollBarVisible = true;
        settings.IsVScrollBarVisible = true;
        settings.Shared = false;
        settings.LanguageCode = CountryCode.USA;
        settings.Region = CountryCode.USA;
        settings.CultureInfo = new CultureInfo("en-US");
        settings.GlobalizationSettings = new GlobalizationSettings();
        settings.NumberDecimalSeparator = '.';
        settings.NumberGroupSeparator = ',';
        settings.Password = "password123";
        settings.IsDefaultEncrypted = false;
        settings.IsMinimized = false;
        settings.IsHidden = false;
        settings.AutoCompressPictures = true;
        settings.RemovePersonalInformation = false;
        settings.HidePivotFieldList = false;
        settings.UpdateLinksType = UpdateLinksType.UserSet;
        settings.WindowLeft = 0;
        settings.WindowLeftInch = 0;
        settings.WindowLeftCM = 0;
        settings.WindowTop = 0;
        settings.WindowTopInch = 0;
        settings.WindowTopCM = 0;
        settings.WindowWidth = 800;
        settings.WindowWidthInch = 8;
        settings.WindowWidthCM = 20.32;
        settings.WindowHeight = 600;
        settings.WindowHeightInch = 6;
        settings.WindowHeightCM = 15.24;
        settings.UpdateAdjacentCellsBorder = true;
        settings.SignificantDigits = 15;
        settings.CheckCompatibility = true;
        settings.CheckExcelRestriction = true;
        settings.AutoRecover = true;
        settings.CrashSave = false;
        settings.DataExtractLoad = false;
        settings.RepairLoad = false;
        settings.BuildVersion = "1.0.0";
        settings.MemorySetting = MemorySetting.Normal;
        settings.PaperSize = PaperSizeType.PaperA4;
        settings.WarningCallback = null;
        settings.MaxRowsOfSharedFormula = 1048576;
        settings.Compliance = OoxmlCompliance.Ecma376_2006;
        settings.QuotePrefixToStyle = false;

        // Сохраните книгу
        workbook.Save("WorkbookSettingsDemo.xlsx");
    }
}
```

### См. также

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


