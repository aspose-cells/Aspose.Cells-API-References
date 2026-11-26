---
title: "Класс Workbook"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.Workbook. Представляет корневой объект для создания электронной таблицы Excel"
type: docs
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
| [Workbook](workbook/#constructor)() | Инициализирует новый экземпляр класса `Workbook`. |
| [Workbook](workbook/#constructor_1)(FileFormatType) | Инициализирует новый экземпляр класса `Workbook`. |
| [Workbook](workbook/#constructor_2)(LoadOptions) | Инициализирует новый пустой экземпляр класса `Workbook` с параметрами |
| [Workbook](workbook/#constructor_3)(Stream) | Инициализирует новый экземпляр класса `Workbook` и открывает поток. |
| [Workbook](workbook/#constructor_5)(string) | Инициализирует новый экземпляр класса `Workbook` и открывает файл. |
| [Workbook](workbook/#constructor_4)(Stream, LoadOptions) | Инициализирует новый экземпляр класса `Workbook` и открывает поток. |
| [Workbook](workbook/#constructor_6)(string, LoadOptions) | Инициализирует новый экземпляр класса `Workbook` и открывает файл. |

## Свойства

| Имя | Описание |
| --- | --- |
| [AbsolutePath](../../aspose.cells/workbook/absolutepath/) { get; set; } | Получает и задает абсолютный путь к файлу. |
| [BuiltInDocumentProperties](../../aspose.cells/workbook/builtindocumentproperties/) { get; } | Возвращает коллекцию [`DocumentProperty`](../../aspose.cells.properties/documentproperty/), представляющую все встроенные свойства документа таблицы. |
| [CellsDataTableFactory](../../aspose.cells/workbook/cellsdatatablefactory/) { get; } | Получает фабрику для создания ICellsDataTable из пользовательских объектов |
| [Colors](../../aspose.cells/workbook/colors/) { get; } | Возвращает цвета в палитре для электронной таблицы. |
| [ContentTypeProperties](../../aspose.cells/workbook/contenttypeproperties/) { get; } | Получает список объектов [`ContentTypeProperty`](../../aspose.cells.properties/contenttypeproperty/) в рабочей книге. |
| [CountOfStylesInPool](../../aspose.cells/workbook/countofstylesinpool/) { get; } | Получает количество стилей в пуле стилей. |
| [CustomDocumentProperties](../../aspose.cells/workbook/customdocumentproperties/) { get; } | Возвращает коллекцию [`DocumentProperty`](../../aspose.cells.properties/documentproperty/), представляющую все пользовательские свойства документа таблицы. |
| [CustomXmlParts](../../aspose.cells/workbook/customxmlparts/) { get; } | Представляет часть хранилища пользовательского XML-данных (пользовательские XML‑данные внутри пакета). |
| [DataConnections](../../aspose.cells/workbook/dataconnections/) { get; } | Получает коллекцию [`ExternalConnection`](../../aspose.cells.externalconnections/externalconnection/). |
| [DataMashup](../../aspose.cells/workbook/datamashup/) { get; } | Получает данные mashup. |
| [DataModel](../../aspose.cells/workbook/datamodel/) { get; } | Получает модель данных в рабочей книге. |
| [DataSorter](../../aspose.cells/workbook/datasorter/) { get; } | Получает объект DataSorter для сортировки данных. |
| [DefaultStyle](../../aspose.cells/workbook/defaultstyle/) { get; set; } | Получает или задает объект по умолчанию [`Style`](../style/) рабочей книги. |
| [FileFormat](../../aspose.cells/workbook/fileformat/) { get; set; } | Получает и задает формат файла. |
| [FileName](../../aspose.cells/workbook/filename/) { get; set; } | Получает и задает текущее имя файла. |
| [HasCustomFunction](../../aspose.cells/workbook/hascustomfunction/) { get; } | Определяет, используется ли в этой рабочей книге пользовательская функция, например в формулах ячеек, в определённых именах... |
| [HasMacro](../../aspose.cells/workbook/hasmacro/) { get; } | Указывает, содержит ли эта электронная таблица макросы/VBA. |
| [HasRevisions](../../aspose.cells/workbook/hasrevisions/) { get; } | Получает, есть ли в рабочей книге отслеживаемые изменения |
| [InterruptMonitor](../../aspose.cells/workbook/interruptmonitor/) { get; set; } | Получает и задает монитор прерываний. |
| [IsDigitallySigned](../../aspose.cells/workbook/isdigitallysigned/) { get; } | Указывает, подписана ли эта электронная таблица цифровой подписью. |
| [IsLicensed](../../aspose.cells/workbook/islicensed/) { get; } | Указывает, установлен ли лицензионный ключ. |
| [IsWorkbookProtectedWithPassword](../../aspose.cells/workbook/isworkbookprotectedwithpassword/) { get; } | Указывает, защищены ли структура или окно паролем. |
| [RibbonXml](../../aspose.cells/workbook/ribbonxml/) { get; set; } | Получает и задает XML‑файл, определяющий интерфейс Ribbon. |
| [Settings](../../aspose.cells/workbook/settings/) { get; } | Представляет настройки рабочей книги. |
| [Theme](../../aspose.cells/workbook/theme/) { get; } | Получает название темы. |
| [VbaProject](../../aspose.cells/workbook/vbaproject/) { get; } | Получает [`VbaProject`](./vbaproject/) в электронной таблице. |
| [Worksheets](../../aspose.cells/workbook/worksheets/) { get; } | Получает коллекцию [`WorksheetCollection`](../worksheetcollection/) в электронной таблице. |

## Методы

| Имя | Описание |
| --- | --- |
| [AcceptAllRevisions](../../aspose.cells/workbook/acceptallrevisions/)() | Принимает все отслеживаемые изменения в рабочей книге. |
| [AddDigitalSignature](../../aspose.cells/workbook/adddigitalsignature/)(DigitalSignatureCollection) | Добавляет цифровую подпись в файл электронных таблиц OOXML (Excel2007 и новее). |
| [CalculateFormula](../../aspose.cells/workbook/calculateformula/#calculateformula)() | Вычисляет результат формул. |
| [CalculateFormula](../../aspose.cells/workbook/calculateformula/#calculateformula_2)(bool) | Вычисляет результат формул. |
| [CalculateFormula](../../aspose.cells/workbook/calculateformula/#calculateformula_1)(CalculationOptions) | Вычисление формул в этой рабочей книге. |
| [ChangePalette](../../aspose.cells/workbook/changepalette/)(Color, int) | Изменяет палитру электронных таблиц в указанном индексе. |
| [CloseAccessCache](../../aspose.cells/workbook/closeaccesscache/)(AccessCacheOptions) | Закрывает сеанс, использующий кэши для доступа к данным. |
| [Combine](../../aspose.cells/workbook/combine/)(Workbook) | Объединяет другой объект Workbook. |
| [Copy](../../aspose.cells/workbook/copy/#copy)(Workbook) | Копирует данные из исходного объекта Workbook. |
| [Copy](../../aspose.cells/workbook/copy/#copy_1)(Workbook, CopyOptions) | Копирует другой объект Workbook. |
| [CopyTheme](../../aspose.cells/workbook/copytheme/)(Workbook) | Копирует тему из другой рабочей книги. |
| [CreateBuiltinStyle](../../aspose.cells/workbook/createbuiltinstyle/)(BuiltinStyleType) | Создаёт встроенный стиль заданного типа. |
| [CreateCellsColor](../../aspose.cells/workbook/createcellscolor/)() | Создаёт объект [`CellsColor`](../cellscolor/). |
| [CreateStyle](../../aspose.cells/workbook/createstyle/#createstyle)() | Создаёт новый стиль. |
| [CreateStyle](../../aspose.cells/workbook/createstyle/#createstyle_1)(bool) | Создаёт новый стиль. |
| [CustomTheme](../../aspose.cells/workbook/customtheme/)(string, Color[]) | Настраивает тему. |
| [Dispose](../../aspose.cells/workbook/dispose/)() | Выполняет задачи, определённые приложением, связанные с освобождением, высвобождением или сбросом неуправляемых ресурсов. |
| [ExportXml](../../aspose.cells/workbook/exportxml/#exportxml)(string, Stream) | Экспортировать XML-данные. |
| [ExportXml](../../aspose.cells/workbook/exportxml/#exportxml_1)(string, string) | Экспортировать XML-данные, связанные указанной XML-картой. |
| [GetDigitalSignature](../../aspose.cells/workbook/getdigitalsignature/)() | Получает цифровую подпись из файла. |
| [GetFonts](../../aspose.cells/workbook/getfonts/)() | Получает все шрифты в пуле стилей. |
| [GetMatchingColor](../../aspose.cells/workbook/getmatchingcolor/)(Color) | Находит наиболее подходящий цвет в текущей палитре. |
| [GetNamedStyle](../../aspose.cells/workbook/getnamedstyle/)(string) | Получает именованный стиль из пула стилей. |
| [GetStyleInPool](../../aspose.cells/workbook/getstyleinpool/)(int) | Получает стиль из пула стилей. Все стили в рабочей книге будут собраны в пул. В ячейках присутствует только простой индекс ссылки. |
| [GetThemeColor](../../aspose.cells/workbook/getthemecolor/)(ThemeColorType) | Получает цвет темы. |
| [HasExernalLinks](../../aspose.cells/workbook/hasexernallinks/)() | (**Obsolete.**) Указывает, содержит ли эта рабочая книга внешние ссылки на другие источники данных. |
| [ImportXml](../../aspose.cells/workbook/importxml/#importxml)(Stream, string, int, int) | Импортирует/обновляет XML-файл данных в рабочую книгу. |
| [ImportXml](../../aspose.cells/workbook/importxml/#importxml_1)(string, string, int, int) | Импортирует/обновляет XML-файл данных в рабочую книгу. |
| [IsColorInPalette](../../aspose.cells/workbook/iscolorinpalette/)(Color) | Проверяет, находится ли цвет в палитре электронных таблиц. |
| [MergeNamedStyles](../../aspose.cells/workbook/mergenamedstyles/)(Workbook) | Объединяет именованные стили из другого Excel-файла. |
| [ParseFormulas](../../aspose.cells/workbook/parseformulas/)(bool) | Разбирает все формулы, которые не были разобраны при загрузке из шаблонного файла или при установке в ячейку. |
| [Protect](../../aspose.cells/workbook/protect/)(ProtectionType, string) | Защищает книгу. |
| [ProtectSharedWorkbook](../../aspose.cells/workbook/protectsharedworkbook/)(string) | Защищает общую книгу. |
| [RefreshAll](../../aspose.cells/workbook/refreshall/)() | Обновляет связанные фигуры, все сводные таблицы и диаграммы с источником сводных данных. |
| [RefreshDynamicArrayFormulas](../../aspose.cells/workbook/refreshdynamicarrayformulas/#refreshdynamicarrayformulas)(bool) | Обновляет формулы динамических массивов (размещение в новый диапазон соседних ячеек в соответствии с текущими данными). Другие формулы в книге не будут вычисляться рекурсивно, даже если они использовались формулами динамических массивов. |
| [RefreshDynamicArrayFormulas](../../aspose.cells/workbook/refreshdynamicarrayformulas/#refreshdynamicarrayformulas_1)(bool, CalculationOptions) | Обновляет формулы динамических массивов (размещение в новый диапазон соседних ячеек в соответствии с текущими данными). |
| [RemoveDigitalSignature](../../aspose.cells/workbook/removedigitalsignature/)() | Удаляет цифровую подпись из этой таблицы. |
| [RemoveExternalLinks](../../aspose.cells/workbook/removeexternallinks/)() | (**Obsolete.**) Удаляет все внешние ссылки в книге. |
| [RemoveMacro](../../aspose.cells/workbook/removemacro/)() | Удаляет VBA/макрос из этой таблицы. |
| [RemovePersonalInformation](../../aspose.cells/workbook/removepersonalinformation/)() | Удаляет личную информацию. |
| [RemoveUnusedStyles](../../aspose.cells/workbook/removeunusedstyles/)() | Удалить все неиспользуемые стили. |
| [Replace](../../aspose.cells/workbook/replace/#replace)(bool, object) | Заменяет значения ячеек новыми данными. |
| [Replace](../../aspose.cells/workbook/replace/#replace_1)(int, object) | Заменяет значения ячеек новыми данными. |
| [Replace](../../aspose.cells/workbook/replace/#replace_6)(string, DataTable) | Заменяет значения ячеек данными из DataTable. |
| [Replace](../../aspose.cells/workbook/replace/#replace_2)(string, double) | Заменяет значение ячейки новым double. |
| [Replace](../../aspose.cells/workbook/replace/#replace_4)(string, int) | Заменяет значение ячейки новым integer. |
| [Replace](../../aspose.cells/workbook/replace/#replace_7)(string, string) | Заменяет значение ячейки новой строкой. |
| [Replace](../../aspose.cells/workbook/replace/#replace_3)(string, double[], bool) | Заменяет значения ячеек массивом double. |
| [Replace](../../aspose.cells/workbook/replace/#replace_5)(string, int[], bool) | Заменяет значения ячеек массивом integer. |
| [Replace](../../aspose.cells/workbook/replace/#replace_8)(string, string, ReplaceOptions) | Заменяет значение ячейки новой строкой. |
| [Replace](../../aspose.cells/workbook/replace/#replace_9)(string, string[], bool) | Заменяет значение ячейки новым массивом строк. |
| [Save](../../aspose.cells/workbook/save/#save_2)(string) | Сохранить книгу на диск. |
| [Save](../../aspose.cells/workbook/save/#save)(Stream, SaveFormat) | Сохраняет книгу в поток. |
| [Save](../../aspose.cells/workbook/save/#save_1)(Stream, SaveOptions) | Сохраняет книгу в поток. |
| [Save](../../aspose.cells/workbook/save/#save_3)(string, SaveFormat) | Сохраняет книгу на диск. |
| [Save](../../aspose.cells/workbook/save/#save_4)(string, SaveOptions) | Сохраняет книгу на диск. |
| [Save](../../aspose.cells/workbook/save/#save_5)(HttpResponse, string, ContentDisposition, SaveOptions) | Создаёт результирующую таблицу и передаёт её клиенту, затем открывает в браузере или в MS Workbook. |
| [Save](../../aspose.cells/workbook/save/#save_6)(HttpResponse, string, ContentDisposition, SaveOptions, bool) | Создаёт результирующую таблицу и передаёт её клиенту, затем открывает в браузере или в MS Workbook. |
| [SaveToStream](../../aspose.cells/workbook/savetostream/)() | Сохраняет файл Excel в объект MemoryStream как файл Excel97-2003 xls и возвращает его. |
| [SetDigitalSignature](../../aspose.cells/workbook/setdigitalsignature/)(DigitalSignatureCollection) | Устанавливает цифровую подпись в файл таблицы (Excel2007 и новее). |
| [SetEncryptionOptions](../../aspose.cells/workbook/setencryptionoptions/)(EncryptionType, int) | Установить параметры шифрования. |
| [SetThemeColor](../../aspose.cells/workbook/setthemecolor/)(ThemeColorType, Color) | Устанавливает цвет темы |
| [StartAccessCache](../../aspose.cells/workbook/startaccesscache/)(AccessCacheOptions) | Запускает сеанс, использующий кэш для доступа к данным. |
| [Unprotect](../../aspose.cells/workbook/unprotect/)(string) | Снимает защиту с книги. |
| [UnprotectSharedWorkbook](../../aspose.cells/workbook/unprotectsharedworkbook/)(string) | Снимает защиту с общей книги. |
| [UpdateCustomFunctionDefinition](../../aspose.cells/workbook/updatecustomfunctiondefinition/)(CustomFunctionDefinition) | Обновляет определение пользовательских функций. |
| [UpdateLinkedDataSource](../../aspose.cells/workbook/updatelinkeddatasource/)(Workbook[]) | Если эта книга содержит внешние ссылки на другие источники данных, Aspose.Cells попытается получить последние данные из указанных источников. |

### Примечания

Класс Workbook обозначает электронную таблицу Excel. Каждая таблица может содержать несколько листов. Основная возможность класса — открывать и сохранять нативные файлы Excel. Класс имеет некоторые расширенные функции, такие как копирование данных из других Workbook, объединение двух Workbook, преобразование Excel в PDF, рендеринг Excel в изображение и защита электронной таблицы Excel.

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class WorkbookDemo
    {
        public static void WorkbookExample()
        {
            // Создать новый экземпляр Workbook
            Workbook workbook = new Workbook();

            // Получить доступ к листу по умолчанию
            Worksheet worksheet = workbook.Worksheets[0];

            // Установить некоторые свойства книги
            workbook.FileName = "ExampleWorkbook.xlsx";
            workbook.DefaultStyle.Font.Name = "Tahoma";

            // Добавить новый лист
            int newSheetIndex = workbook.Worksheets.Add();
            Worksheet newWorksheet = workbook.Worksheets[newSheetIndex];
            newWorksheet.Name = "NewSheet";

            // Добавить данные в новый лист
            newWorksheet.Cells["A1"].PutValue("Hello, Aspose.Cells!");

            // Установить некоторые свойства документа
            workbook.BuiltInDocumentProperties["Author"].Value = "John Smith";
            workbook.CustomDocumentProperties.Add("Checked by", "Jane");

            // Сохранить книгу в файл
            workbook.Save("WorkbookExample.xlsx");

            // Отобразить некоторые свойства
            Console.WriteLine("Workbook File Name: " + workbook.FileName);
            Console.WriteLine("Default Font: " + workbook.DefaultStyle.Font.Name);
            Console.WriteLine("Author: " + workbook.BuiltInDocumentProperties["Author"].Value);
            Console.WriteLine("Custom Property 'Checked by': " + workbook.CustomDocumentProperties["Checked by"].Value);

            // Проверить, лицензирована ли книга
            Console.WriteLine("Is Licensed: " + workbook.IsLicensed);

            // Проверить, подписана ли книга цифровой подписью
            Console.WriteLine("Is Digitally Signed: " + workbook.IsDigitallySigned);

            // Проверить, содержит ли книга макросы
            Console.WriteLine("Has Macros: " + workbook.HasMacro);

            // Проверить, есть ли в книге отслеживаемые изменения
            Console.WriteLine("Has Revisions: " + workbook.HasRevisions);

            // Проверить количество стилей в пуле стилей
            Console.WriteLine("Number of Styles in Pool: " + workbook.CountOfStylesInPool);

            // Проверить название темы
            Console.WriteLine("Theme: " + workbook.Theme);

            // Проверить, защищена ли книга паролем
            Console.WriteLine("Is Workbook Protected With Password: " + workbook.IsWorkbookProtectedWithPassword);

            // Проверить, содержит ли книга внешние ссылки
            Console.WriteLine("Has External Links: " + (workbook.Worksheets.ExternalLinks.Count > 0));

            // Освободить ресурсы книги
            workbook.Dispose();
        }
    }
}
```

### См. также

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


