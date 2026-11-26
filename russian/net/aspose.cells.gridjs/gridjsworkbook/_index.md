---
title: "Класс GridJsWorkbook"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.GridJs.GridJsWorkbook. Представляет основной класс входа для GridJs"
type: docs
url: /ru/net/aspose.cells.gridjs/gridjsworkbook/
---
## GridJsWorkbook class

Представляет основной класс входа для GridJs.

```csharp
public class GridJsWorkbook
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [GridJsWorkbook](gridjsworkbook/)() | Создаёт новый экземпляр GridJsWorkbook. |

## Свойства

| Имя | Описание |
| --- | --- |
| [CacheDirectory](../../aspose.cells.gridjs/gridjsworkbook/cachedirectory/) { get; set; } | Получает/устанавливает каталог кэша для хранения файлов электронных таблиц. Если он не установлен, мы будем использовать статическое свойство из [`FileCacheDirectory`](../config/filecachedirectory/) или [`CacheImp`](./cacheimp/). |
| [Settings](../../aspose.cells.gridjs/gridjsworkbook/settings/) { get; set; } | Представляет настройки рабочей книги. |
| [WarningCallback](../../aspose.cells.gridjs/gridjsworkbook/warningcallback/) { get; set; } | Получает или устанавливает обратный вызов предупреждения для импорта файла. |

## Методы

| Имя | Описание |
| --- | --- |
| [BurnRedactionFile](../../aspose.cells.gridjs/gridjsworkbook/burnredactionfile/)(string, string) | Выполняет (применяет) все операции редактирования в рабочей книге, удаляя формы редактирования и их целевые формы или очищая содержимое целевых диапазонов ячеек. |
| [CheckInCacheForCollaborative](../../aspose.cells.gridjs/gridjsworkbook/checkincacheforcollaborative/)(string) | Проверяет, находится ли экземпляр рабочей книги в кэше памяти. Этот метод применяется только в режиме совместной работы. |
| [ClearAllJsonCache](../../aspose.cells.gridjs/gridjsworkbook/clearalljsoncache/)() | Очистить весь JSON‑кеш |
| [ClearJsonCacheForUid](../../aspose.cells.gridjs/gridjsworkbook/clearjsoncacheforuid/)(string) | Очистить JSON‑кеш по uid (используется в сценариях, таких как UpdateCell, где есть только uid) |
| [CopyImageOrShape](../../aspose.cells.gridjs/gridjsworkbook/copyimageorshape/)(string, string) | Копирует изображение или форму. |
| [Dispose](../../aspose.cells.gridjs/gridjsworkbook/dispose/)() | Выполняет задачи, определённые приложением, связанные с освобождением, высвобождением или сбросом неуправляемых ресурсов. |
| [ErrorJson](../../aspose.cells.gridjs/gridjsworkbook/errorjson/)(string) | Получает строку сообщения об ошибке в формате JSON. |
| [ExportToJson](../../aspose.cells.gridjs/gridjsworkbook/exporttojson/#exporttojson)() | Получает строку JSON из данных в памяти, имя файла по умолчанию в JSON: book1. |
| [ExportToJson](../../aspose.cells.gridjs/gridjsworkbook/exporttojson/#exporttojson_1)(string) | Получает строку JSON из данных в памяти, задаёт имя выходного файла в JSON. |
| [ExportToJsonStringBuilder](../../aspose.cells.gridjs/gridjsworkbook/exporttojsonstringbuilder/)(string, string) | Получает строку JSON из данных в памяти, задаёт имя выходного файла в JSON. |
| [GetJsonByUid](../../aspose.cells.gridjs/gridjsworkbook/getjsonbyuid/)(string, string) | Получает строку JSON файла из кэша, используя указанный уникальный идентификатор, задает имя выходного файла в JSON. |
| [GetOle](../../aspose.cells.gridjs/gridjsworkbook/getole/)(string, string, int, out string) | Получает данные массива байтов встроенного OLE‑объекта. |
| [GetSheetJsonWithCache](../../aspose.cells.gridjs/gridjsworkbook/getsheetjsonwithcache/)(string, string, string) | Получить JSON указанного листа (с кешем) |
| [GetWorkbookJsonWithCache](../../aspose.cells.gridjs/gridjsworkbook/getworkbookjsonwithcache/)(string, string) | Получить JSON всей рабочей книги (с кэшированием) |
| [ImportExcelFile](../../aspose.cells.gridjs/gridjsworkbook/importexcelfile/#importexcelfile_3)(string) | Импортирует файл Excel из пути к файлу. |
| [ImportExcelFile](../../aspose.cells.gridjs/gridjsworkbook/importexcelfile/#importexcelfile)(Workbook) | Импортирует файл Excel из объекта Workbook. |
| [ImportExcelFile](../../aspose.cells.gridjs/gridjsworkbook/importexcelfile/#importexcelfile_1)(Stream, GridLoadFormat) | Импортирует файл Excel из потока файла с форматом загрузки. |
| [ImportExcelFile](../../aspose.cells.gridjs/gridjsworkbook/importexcelfile/#importexcelfile_7)(string, string) | Импортирует файл Excel из пути к файлу. |
| [ImportExcelFile](../../aspose.cells.gridjs/gridjsworkbook/importexcelfile/#importexcelfile_4)(string, Workbook) | Импортирует файл Excel из объекта Workbook. |
| [ImportExcelFile](../../aspose.cells.gridjs/gridjsworkbook/importexcelfile/#importexcelfile_2)(Stream, GridLoadFormat, string) | Импортирует файл Excel из потока файла с форматом загрузки и паролем открытия. |
| [ImportExcelFile](../../aspose.cells.gridjs/gridjsworkbook/importexcelfile/#importexcelfile_5)(string, Stream, GridLoadFormat) | Импортирует файл Excel из потока файла. |
| [ImportExcelFile](../../aspose.cells.gridjs/gridjsworkbook/importexcelfile/#importexcelfile_8)(string, string, string) | Импортирует файл Excel из пути к файлу и пароля открытия. |
| [ImportExcelFile](../../aspose.cells.gridjs/gridjsworkbook/importexcelfile/#importexcelfile_6)(string, Stream, GridLoadFormat, string) | Импортирует файл Excel из потока файла с форматом загрузки и паролем открытия. |
| [ImportExcelFileFromJson](../../aspose.cells.gridjs/gridjsworkbook/importexcelfilefromjson/)(string) | Импортирует файл Excel из строки в формате JSON. |
| [InsertImage](../../aspose.cells.gridjs/gridjsworkbook/insertimage/)(string, string, Stream, string) | Вставляет изображение в лист из потока файла или URL (необходимо предоставить либо поток файла, либо URL) или вставляет форму, когда p.type является одним из AutoShapeType |
| [JsonToStream](../../aspose.cells.gridjs/gridjsworkbook/jsontostream/)(Stream, string, string) | Генерирует JSON из находящегося в памяти Workbook и записывает его в указанный поток. При необходимости кэширует сгенерированный JSON для более быстрого последующего получения. Ключевые отличия от JsonToStreamByUid: - Этот метод использует текущее состояние Workbook в памяти (поле wb) - JsonToStreamByUid загружает Workbook из файлов кэша .cells на диске - Используйте этот метод, когда нужно экспортировать текущее состояние книги после изменений - Используйте JsonToStreamByUid, когда необходимо восстановить JSON из ранее кэшированного состояния файла. Поведение кэширования (при указании uid): - Проверяет кэш JSON перед генерацией (L1 память + L2 диск) - При промахе кэша генерирует JSON из Workbook в памяти - Сохраняет сгенерированный JSON в кэш для будущих запросов. |
| [JsonToStreamByUid](../../aspose.cells.gridjs/gridjsworkbook/jsontostreambyuid/)(Stream, string, string) | Получить строку JSON файла из кэша, используя указанный уникальный идентификатор, установить имя выходного файла в JSON и записать его в поток. |
| [LazyLoadingJson](../../aspose.cells.gridjs/gridjsworkbook/lazyloadingjson/)(string, string) | Получает строку JSON указанного листа в файле из кэша, используя указанный уникальный идентификатор. |
| [LazyLoadingStream](../../aspose.cells.gridjs/gridjsworkbook/lazyloadingstream/)(Stream, string, string) | Получить строку JSON указанного листа в файле из кэша, используя указанный уникальный идентификатор, и записать её в поток. |
| [MergeExcelFileFromJson](../../aspose.cells.gridjs/gridjsworkbook/mergeexcelfilefromjson/)(string, string) | Применяет пакетное обновление к данным в памяти. |
| [RedactFile](../../aspose.cells.gridjs/gridjsworkbook/redactfile/)(string, string, string[]) | Выполняет редактирование Excel-файла на основе массива операций JSON. |
| [SaveToCacheWithFileName](../../aspose.cells.gridjs/gridjsworkbook/savetocachewithfilename/)(string, string, string) | Сохраняет данные из памяти в файл кэша с указанным именем файла и также задает пароль открытия; формат сохранения определяется расширением имени файла. |
| [SaveToExcelFile](../../aspose.cells.gridjs/gridjsworkbook/savetoexcelfile/#savetoexcelfile)(Stream) | Сохраняет данные из памяти в поток, формат сохраняется на основе исходного формата файла. |
| [SaveToExcelFile](../../aspose.cells.gridjs/gridjsworkbook/savetoexcelfile/#savetoexcelfile_1)(string) | Сохраняет данные из памяти по пути к файлу; если у файла есть расширение, формат сохранения определяется расширением файла. |
| [SaveToHtml](../../aspose.cells.gridjs/gridjsworkbook/savetohtml/#savetohtml)(Stream) | Сохраняет данные из памяти в поток, формат сохранения — html. |
| [SaveToHtml](../../aspose.cells.gridjs/gridjsworkbook/savetohtml/#savetohtml_1)(string) | Сохраняет данные из памяти по пути к файлу, формат сохранения — html. |
| [SaveToPdf](../../aspose.cells.gridjs/gridjsworkbook/savetopdf/#savetopdf)(Stream) | Сохраняет данные из памяти в поток, формат сохранения — pdf. |
| [SaveToPdf](../../aspose.cells.gridjs/gridjsworkbook/savetopdf/#savetopdf_1)(string) | Сохраняет данные из памяти по пути к файлу, формат сохранения — pdf. |
| [SaveToXlsx](../../aspose.cells.gridjs/gridjsworkbook/savetoxlsx/#savetoxlsx)(Stream) | Сохраняет данные из памяти в поток, формат сохранения — xlsx. |
| [SaveToXlsx](../../aspose.cells.gridjs/gridjsworkbook/savetoxlsx/#savetoxlsx_1)(string) | Сохраняет данные из памяти по пути к файлу, формат сохранения — xlsx. |
| [SetInterruptMonitorForLoad](../../aspose.cells.gridjs/gridjsworkbook/setinterruptmonitorforload/)(GridInterruptMonitor, int) | Устанавливает InterruptMonitor для операции загрузки. |
| [SetInterruptMonitorForSave](../../aspose.cells.gridjs/gridjsworkbook/setinterruptmonitorforsave/)(GridInterruptMonitor) | Устанавливает InterruptMonitor для операции сохранения. |
| [SetTransParentView](../../aspose.cells.gridjs/gridjsworkbook/settransparentview/)(string, string, bool) | Устанавливает прозрачность форм редактирования в рабочей книге. |
| [TranslateSheetAsync](../../aspose.cells.gridjs/gridjsworkbook/translatesheetasync/)(string, string, ITextTranslator, string) | Перевести все строковые значения на целевой язык в листе. |
| [UpdateCell](../../aspose.cells.gridjs/gridjsworkbook/updatecell/)(string, string) | Применяет операцию обновления. |
| static [GetGridLoadFormat](../../aspose.cells.gridjs/gridjsworkbook/getgridloadformat/)(string) | Получает формат загрузки по расширению файла |
| static [GetImageStream](../../aspose.cells.gridjs/gridjsworkbook/getimagestream/)(string, string, string) | Получить поток изображения. |
| static [GetImageUrl](../../aspose.cells.gridjs/gridjsworkbook/getimageurl/)(string, string, string) | Получает URL изображения. |
| static [GetUidForFile](../../aspose.cells.gridjs/gridjsworkbook/getuidforfile/)(string) | Создаёт новый уникальный идентификатор для кэша файлов, используя указанное имя файла. |
| static [SetImageUrlBase](../../aspose.cells.gridjs/gridjsworkbook/setimageurlbase/)(string) | Установите базовый URL действия получения изображения из контроллера. |

## Поля

| Имя | Описание |
| --- | --- |
| static [CacheImp](../../aspose.cells.gridjs/gridjsworkbook/cacheimp/) | Пользовательская реализация для хранения кэша. Если вы хотите хранить кэш в виде потока, вам необходимо установить и реализовать её. |
| static [CalculateEngine](../../aspose.cells.gridjs/gridjsworkbook/calculateengine/) | Пользовательская реализация для вычислительного движка. Если вы хотите выполнять пользовательские расчёты, вам необходимо установить и реализовать её. |
| const [pictureType](../../aspose.cells.gridjs/gridjsworkbook/picturetype/) | константное значение для типа изображения |
| static [UpdateMonitor](../../aspose.cells.gridjs/gridjsworkbook/updatemonitor/) | Получает/Устанавливает монитор обновления для отслеживания операции обновления |

### См. также

* namespace [Aspose.Cells.GridJs](../../aspose.cells.gridjs/)
* assembly [Aspose.Cells.GridJs](../../)


