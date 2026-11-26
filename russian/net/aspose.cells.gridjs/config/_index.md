---
title: "Класс Config"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.GridJs.Config. Представляет все статические настройки для GridJs"
type: docs
url: /ru/net/aspose.cells.gridjs/config/
---
## Config class

Представляет все статические настройки для GridJs

```csharp
public class Config
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [Config](config/)() | Конструктор по умолчанию. |

## Свойства

| Имя | Описание |
| --- | --- |
| static [AutoFitColumnsOnLoad](../../aspose.cells.gridjs/config/autofitcolumnsonload/) { get; set; } | Указывает, следует ли автоматически подгонять ширину столбцов при загрузке файла. Значение по умолчанию — `false`. Предупреждение: установка значения `true` выполнит автоматическую подгонку всех столбцов после загрузки, что может заметно повлиять на производительность. |
| static [AutoFitRowsHeightOnLoad](../../aspose.cells.gridjs/config/autofitrowsheightonload/) { get; set; } | Указывает, следует ли автоматически подгонять высоту строк при загрузке файла. Значение по умолчанию — `false`. Предупреждение: установка значения `true` выполнит автоматическую подгонку всех строк после загрузки, что может заметно повлиять на производительность. |
| static [AutoOptimizeForLargeCells](../../aspose.cells.gridjs/config/autooptimizeforlargecells/) { get; set; } | Получает/устанавливает, следует ли автоматически оптимизировать производительность загрузки листа с большими ячейками. Будут игнорироваться некоторые стили/границы для сокращения времени загрузки. Значение по умолчанию — true. |
| static [BaseRouteName](../../aspose.cells.gridjs/config/baseroutename/) { get; set; } | Получает/устанавливает базовое имя маршрута для URL контроллера GridJs. По умолчанию — "/GridJs2". |
| static [CustomPdfSaveOptions](../../aspose.cells.gridjs/config/custompdfsaveoptions/) { get; set; } | Получает/устанавливает пользовательские PdfSaveOptions для экспорта в PDF. Если задано, будет использовано вместо параметров по умолчанию. Значение по умолчанию — null. |
| static [EmptySheetMaxCol](../../aspose.cells.gridjs/config/emptysheetmaxcol/) { get; set; } | Получает/устанавливает максимальное количество столбцов по умолчанию для пустого листа. Значение по умолчанию — 15. |
| static [EmptySheetMaxRow](../../aspose.cells.gridjs/config/emptysheetmaxrow/) { get; set; } | Получает/устанавливает максимальное количество строк по умолчанию для пустого листа. Значение по умолчанию — 12. |
| static [EnableChartClientRendering](../../aspose.cells.gridjs/config/enablechartclientrendering/) { get; set; } | Получает/устанавливает, включена ли отрисовка диаграмм на клиенте. Если установить значение false, GridJs будет использовать только серверно‑созданные изображения/формы диаграмм. Значение по умолчанию — true. |
| static [FileCacheDirectory](../../aspose.cells.gridjs/config/filecachedirectory/) { get; set; } | Получает/Устанавливает каталог кэша для хранения файлов электронных таблиц. Необходимо установить его в конкретный путь перед использованием GridJs. |
| static [IgnoreEmptyContent](../../aspose.cells.gridjs/config/ignoreemptycontent/) { get; set; } | Получает/Устанавливает, показывать ли максимальный диапазон, который включает данные, стиль, объединённые ячейки и формы. Если последняя строка или столбец содержит ячейки без значения и формулы, но с пользовательским стилем, то при истинном значении мы не будем показывать эту строку/столбец. Значение по умолчанию — true. |
| static [IsCollaborative](../../aspose.cells.gridjs/config/iscollaborative/) { get; set; } | Получает/Устанавливает, поддерживать ли совместное редактирование, значение по умолчанию — false. |
| static [IslimitShapeOrImage](../../aspose.cells.gridjs/config/islimitshapeorimage/) { get; set; } | Получает/Устанавливает, ограничивать ли общее количество отображаемых форм/изображений в одном листе; если установлено в true, GridJs ограничит общее количество отображаемых форм или изображений в одном листе значением MaxShapeOrImageCount. Значение по умолчанию — true. |
| static [IsWasm](../../aspose.cells.gridjs/config/iswasm/) { get; set; } | Получает/устанавливает, работает ли GridJs внутри WebAssembly‑хоста в браузере вместо серверного процесса. При значении true не используется путь FileCacheDirectory / диск / прерывающий поток, и кэш файлов должен поступать из GridJsOptions.CacheImp. GridJsOptions.IsWasm задаёт это при построении сервиса GridJs, поэтому один Aspose.Cells.GridJs.dll обслуживает оба хоста. Значение по умолчанию — false. |
| static [JsonCache](../../aspose.cells.gridjs/config/jsoncache/) { get; set; } | Получает/Устанавливает параметры конфигурации кэша JSON. Управляет поведением кэша в памяти (L1) и на диске (L2) для сгенерированного JSON книги. |
| static [LazyLoading](../../aspose.cells.gridjs/config/lazyloading/) { get; set; } | Получает/Устанавливает, загружать ли только активный лист, значение по умолчанию — false. |
| static [MaxPdfSaveSeconds](../../aspose.cells.gridjs/config/maxpdfsaveseconds/) { get; set; } | Получает/Устанавливает максимальное время ожидания в секундах при сохранении в PDF. Значение по умолчанию — 10. |
| static [MaxShapeOrImageCount](../../aspose.cells.gridjs/config/maxshapeorimagecount/) { get; set; } | Получает/Устанавливает общее количество отображаемых форм или изображений в активном листе, действует при IslimitShapeOrImage=true. Значение по умолчанию — 100. |
| static [MaxShapeOrImageWidthOrHeight](../../aspose.cells.gridjs/config/maxshapeorimagewidthorheight/) { get; set; } | Получает/Устанавливает максимальную ширину или высоту для формы или изображения, GridJs будет игнорировать форму или изображение с шириной или высотой, превышающей это значение, действует при IslimitShapeOrImage=true. Значение по умолчанию — 10000. |
| static [MaxTotalShapeOrImageCount](../../aspose.cells.gridjs/config/maxtotalshapeorimagecount/) { get; set; } | Получает/Устанавливает общее количество отображаемых форм или изображений в книге, действует при IslimitShapeOrImage=true. Значение по умолчанию — 300. |
| static [MessageTopic](../../aspose.cells.gridjs/config/messagetopic/) { get; set; } | Получает/Устанавливает назначения веб‑сокетов с префиксом "/topic". По умолчанию — "/topic/opr". Используется только в режиме совместной работы. |
| static [PictureCacheDirectory](../../aspose.cells.gridjs/config/picturecachedirectory/) { get; set; } | Получает/Устанавливает каталог кэша для изображений (это действует, когда GridJsWorkbook.CacheImp равно null). Путь по умолчанию будет "_piccache" внутри FileCacheDirectory. |
| static [SameImageDetecting](../../aspose.cells.gridjs/config/sameimagedetecting/) { get; set; } | Получает/Устанавливает, проверять ли, имеют ли изображения одинаковый источник, значение по умолчанию — true. |
| static [SaveHtmlAsZip](../../aspose.cells.gridjs/config/savehtmlaszip/) { get; set; } | Получает/Устанавливает, сохранять ли HTML‑файл как ZIP‑архив, значение по умолчанию — false. |
| static [ShowChartSheet](../../aspose.cells.gridjs/config/showchartsheet/) { get; set; } | Получает/Устанавливает, показывать ли лист с диаграммами. Значение по умолчанию — false. |
| static [SkipInvisibleShapes](../../aspose.cells.gridjs/config/skipinvisibleshapes/) { get; set; } | Получает/Устанавливает, пропускать ли формы, невидимые в пользовательском интерфейсе, значение по умолчанию — true. |
| static [UsePrintArea](../../aspose.cells.gridjs/config/useprintarea/) { get; set; } | Получает/Устанавливает, использовать ли PageSetup.PrintArea для диапазона отображения в UI, когда лист имеет настройку PageSetup для PrintArea. Значение по умолчанию — false. |

## Методы

| Имя | Описание |
| --- | --- |
| static [SetFontFolder](../../aspose.cells.gridjs/config/setfontfolder/)(string, bool) | Устанавливает папку шрифтов |
| static [SetFontFolders](../../aspose.cells.gridjs/config/setfontfolders/)(string[], bool) | Устанавливает папки шрифтов |

## Поля

| Имя | Описание |
| --- | --- |
| static [RedactionUseClientGenerateId](../../aspose.cells.gridjs/config/redactionuseclientgenerateid/) | Указывает, использовать ли идентификатор, сгенерированный клиентом, вместо фактического идентификатора формы в операциях, связанных с редактированием. |

### См. также

* namespace [Aspose.Cells.GridJs](../../aspose.cells.gridjs/)
* assembly [Aspose.Cells.GridJs](../../)


