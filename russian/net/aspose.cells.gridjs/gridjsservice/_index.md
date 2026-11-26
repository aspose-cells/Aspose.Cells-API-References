---
title: "Класс GridJsService"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Aspose.Cells.GridJs.GridJsService class. Предоставляет базовые API операций, используемые в действиях контроллера"
type: docs
url: /ru/net/aspose.cells.gridjs/gridjsservice/
---
## GridJsService class

Предоставляет базовые API операций, используемые в действиях контроллера.

```csharp
public class GridJsService : IGridJsService
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [GridJsService](gridjsservice/#constructor)(GridJsOptions) | Конструктор GridJsService для хостов, которые самостоятельно создают объект параметров (браузерный WASM‑хост и любые серверные настройки без DI). |
| [GridJsService](gridjsservice/#constructor_1)(IOptions&lt;GridJsOptions&gt;) | Конструктор по умолчанию для GridJsService |

## Свойства

| Имя | Описание |
| --- | --- |
| [Settings](../../aspose.cells.gridjs/gridjsservice/settings/) { get; set; } | Представляет настройки рабочей книги. |

## Методы

| Имя | Описание |
| --- | --- |
| [AddImage](../../aspose.cells.gridjs/gridjsservice/addimage/#addimage)(string, string, string, byte[]) | Выполняет операцию добавления изображения из локального файла (байты файла поступают из JS FormData или любого хоста). |
| [AddImage](../../aspose.cells.gridjs/gridjsservice/addimage/#addimage_1)(string, string, string, IFormFileCollection) | Выполняет операцию добавления изображения из локального файла. |
| [AddImageByURL](../../aspose.cells.gridjs/gridjsservice/addimagebyurl/)(string, string, string) | Выполняет операцию добавления изображения из удалённого URL. |
| [CheckInCacheForCollaborative](../../aspose.cells.gridjs/gridjsservice/checkincacheforcollaborative/)(string) | Проверяет, находится ли экземпляр рабочей книги в кэше памяти. Этот метод применяется только в режиме совместной работы. |
| [ClearAllJsonCache](../../aspose.cells.gridjs/gridjsservice/clearalljsoncache/)() | Очищает все записи кэша JSON (в памяти и на диске). |
| [ClearJsonCacheForUid](../../aspose.cells.gridjs/gridjsservice/clearjsoncacheforuid/)(string) | Очищает все записи кэша JSON, принадлежащие указанному уникальному идентификатору. Вызовите это после изменения исходного файла вне обычного потока, чтобы следующий запрос сгенерировал JSON заново. |
| [CopyImage](../../aspose.cells.gridjs/gridjsservice/copyimage/)(string, string) | Выполняет операцию копирования изображения. |
| [Destroy](../../aspose.cells.gridjs/gridjsservice/destroy/)() | Этот метод предназначен только для Java, он реализует метод destroy в DisposableBean, который будет вызван автоматически Spring после завершения запроса; фактически он вызывает метод Dispose. |
| [DetailFileJsonWithUid](../../aspose.cells.gridjs/gridjsservice/detailfilejsonwithuid/#detailfilejsonwithuid_1)(string, string) | Получает строку JSON для файла по указанному уникальному идентификатору. |
| [DetailFileJsonWithUid](../../aspose.cells.gridjs/gridjsservice/detailfilejsonwithuid/#detailfilejsonwithuid)(Workbook, string, string) | Получает строку JSON для рабочей книги по указанному уникальному идентификатору. |
| [DetailStreamJson](../../aspose.cells.gridjs/gridjsservice/detailstreamjson/#detailstreamjson_1)(Stream, string) | Записывает строку JSON для файла в поток. |
| [DetailStreamJson](../../aspose.cells.gridjs/gridjsservice/detailstreamjson/#detailstreamjson)(Stream, Workbook, string) | Записывает строку JSON для рабочей книги в поток |
| [DetailStreamJsonWithUid](../../aspose.cells.gridjs/gridjsservice/detailstreamjsonwithuid/#detailstreamjsonwithuid_1)(Stream, string, string) | Записывает строку JSON для файла в поток по указанному уникальному идентификатору. |
| [DetailStreamJsonWithUid](../../aspose.cells.gridjs/gridjsservice/detailstreamjsonwithuid/#detailstreamjsonwithuid)(Stream, Workbook, string, string) | Записывает строку JSON для рабочей книги в поток по указанному уникальному идентификатору. |
| [Dispose](../../aspose.cells.gridjs/gridjsservice/dispose/)() | Выполняет задачи, определённые приложением, связанные с освобождением, высвобождением или сбросом неуправляемых ресурсов. |
| [Download](../../aspose.cells.gridjs/gridjsservice/download/)(string, string, string) | Применяет операцию загрузки файла |
| [GetFile](../../aspose.cells.gridjs/gridjsservice/getfile/)(string) | Получить поток файла |
| [GetWarningCallback](../../aspose.cells.gridjs/gridjsservice/getwarningcallback/)() | Получает пользовательский обратный вызов предупреждения для импорта файла. |
| [Image](../../aspose.cells.gridjs/gridjsservice/image/)(string, string) | Получить поток изображения. |
| [ImageUrl](../../aspose.cells.gridjs/gridjsservice/imageurl/)(string, string, string) | Получает URL изображения. |
| [LazyLoadingJson](../../aspose.cells.gridjs/gridjsservice/lazyloadingjson/)(string, string) | Получает строку JSON указанного листа в файле из кэша, используя указанный уникальный идентификатор. |
| [LazyLoadingStreamJson](../../aspose.cells.gridjs/gridjsservice/lazyloadingstreamjson/)(Stream, string, string) | Записывает строку JSON указанного листа в файле из кэша, используя указанный уникальный идентификатор, в поток. |
| [Load](../../aspose.cells.gridjs/gridjsservice/load/)(string, string) | Получает строку JSON файла из кэша, используя указанный уникальный идентификатор, задает имя выходного файла в JSON. |
| [Ole](../../aspose.cells.gridjs/gridjsservice/ole/)(string, string, int, out string) | Получает данные массива байтов встроенного OLE‑объекта. |
| [SetWarningCallback](../../aspose.cells.gridjs/gridjsservice/setwarningcallback/)(IWarningCallback) | Устанавливает пользовательский обратный вызов предупреждения для импорта файла. |
| [TranslateSheetAsync](../../aspose.cells.gridjs/gridjsservice/translatesheetasync/)(string, string, ITextTranslator, string) | Перевести все строковые значения на целевой язык в листе. |
| [UpdateCell](../../aspose.cells.gridjs/gridjsservice/updatecell/)(string, string) | Применяет операцию обновления. |

### См. также

* interface [IGridJsService](../igridjsservice/)
* namespace [Aspose.Cells.GridJs](../../aspose.cells.gridjs/)
* assembly [Aspose.Cells.GridJs](../../)


