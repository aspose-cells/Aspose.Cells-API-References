---
title: "Класс GridJsOptions"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Aspose.Cells.GridJs.GridJsOptions class. Представляет все параметры загрузки для GridJs"
type: docs
url: /ru/net/aspose.cells.gridjs/gridjsoptions/
---
## GridJsOptions class

Представляет все параметры загрузки для GridJs.

```csharp
public class GridJsOptions
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [GridJsOptions](gridjsoptions/)() | Конструктор по умолчанию. |

## Свойства

| Имя | Описание |
| --- | --- |
| [AutoFitColumnsOnLoad](../../aspose.cells.gridjs/gridjsoptions/autofitcolumnsonload/) { get; set; } | Указывает, следует ли автоматически подгонять ширину столбцов при загрузке файла, значение по умолчанию — false. |
| [AutoFitRowsHeightOnLoad](../../aspose.cells.gridjs/gridjsoptions/autofitrowsheightonload/) { get; set; } | Указывает, следует ли автоматически подгонять высоту строк при загрузке файла, значение по умолчанию — false. |
| [AutoOptimizeForLargeCells](../../aspose.cells.gridjs/gridjsoptions/autooptimizeforlargecells/) { get; set; } | Получает/устанавливает, следует ли автоматически оптимизировать производительность загрузки листа с большими ячейками. Будут игнорироваться некоторые стили/границы для сокращения времени загрузки. Значение по умолчанию — true. |
| [BaseRouteName](../../aspose.cells.gridjs/gridjsoptions/baseroutename/) { get; set; } | Получает/устанавливает базовое имя маршрута URL для контроллера GridJs. По умолчанию — GridJs2 |
| [CustomPdfSaveOptions](../../aspose.cells.gridjs/gridjsoptions/custompdfsaveoptions/) { get; set; } | Получает/устанавливает пользовательские PdfSaveOptions для экспорта в PDF. Если задано, будет использовано вместо параметров по умолчанию. Значение по умолчанию — null. |
| [EmptySheetMaxCol](../../aspose.cells.gridjs/gridjsoptions/emptysheetmaxcol/) { get; set; } | Получает/устанавливает максимальное количество столбцов по умолчанию для пустого листа. Значение по умолчанию — 15. |
| [EmptySheetMaxRow](../../aspose.cells.gridjs/gridjsoptions/emptysheetmaxrow/) { get; set; } | Получает/устанавливает максимальное количество строк по умолчанию для пустого листа. Значение по умолчанию — 12. |
| [EnableChartClientRendering](../../aspose.cells.gridjs/gridjsoptions/enablechartclientrendering/) { get; set; } | Получает/устанавливает, следует ли включить рендеринг диаграмм на клиенте. Если установить false, GridJs будет выводить только изображения/формы диаграмм и не потребует рендеринг на клиенте. Значение по умолчанию — true. |
| [FileCacheDirectory](../../aspose.cells.gridjs/gridjsoptions/filecachedirectory/) { get; set; } | Получает/Устанавливает каталог кэша для хранения файлов электронных таблиц. Необходимо установить его в конкретный путь перед использованием GridJs. |
| [FontFolders](../../aspose.cells.gridjs/gridjsoptions/fontfolders/) { get; set; } | Получает/Устанавливает папки шрифтов для шрифтов в отрисованных изображениях/формах |
| [IgnoreEmptyContent](../../aspose.cells.gridjs/gridjsoptions/ignoreemptycontent/) { get; set; } | Получает/Устанавливает, показывать ли максимальный диапазон, который включает данные, стиль, объединённые ячейки и формы. Если последняя строка или столбец содержит ячейки без значения и формулы, но с пользовательским стилем, то при истинном значении мы не будем показывать эту строку/столбец. Значение по умолчанию — true. |
| [IsCollaborative](../../aspose.cells.gridjs/gridjsoptions/iscollaborative/) { get; set; } | Получает/Устанавливает, поддерживать ли совместное редактирование, значение по умолчанию — false. |
| [IslimitShapeOrImage](../../aspose.cells.gridjs/gridjsoptions/islimitshapeorimage/) { get; set; } | Получает/Устанавливает, ограничивать ли общее количество отображаемых форм/изображений в одном листе; если установлено в true, GridJs ограничит общее количество отображаемых форм или изображений в одном листе значением MaxShapeOrImageCount. Значение по умолчанию — true. |
| [IsWasm](../../aspose.cells.gridjs/gridjsoptions/iswasm/) { get; set; } | Получает/Устанавливает, работает ли GridJs внутри браузерного WebAssembly‑хоста вместо серверного процесса. При значении true не используется FileCacheDirectory / диск / путь interrupt‑thread, и кэш файлов должен поступать из CacheImp, поскольку у браузерного хоста нет локального диска. Выбираются пути кода во время выполнения, поэтому один Aspose.Cells.GridJs.dll обслуживает оба хоста. Значение по умолчанию — false. |
| [JsonCache](../../aspose.cells.gridjs/gridjsoptions/jsoncache/) { get; set; } | Получает/Устанавливает параметры конфигурации кэша JSON. Управляет поведением кэша в памяти (L1) и на диске (L2) для сгенерированного JSON книги. |
| [LazyLoading](../../aspose.cells.gridjs/gridjsoptions/lazyloading/) { get; set; } | Получает/Устанавливает, загружать ли только активный лист, значение по умолчанию — false. |
| [MaxPdfSaveSeconds](../../aspose.cells.gridjs/gridjsoptions/maxpdfsaveseconds/) { get; set; } | Получает/Устанавливает максимальное время ожидания в секундах при сохранении в PDF. Значение по умолчанию — 10. |
| [MaxShapeOrImageCount](../../aspose.cells.gridjs/gridjsoptions/maxshapeorimagecount/) { get; set; } | Получает/Устанавливает общее количество отображаемых форм или изображений в активном листе, действует при IslimitShapeOrImage=true. Значение по умолчанию — 100. |
| [MaxShapeOrImageWidthOrHeight](../../aspose.cells.gridjs/gridjsoptions/maxshapeorimagewidthorheight/) { get; set; } | Получает/Устанавливает максимальную ширину или высоту для формы или изображения, GridJs будет игнорировать форму или изображение с шириной или высотой, превышающей это значение, действует при IslimitShapeOrImage=true. Значение по умолчанию — 10000. |
| [MaxTotalShapeOrImageCount](../../aspose.cells.gridjs/gridjsoptions/maxtotalshapeorimagecount/) { get; set; } | Получает/Устанавливает общее количество отображаемых форм или изображений в книге, действует при IslimitShapeOrImage=true. Значение по умолчанию — 300. |
| [MessageTopic](../../aspose.cells.gridjs/gridjsoptions/messagetopic/) { get; set; } | Получает/Устанавливает назначения веб‑сокетов с префиксом "/topic". По умолчанию — "/topic/opr". Используется только в режиме совместной работы. |
| [PictureCacheDirectory](../../aspose.cells.gridjs/gridjsoptions/picturecachedirectory/) { get; set; } | Получает/Устанавливает каталог кэша для изображений (это действует, когда GridJsWorkbook.CacheImp равно null). Путь по умолчанию будет "_piccache" внутри FileCacheDirectory. |
| [SameImageDetecting](../../aspose.cells.gridjs/gridjsoptions/sameimagedetecting/) { get; set; } | Получает/Устанавливает, проверять ли, имеют ли изображения одинаковый источник, значение по умолчанию — true. |
| [SaveHtmlAsZip](../../aspose.cells.gridjs/gridjsoptions/savehtmlaszip/) { get; set; } | Получает/Устанавливает, сохранять ли HTML‑файл как ZIP‑архив, значение по умолчанию — false. |
| [ShowChartSheet](../../aspose.cells.gridjs/gridjsoptions/showchartsheet/) { get; set; } | Получает/Устанавливает, показывать ли лист с диаграммами. Значение по умолчанию — false. |
| [SkipInvisibleShapes](../../aspose.cells.gridjs/gridjsoptions/skipinvisibleshapes/) { get; set; } | Получает/Устанавливает, пропускать ли формы, невидимые в пользовательском интерфейсе, значение по умолчанию — true. |
| [UsePrintArea](../../aspose.cells.gridjs/gridjsoptions/useprintarea/) { get; set; } | Получает/Устанавливает, использовать ли PageSetup.PrintArea для диапазона отображения в UI, когда лист имеет настройку PageSetup для PrintArea. Значение по умолчанию — false. |

## Поля

| Имя | Описание |
| --- | --- |
| [CacheImp](../../aspose.cells.gridjs/gridjsoptions/cacheimp/) | Пользовательская реализация хранилища кэша. Если вы хотите сохранять кэш в виде потока, необходимо установить и реализовать её. WebAssembly‑хост (IsWasm = true) должен установить её, поскольку для кэша по умолчанию нет локального диска. |
| [RedactionUseClientGenerateId](../../aspose.cells.gridjs/gridjsoptions/redactionuseclientgenerateid/) | Указывает, использовать ли идентификатор, сгенерированный клиентом, вместо фактического идентификатора формы в операциях, связанных с редактированием. |

### См. также

* namespace [Aspose.Cells.GridJs](../../aspose.cells.gridjs/)
* assembly [Aspose.Cells.GridJs](../../)


