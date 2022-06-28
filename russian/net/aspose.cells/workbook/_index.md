---
title: Workbook
second_title: Справочник по Aspose.Cells для .NET API
description: Представляет корневой объект для создания электронной таблицы Excel.
type: docs
weight: 6480
url: /ru/net/aspose.cells/workbook/
---
## Workbook class

Представляет корневой объект для создания электронной таблицы Excel.

```csharp
public class Workbook : IDisposable
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [Workbook](workbook#constructor)() | Инициализирует новый экземпляр класса[`Workbook`](../workbook). |
| [Workbook](workbook#constructor_1)(FileFormatType) | Инициализирует новый экземпляр класса[`Workbook`](../workbook). |
| [Workbook](workbook#constructor_2)(Stream) | Инициализирует новый экземпляр класса[`Workbook`](../workbook)и открывает поток. |
| [Workbook](workbook#constructor_4)(string) | Инициализирует новый экземпляр класса[`Workbook`](../workbook)и открывает файл. |
| [Workbook](workbook#constructor_3)(Stream, LoadOptions) | Инициализирует новый экземпляр класса[`Workbook`](../workbook)и открытый поток. |
| [Workbook](workbook#constructor_5)(string, LoadOptions) | Инициализирует новый экземпляр класса[`Workbook`](../workbook)и открывает файл. |

## Характеристики

| Имя | Описание |
| --- | --- |
| [AbsolutePath](../../aspose.cells/workbook/absolutepath) { get; set; } | Получает и задает абсолютный путь к файлу. |
| [BuiltInDocumentProperties](../../aspose.cells/workbook/builtindocumentproperties) { get; } | Возвращает коллекцию[`DocumentProperty`](../../aspose.cells.properties/documentproperty), которая представляет все встроенные свойства документа электронной таблицы. |
| [CellsDataTableFactory](../../aspose.cells/workbook/cellsdatatablefactory) { get; } | Получает фабрику для построения ICellsDataTable из пользовательских объектов |
| [Colors](../../aspose.cells/workbook/colors) { get; } | Возвращает цвета в палитре электронной таблицы. |
| [ContentTypeProperties](../../aspose.cells/workbook/contenttypeproperties) { get; } | Получает список объектов[`ContentTypeProperty`](../../aspose.cells.properties/contenttypeproperty)в книге. |
| [CountOfStylesInPool](../../aspose.cells/workbook/countofstylesinpool) { get; } | Получает количество стилей в пуле стилей. |
| [CustomDocumentProperties](../../aspose.cells/workbook/customdocumentproperties) { get; } | Возвращает коллекцию[`DocumentProperty`](../../aspose.cells.properties/documentproperty), которая представляет все настраиваемые свойства документа электронной таблицы. |
| [CustomXmlParts](../../aspose.cells/workbook/customxmlparts) { get; } | Представляет пользовательскую часть хранения данных XML (пользовательские данные XML в пакете). |
| [DataConnections](../../aspose.cells/workbook/dataconnections) { get; } | Получает коллекцию[`ExternalConnection`](../../aspose.cells.externalconnections/externalconnection). |
| [DataMashup](../../aspose.cells/workbook/datamashup) { get; } | Получает данные мэшапа. |
| [DataSorter](../../aspose.cells/workbook/datasorter) { get; } | Получает объект DataSorter для сортировки данных. |
| [DefaultStyle](../../aspose.cells/workbook/defaultstyle) { get; set; } | Получает или задает объект по умолчанию[`Style`](../style)рабочей книги. |
| [FileFormat](../../aspose.cells/workbook/fileformat) { get; set; } | Получает и задает формат файла. |
| [FileName](../../aspose.cells/workbook/filename) { get; set; } | Получает и устанавливает текущее имя файла. |
| [HasMacro](../../aspose.cells/workbook/hasmacro) { get; } | Указывает, содержит ли эта электронная таблица макрос/VBA. |
| [HasRevisions](../../aspose.cells/workbook/hasrevisions) { get; } | Получает, есть ли в книге какие-либо отслеживаемые изменения |
| [InterruptMonitor](../../aspose.cells/workbook/interruptmonitor) { get; set; } | Получает и устанавливает монитор прерываний. |
| [IsDigitallySigned](../../aspose.cells/workbook/isdigitallysigned) { get; } | Указывает, имеет ли эта электронная таблица цифровую подпись. |
| [IsLicensed](../../aspose.cells/workbook/islicensed) { get; } | Указывает, установлена ли лицензия. |
| [IsWorkbookProtectedWithPassword](../../aspose.cells/workbook/isworkbookprotectedwithpassword) { get; } | Указывает, защищены ли структура или окно паролем. |
| [RibbonXml](../../aspose.cells/workbook/ribbonxml) { get; set; } | Получает и задает XML-файл, определяющий пользовательский интерфейс ленты. |
| [Settings](../../aspose.cells/workbook/settings) { get; } | Представляет параметры книги. |
| [Theme](../../aspose.cells/workbook/theme) { get; } | Получает имя темы. |
| [VbaProject](../../aspose.cells/workbook/vbaproject) { get; } | Получает[`VbaProject`](./vbaproject)в электронной таблице. |
| [Worksheets](../../aspose.cells/workbook/worksheets) { get; } | Получает коллекцию[`WorksheetCollection`](../worksheetcollection)в электронной таблице. |

## Методы

| Имя | Описание |
| --- | --- |
| [AcceptAllRevisions](../../aspose.cells/workbook/acceptallrevisions)() | Принимает все отслеживаемые изменения в книге. |
| [AddDigitalSignature](../../aspose.cells/workbook/adddigitalsignature)(DigitalSignatureCollection) | Добавляет цифровую подпись к файлу электронной таблицы OOXML (Excel2007 и более поздние версии). |
| [CalculateFormula](../../aspose.cells/workbook/calculateformula#calculateformula)() | Вычисляет результат формул. |
| [CalculateFormula](../../aspose.cells/workbook/calculateformula#calculateformula_2)(bool) | Вычисляет результат формул. |
| [CalculateFormula](../../aspose.cells/workbook/calculateformula#calculateformula_1)(CalculationOptions) | Вычисление формул в этой книге. |
| [ChangePalette](../../aspose.cells/workbook/changepalette)(Color, int) | Изменяет палитру электронной таблицы в указанном индексе. |
| [CloseAccessCache](../../aspose.cells/workbook/closeaccesscache)(AccessCacheOptions) | Закрывает сеанс, который использует кэши для доступа к данным. |
| [Combine](../../aspose.cells/workbook/combine)(Workbook) | Объединяет другой объект Workbook. |
| [Copy](../../aspose.cells/workbook/copy#copy)(Workbook) | Копирует данные из исходного объекта Workbook. |
| [Copy](../../aspose.cells/workbook/copy#copy_1)(Workbook, CopyOptions) | Копирует данные из исходного объекта Workbook. |
| [CopyTheme](../../aspose.cells/workbook/copytheme)(Workbook) | Копирует тему из другой книги. |
| [CreateBuiltinStyle](../../aspose.cells/workbook/createbuiltinstyle)(BuiltinStyleType) | Создает встроенный стиль по заданному типу. |
| [CreateCellsColor](../../aspose.cells/workbook/createcellscolor)() | Создает объект[`CellsColor`](../cellscolor). |
| [CreateStyle](../../aspose.cells/workbook/createstyle)() | Создает новый стиль. |
| [CustomTheme](../../aspose.cells/workbook/customtheme)(string, Color[]) | Пользовательская тема. |
| [Dispose](../../aspose.cells/workbook/dispose)() | Выполняет определяемые приложением задачи, связанные с освобождением, освобождением или сбросом неуправляемых ресурсов. |
| [ExportXml](../../aspose.cells/workbook/exportxml#exportxml)(string, Stream) | Экспорт XML-данных. |
| [ExportXml](../../aspose.cells/workbook/exportxml#exportxml_1)(string, string) | Экспорт данных XML, связанных указанной картой XML. |
| [GetDigitalSignature](../../aspose.cells/workbook/getdigitalsignature)() | Получает цифровую подпись из файла. |
| [GetFonts](../../aspose.cells/workbook/getfonts)() | Получает все шрифты в пуле стилей. |
| [GetMatchingColor](../../aspose.cells/workbook/getmatchingcolor)(Color) | Найти наиболее подходящий цвет в текущей палитре. |
| [GetNamedStyle](../../aspose.cells/workbook/getnamedstyle)(string) | Получает именованный стиль в пуле стилей. |
| [GetStyleInPool](../../aspose.cells/workbook/getstyleinpool)(int) | Получает стиль из пула стилей. Все стили в книге будут собраны в пул. В ячейках есть только простой ссылочный индекс. |
| [GetThemeColor](../../aspose.cells/workbook/getthemecolor)(ThemeColorType) | Получает цвет темы. |
| [ImportXml](../../aspose.cells/workbook/importxml#importxml)(Stream, string, int, int) | Импортирует/обновляет файл данных XML в книгу. |
| [ImportXml](../../aspose.cells/workbook/importxml#importxml_1)(string, string, int, int) | Импортирует/обновляет файл данных XML в книгу. |
| [IsColorInPalette](../../aspose.cells/workbook/iscolorinpalette)(Color) | Проверяет наличие цвета в палитре электронной таблицы. |
| [ParseFormulas](../../aspose.cells/workbook/parseformulas)(bool) | Разбирает все формулы, которые не были проанализированы, когда они были загружены из файла шаблона или установлены в ячейку. |
| [Protect](../../aspose.cells/workbook/protect)(ProtectionType, string) | Защищает рабочую книгу. |
| [ProtectSharedWorkbook](../../aspose.cells/workbook/protectsharedworkbook)(string) | Защищает общую книгу. |
| [RefreshDynamicArrayFormulas](../../aspose.cells/workbook/refreshdynamicarrayformulas)(bool) | Обновляет формулы динамического массива (переливается в новый диапазон соседних ячеек в соответствии с текущими данными) |
| [RemoveDigitalSignature](../../aspose.cells/workbook/removedigitalsignature)() | Удаляет цифровую подпись из этой электронной таблицы. |
| [RemoveMacro](../../aspose.cells/workbook/removemacro)() | Удаляет VBA/макрос из этой электронной таблицы. |
| [RemovePersonalInformation](../../aspose.cells/workbook/removepersonalinformation)() | Удаляет личную информацию. |
| [RemoveUnusedStyles](../../aspose.cells/workbook/removeunusedstyles)() | Удалите все неиспользуемые стили. |
| [Replace](../../aspose.cells/workbook/replace#replace)(bool, object) | Заменяет значения ячеек новыми данными. |
| [Replace](../../aspose.cells/workbook/replace#replace_1)(int, object) | Заменяет значения ячеек новыми данными. |
| [Replace](../../aspose.cells/workbook/replace#replace_6)(string, DataTable) | Заменяет значения ячеек данными из таблицыDataTable. |
| [Replace](../../aspose.cells/workbook/replace#replace_2)(string, double) | Заменяет значение ячейки новым двойным значением. |
| [Replace](../../aspose.cells/workbook/replace#replace_4)(string, int) | Заменяет значение ячейки новым целым числом. |
| [Replace](../../aspose.cells/workbook/replace#replace_7)(string, string) | Заменяет значение ячейки новой строкой. |
| [Replace](../../aspose.cells/workbook/replace#replace_3)(string, double[], bool) | Заменяет значения ячеек двойным массивом. |
| [Replace](../../aspose.cells/workbook/replace#replace_5)(string, int[], bool) | Заменяет значения ячеек целочисленным массивом. |
| [Replace](../../aspose.cells/workbook/replace#replace_8)(string, string, ReplaceOptions) | Заменяет значение ячейки новой строкой. |
| [Replace](../../aspose.cells/workbook/replace#replace_9)(string, string[], bool) | Заменяет значение ячейки новым массивом строк. |
| [Save](../../aspose.cells/workbook/save#save_2)(string) | Сохраните книгу на диск. |
| [Save](../../aspose.cells/workbook/save#save)(Stream, SaveFormat) | Сохраняет книгу в потоке. |
| [Save](../../aspose.cells/workbook/save#save_1)(Stream, SaveOptions) | Сохраняет книгу в потоке. |
| [Save](../../aspose.cells/workbook/save#save_3)(string, SaveFormat) | Сохраняет книгу на диск. |
| [Save](../../aspose.cells/workbook/save#save_4)(string, SaveOptions) | Сохраняет книгу на диск. |
| [Save](../../aspose.cells/workbook/save#save_5)(HttpResponse, string, ContentDisposition, SaveOptions) | Создает электронную таблицу результатов и передает ее клиенту, а затем открывает в браузере или MS Workbook. |
| [Save](../../aspose.cells/workbook/save#save_6)(HttpResponse, string, ContentDisposition, SaveOptions, bool) | Создает электронную таблицу результатов и передает ее клиенту, а затем открывает в браузере или MS Workbook. |
| [SaveToStream](../../aspose.cells/workbook/savetostream)() | Сохраняет файл Excel в объект MemoryStream и возвращает его. |
| [SetDigitalSignature](../../aspose.cells/workbook/setdigitalsignature)(DigitalSignatureCollection) | Устанавливает цифровую подпись для файла электронной таблицы (Excel2007 и более поздние версии). |
| [SetEncryptionOptions](../../aspose.cells/workbook/setencryptionoptions)(EncryptionType, int) | Установить параметры шифрования. |
| [SetThemeColor](../../aspose.cells/workbook/setthemecolor)(ThemeColorType, Color) | Устанавливает цвет темы |
| [StartAccessCache](../../aspose.cells/workbook/startaccesscache)(AccessCacheOptions) | Запускает сеанс, использующий кэши для доступа к данным. |
| [Unprotect](../../aspose.cells/workbook/unprotect)(string) | Снимает защиту с книги. |
| [UnprotectSharedWorkbook](../../aspose.cells/workbook/unprotectsharedworkbook)(string) | Снимает защиту с общей книги. |
| [UpdateLinkedDataSource](../../aspose.cells/workbook/updatelinkeddatasource)(Workbook[]) | Если эта книга содержит внешние ссылки на другой источник данных, Aspose.Cells попытается получить последние данные. |

### Примечания

Класс Workbook обозначает электронную таблицу Excel. Каждая электронная таблица может содержать несколько рабочих листов. Основной функцией класса является открытие и сохранение исходных файлов Excel. Класс имеет некоторые дополнительные функции, такие как копирование данных из других рабочих книг, объединение двух рабочих книг и защита электронной таблицы Excel.

### Примеры

В следующем примере рабочая книга загружается из файла с именем Designer.xls и выполняется горизонтальная и вертикальная прокрутка. полосы, невидимые для Рабочей тетради. Затем он заменяет два строковых значения целочисленным значением и строковым значением соответственно в электронной таблице и, наконец, отправляет обновленный файл в клиентский браузер.

```csharp
[C#]

  //Открываем конструктор file
string designerFile = "designer.xls";
Workbook workbook = new Workbook(designerFile);

  //Установить полосы прокрутки
workbook.Settings.IsHScrollBarVisible = false;
workbook.Settings.IsVScrollBarVisible = false;

  //Замените строку-заполнитель новыми значениями
int newInt = 100;
workbook.Replace("OldInt", newInt);

string newString = "Hello!";
workbook.Replace("OldString", newString);
workbook.Save("result.xls");

[Visual Basic]

'Открываем конструктор file
Dim designerFile as String = "\designer.xls"
Dim workbook as Workbook = new Workbook(designerFile)

'Установить полосы прокрутки
workbook.IsHScrollBarVisible = False
workbook.IsVScrollBarVisible = False

'Замените строку-заполнитель новыми значениями
Dim newInt as Integer = 100
workbook.Replace("OldInt", newInt)

Dim newString as String = "Hello!"
workbook.Replace("OldString", newString)
workbook.Save("result.xls")    
```

### Смотрите также

* пространство имен [Aspose.Cells](../../aspose.cells)
* сборка [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
