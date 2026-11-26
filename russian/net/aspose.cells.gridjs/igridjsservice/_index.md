---
title: "Интерфейс IGridJsService"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Интерфейс Aspose.Cells.GridJs.IGridJsService. Представляет базовый интерфейс API операций, используемый в действиях контроллера."
type: docs
url: /ru/net/aspose.cells.gridjs/igridjsservice/
---
## IGridJsService interface

Представляет интерфейс базовых API операций, используемых в действиях контроллера.

```csharp
public interface IGridJsService : IDisposable
```

## Методы

| Имя | Описание |
| --- | --- |
| [AddImage](../../aspose.cells.gridjs/igridjsservice/addimage/#addimage)(string, string, string, byte[]) | Выполняет операцию добавления изображения из локального файла, получая байты изображения напрямую. |
| [AddImage](../../aspose.cells.gridjs/igridjsservice/addimage/#addimage_1)(string, string, string, IFormFileCollection) | Выполняет операцию добавления изображения из локального файла, используя загруженные файлы формы. |
| [AddImageByURL](../../aspose.cells.gridjs/igridjsservice/addimagebyurl/)(string, string, string) | Выполняет операцию добавления изображения из удалённого URL. |
| [CheckInCacheForCollaborative](../../aspose.cells.gridjs/igridjsservice/checkincacheforcollaborative/)(string) | Проверяет, находится ли экземпляр рабочей книги в кэше памяти. Этот метод применяется только в режиме совместной работы. |
| [ClearAllJsonCache](../../aspose.cells.gridjs/igridjsservice/clearalljsoncache/)() | Очищает все записи кэша JSON (в памяти и на диске). |
| [ClearJsonCacheForUid](../../aspose.cells.gridjs/igridjsservice/clearjsoncacheforuid/)(string) | Очищает все записи кэша JSON, принадлежащие указанному уникальному идентификатору. Вызовите это после изменения исходного файла вне обычного потока, чтобы следующий запрос сгенерировал JSON заново. |
| [CopyImage](../../aspose.cells.gridjs/igridjsservice/copyimage/)(string, string) | Выполняет операцию копирования изображения. |
| [DetailFileJsonWithUid](../../aspose.cells.gridjs/igridjsservice/detailfilejsonwithuid/#detailfilejsonwithuid_1)(string, string) | Получает строку JSON для файла по указанному уникальному идентификатору. |
| [DetailFileJsonWithUid](../../aspose.cells.gridjs/igridjsservice/detailfilejsonwithuid/#detailfilejsonwithuid)(Workbook, string, string) | Получает строку JSON для рабочей книги по указанному уникальному идентификатору. |
| [DetailStreamJson](../../aspose.cells.gridjs/igridjsservice/detailstreamjson/#detailstreamjson_1)(Stream, string) | Записывает строку JSON для рабочей книги в поток |
| [DetailStreamJson](../../aspose.cells.gridjs/igridjsservice/detailstreamjson/#detailstreamjson)(Stream, Workbook, string) | Записывает строку JSON для рабочей книги в поток |
| [DetailStreamJsonWithUid](../../aspose.cells.gridjs/igridjsservice/detailstreamjsonwithuid/#detailstreamjsonwithuid_1)(Stream, string, string) | Записывает строку JSON для файла в поток по указанному уникальному идентификатору. |
| [DetailStreamJsonWithUid](../../aspose.cells.gridjs/igridjsservice/detailstreamjsonwithuid/#detailstreamjsonwithuid)(Stream, Workbook, string, string) | Записывает строку JSON для рабочей книги в поток по указанному уникальному идентификатору. |
| [Download](../../aspose.cells.gridjs/igridjsservice/download/)(string, string, string) | Применяет операцию загрузки файла |
| [GetFile](../../aspose.cells.gridjs/igridjsservice/getfile/)(string) | Получить поток файла |
| [GetWarningCallback](../../aspose.cells.gridjs/igridjsservice/getwarningcallback/)() | Получает пользовательский обратный вызов предупреждения для импорта файла. |
| [Image](../../aspose.cells.gridjs/igridjsservice/image/)(string, string) | Получить поток изображения. |
| [ImageUrl](../../aspose.cells.gridjs/igridjsservice/imageurl/)(string, string, string) | Получает URL изображения. |
| [LazyLoadingJson](../../aspose.cells.gridjs/igridjsservice/lazyloadingjson/)(string, string) | Получает строку JSON указанного листа в файле из кэша, используя указанный уникальный идентификатор. |
| [LazyLoadingStreamJson](../../aspose.cells.gridjs/igridjsservice/lazyloadingstreamjson/)(Stream, string, string) | Записывает строку JSON указанного листа в файле из кэша, используя указанный уникальный идентификатор, в поток. |
| [Load](../../aspose.cells.gridjs/igridjsservice/load/)(string, string) | Получает строку JSON файла из кэша, используя указанный уникальный идентификатор, задает имя выходного файла в JSON. |
| [Ole](../../aspose.cells.gridjs/igridjsservice/ole/)(string, string, int, out string) | Получает данные массива байтов встроенного OLE‑объекта. |
| [SetWarningCallback](../../aspose.cells.gridjs/igridjsservice/setwarningcallback/)(IWarningCallback) | Устанавливает пользовательский обратный вызов предупреждения для импорта файла. |
| [UpdateCell](../../aspose.cells.gridjs/igridjsservice/updatecell/)(string, string) | Применяет операцию обновления. |

### См. также

* namespace [Aspose.Cells.GridJs](../../aspose.cells.gridjs/)
* assembly [Aspose.Cells.GridJs](../../)


