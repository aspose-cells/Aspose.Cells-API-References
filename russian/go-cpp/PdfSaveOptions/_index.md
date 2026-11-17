---
title: "Класс PdfSaveOptions"
linktitle: "PdfSaveOptions"
second_title: "Справочник API Aspose.Cells for Go через C++"
description: "Класс PdfSaveOptions. Инкапсулирует объект, представляющий pdfsaveoptions в Go."
type: docs
weight: 200
url: /ru/go-cpp/pdfsaveoptions/
---

## PdfSaveOptions class

Представляет параметры сохранения файла pdf.

```go

type PdfSaveOptions struct  {
	ptr unsafe.Pointer
}

```
## Конструкторы

| Метод | Описание |
| --- | --- |
| [NewPdfSaveOptions](./newpdfsaveoptions/) | Создаёт параметры для сохранения PDF‑файла. |
| [NewPdfSaveOptions_PaginatedSaveOptions](./newpdfsaveoptions_paginatedsaveoptions/) | Создаётся из родительского объекта. |

## Методы

| Метод | Описание |
| --- | --- |
| [IsNull](./isnull/) | Проверяет, является ли объект реализации nullptr. |
| [GetEmbedStandardWindowsFonts](./getembedstandardwindowsfonts/) | True, чтобы встраивать шрифты TrueType. Влияет только на ASCII‑символы 32‑127. Шрифты для кодов символов выше 127 всегда встраиваются. Шрифты всегда встраиваются для стандарта PDF/A-1a, PDF/A-1b. По умолчанию — true. |
| [SetEmbedStandardWindowsFonts](./setembedstandardwindowsfonts/) | True, чтобы встраивать шрифты TrueType. Влияет только на ASCII‑символы 32‑127. Шрифты для кодов символов выше 127 всегда встраиваются. Шрифты всегда встраиваются для стандарта PDF/A-1a, PDF/A-1b. По умолчанию — true. |
| [GetBookmark](./getbookmark/) | Получает и задает объект PdfBookmarkEntry</see>. |
| [SetBookmark](./setbookmark/) | Получает и задает объект PdfBookmarkEntry</see>. |
| [GetCompliance](./getcompliance/) | Получает или задает уровень соответствия стандартам PDF для выходных документов. |
| [SetCompliance](./setcompliance/) | Получает или задает уровень соответствия стандартам PDF для выходных документов. |
| [GetSecurityOptions](./getsecurityoptions/) | Установите эти параметры, когда требуется безопасность в результате xls2pdf. |
| [SetSecurityOptions](./setsecurityoptions/) | Установите эти параметры, когда требуется безопасность в результате xls2pdf. |
| [GetCalculateFormula](./getcalculateformula/) | Указывает, следует ли вычислять формулы перед сохранением PDF‑файла. |
| [SetCalculateFormula](./setcalculateformula/) | Указывает, следует ли вычислять формулы перед сохранением PDF‑файла. |
| [GetPdfCompression](./getpdfcompression/) | Укажите алгоритм сжатия |
| [SetPdfCompression](./setpdfcompression/) | Укажите алгоритм сжатия |
| [SetImageResample](./setimageresample/) | Устанавливает желаемое PPI (pixels per inch) для пересэмплирования изображений и качество JPEG. Все изображения будут преобразованы в JPEG с указанным качеством, а изображения с разрешением выше заданного PPI будут пересэмплированы. |
| [GetCreatedTime](./getcreatedtime/) | Получает и задает время создания PDF‑документа. |
| [SetCreatedTime](./setcreatedtime/) | Получает и задает время создания PDF‑документа. |
| [GetProducer](./getproducer/) | Получает и задает производителя (producer) сгенерированного PDF‑документа. |
| [SetProducer](./setproducer/) | Получает и задает производителя (producer) сгенерированного PDF‑документа. |
| [GetOptimizationType](./getoptimizationtype/) | Получает и задает тип оптимизации PDF. |
| [SetOptimizationType](./setoptimizationtype/) | Получает и задает тип оптимизации PDF. |
| [GetCustomPropertiesExport](./getcustompropertiesexport/) | Получает или задает значение, определяющее способ экспорта CustomDocumentPropertyCollection в PDF‑файл. Значение по умолчанию — None. |
| [SetCustomPropertiesExport](./setcustompropertiesexport/) | Получает или задает значение, определяющее способ экспорта CustomDocumentPropertyCollection в PDF‑файл. Значение по умолчанию — None. |
| [GetExportDocumentStructure](./getexportdocumentstructure/) | Указывает, следует ли экспортировать структуру документа. |
| [SetExportDocumentStructure](./setexportdocumentstructure/) | Указывает, следует ли экспортировать структуру документа. |
| [GetDisplayDocTitle](./getdisplaydoctitle/) | Указывает, должно ли заголовок окна отображать название документа. |
| [SetDisplayDocTitle](./setdisplaydoctitle/) | Указывает, должно ли заголовок окна отображать название документа. |
| [GetFontEncoding](./getfontencoding/) | Получает или задает кодировку встроенных шрифтов в PDF. |
| [SetFontEncoding](./setfontencoding/) | Получает или задает кодировку встроенных шрифтов в PDF. |
| [GetWatermark](./getwatermark/) | Получает или задает водяной знак для вывода. |
| [SetWatermark](./setwatermark/) | Получает или задает водяной знак для вывода. |
| [GetEmbedAttachments](./getembedattachments/) | Указывает, следует ли встраивать вложение для объектов Ole в Excel. |
| [SetEmbedAttachments](./setembedattachments/) | Указывает, следует ли встраивать вложение для объектов Ole в Excel. |
| [GetZoomBehavior](./getzoombehavior/) | Получает или задает режим начального просмотра при открытии сгенерированного PDF‑документа. Значение по умолчанию — PdfZoomBehavior.None. |
| [SetZoomBehavior](./setzoombehavior/) | Получает или задает режим начального просмотра при открытии сгенерированного PDF‑документа. Значение по умолчанию — PdfZoomBehavior.None. |
| [GetZoomFactor](./getzoomfactor/) | Получает или задает процент масштабирования, используемый когдаZoomBehavior равно PdfZoomBehavior.ZoomFactor. |
| [SetZoomFactor](./setzoomfactor/) | Получает или задает процент масштабирования, используемый когдаZoomBehavior равно PdfZoomBehavior.ZoomFactor. |
| [GetDefaultFont](./getdefaultfont/) | Когда символы в Excel являются Unicode и не заданы правильным шрифтом в стиле ячейки, они могут отображаться как блоки в pdf, изображении. Установите DefaultFont, например MingLiu или MS Gothic, чтобы отобразить эти символы. Если это свойство не задано, Aspose.Cells будет использовать системный шрифт по умолчанию для отображения этих Unicode‑символов. |
| [SetDefaultFont](./setdefaultfont/) | Когда символы в Excel являются Unicode и не заданы правильным шрифтом в стиле ячейки, они могут отображаться как блоки в pdf, изображении. Установите DefaultFont, например MingLiu или MS Gothic, чтобы отобразить эти символы. Если это свойство не задано, Aspose.Cells будет использовать системный шрифт по умолчанию для отображения этих Unicode‑символов. |
| [GetCheckWorkbookDefaultFont](./getcheckworkbookdefaultfont/) | Когда символы в Excel являются Unicode и не заданы правильным шрифтом в стиле ячейки, они могут отображаться как блоки в pdf, изображении. Установите значение true, чтобы сначала попытаться использовать шрифт по умолчанию книги для отображения этих символов. |
| [SetCheckWorkbookDefaultFont](./setcheckworkbookdefaultfont/) | Когда символы в Excel являются Unicode и не заданы правильным шрифтом в стиле ячейки, они могут отображаться как блоки в pdf, изображении. Установите значение true, чтобы сначала попытаться использовать шрифт по умолчанию книги для отображения этих символов. |
| [SetCheckFontCompatibility](./setcheckfontcompatibility/) | Указывает, следует ли проверять совместимость шрифта для каждого символа в тексте. |
| [GetCheckFontCompatibility](./getcheckfontcompatibility/) | Указывает, следует ли проверять совместимость шрифта для каждого символа в тексте. |
| [SetIsFontSubstitutionCharGranularity](./setisfontsubstitutionchargranularity/) | Указывает, следует ли заменять шрифт символа только когда шрифт ячейки несовместим с ним. |
| [IsFontSubstitutionCharGranularity](./isfontsubstitutionchargranularity/) | Указывает, следует ли заменять шрифт символа только когда шрифт ячейки несовместим с ним. |
| [GetOnePagePerSheet](./getonepagepersheet/) | Если OnePagePerSheet равно true, всё содержимое листа будет выводиться на одну страницу в результате. Размер бумаги в настройках страницы будет недействительным, а остальные настройки pagesetup по‑прежнему будут применяться. |
| [SetOnePagePerSheet](./setonepagepersheet/) | Если OnePagePerSheet равно true, всё содержимое листа будет выводиться на одну страницу в результате. Размер бумаги в настройках страницы будет недействительным, а остальные настройки pagesetup по‑прежнему будут применяться. |
| [GetAllColumnsInOnePagePerSheet](./getallcolumnsinonepagepersheet/) | Если AllColumnsInOnePagePerSheet равно true, всё содержимое столбцов листа будет выводиться на одну страницу в результате. Ширина бумаги в настройках страницы будет игнорироваться, а остальные настройки pagesetup по‑прежнему будут применяться. |
| [SetAllColumnsInOnePagePerSheet](./setallcolumnsinonepagepersheet/) | Если AllColumnsInOnePagePerSheet равно true, всё содержимое столбцов листа будет выводиться на одну страницу в результате. Ширина бумаги в настройках страницы будет игнорироваться, а остальные настройки pagesetup по‑прежнему будут применяться. |
| [GetIgnoreError](./getignoreerror/) | Указывает, нужно ли скрывать ошибку при рендеринге. Ошибка может быть связана с формой, изображением, рендерингом диаграммы и т.д. |
| [SetIgnoreError](./setignoreerror/) | Указывает, нужно ли скрывать ошибку при рендеринге. Ошибка может быть связана с формой, изображением, рендерингом диаграммы и т.д. |
| [GetOutputBlankPageWhenNothingToPrint](./getoutputblankpagewhennothingtoprint/) | Указывает, следует ли выводить пустую страницу, когда нечего печатать. |
| [SetOutputBlankPageWhenNothingToPrint](./setoutputblankpagewhennothingtoprint/) | Указывает, следует ли выводить пустую страницу, когда нечего печатать. |
| [SetPageIndex](./setpageindex/) | Получает или задаёт нулевой индекс первой страницы для сохранения. |
| [GetPageIndex](./getpageindex/) | Получает или задаёт нулевой индекс первой страницы для сохранения. |
| [SetPageCount](./setpagecount/) | Получает или задаёт количество страниц для сохранения. |
| [GetPageCount](./getpagecount/) | Получает или задаёт количество страниц для сохранения. |
| [GetPrintingPageType](./getprintingpagetype/) | Указывает, какие страницы не будут печататься. |
| [SetPrintingPageType](./setprintingpagetype/) | Указывает, какие страницы не будут печататься. |
| [GetGridlineType](./getgridlinetype/) | Получает или задаёт тип линий сетки. |
| [SetGridlineType](./setgridlinetype/) | Получает или задаёт тип линий сетки. |
| [GetGridlineColor](./getgridlinecolor/) | Получает или задаёт цвет линий сетки. |
| [SetGridlineColor](./setgridlinecolor/) | Получает или задаёт цвет линий сетки. |
| [GetTextCrossType](./gettextcrosstype/) | Получает или задаёт тип отображения текста, когда ширина текста превышает ширину ячейки. |
| [SetTextCrossType](./settextcrosstype/) | Получает или задаёт тип отображения текста, когда ширина текста превышает ширину ячейки. |
| [GetDefaultEditLanguage](./getdefaulteditlanguage/) | Получает или задаёт язык редактирования по умолчанию. |
| [SetDefaultEditLanguage](./setdefaulteditlanguage/) | Получает или задаёт язык редактирования по умолчанию. |
| [GetSheetSet](./getsheetset/) | Получает или задаёт листы для рендеринга. По умолчанию — все видимые листы в книге: Aspose.Cells.Rendering.SheetSet.Visible. |
| [SetSheetSet](./setsheetset/) | Получает или задаёт листы для рендеринга. По умолчанию — все видимые листы в книге: Aspose.Cells.Rendering.SheetSet.Visible. |
| [GetDrawObjectEventHandler](./getdrawobjecteventhandler/) | Реализует этот интерфейс, чтобы получить DrawObject и Bound при рендеринге. |
| [SetDrawObjectEventHandler](./setdrawobjecteventhandler/) | Реализует этот интерфейс, чтобы получить DrawObject и Bound при рендеринге. |
| [GetEmfRenderSetting](./getemfrendersetting/) | Настройка рендеринга метафайла Emf. |
| [SetEmfRenderSetting](./setemfrendersetting/) | Настройка рендеринга метафайла Emf. |
| [GetCustomRenderSettings](./getcustomrendersettings/) | Получает или задаёт пользовательские настройки во время рендеринга. |
| [SetCustomRenderSettings](./setcustomrendersettings/) | Получает или задаёт пользовательские настройки во время рендеринга. |
| [GetRenderingBehavior](./getrenderingbehavior/) | Получает или задаёт специфические для Excel поведения рендеринга, которые следует применить. |
| [SetRenderingBehavior](./setrenderingbehavior/) | Получает или задаёт специфические для Excel поведения рендеринга, которые следует применить. |
| [GetSaveFormat](./getsaveformat/) | Получает формат сохраняемого файла. |
| [GetClearData](./getcleardata/) | Очищает книгу после сохранения файла. |
| [SetClearData](./setcleardata/) | Очищает книгу после сохранения файла. |
| [GetCachedFileFolder](./getcachedfilefolder/) | Папка для временных файлов, которые могут использоваться в качестве кэша данных. |
| [SetCachedFileFolder](./setcachedfilefolder/) | Папка для временных файлов, которые могут использоваться в качестве кэша данных. |
| [GetValidateMergedAreas](./getvalidatemergedareas/) | Указывает, следует ли проверять объединённые ячейки перед сохранением файла. |
| [SetValidateMergedAreas](./setvalidatemergedareas/) | Указывает, следует ли проверять объединённые ячейки перед сохранением файла. |
| [GetMergeAreas](./getmergeareas/) | Указывает, следует ли объединять области условного форматирования и проверки перед сохранением файла. |
| [SetMergeAreas](./setmergeareas/) | Указывает, следует ли объединять области условного форматирования и проверки перед сохранением файла. |
| [GetCreateDirectory](./getcreatedirectory/) | Если true и каталог не существует, каталог будет автоматически создан перед сохранением файла. |
| [SetCreateDirectory](./setcreatedirectory/) | Если true и каталог не существует, каталог будет автоматически создан перед сохранением файла. |
| [GetSortNames](./getsortnames/) | Указывает, следует ли сортировать определённые имена перед сохранением файла. |
| [SetSortNames](./setsortnames/) | Указывает, следует ли сортировать определённые имена перед сохранением файла. |
| [GetSortExternalNames](./getsortexternalnames/) | Указывает, следует ли сортировать внешние определённые имена перед сохранением файла. |
| [SetSortExternalNames](./setsortexternalnames/) | Указывает, следует ли сортировать внешние определённые имена перед сохранением файла. |
| [GetRefreshChartCache](./getrefreshchartcache/) | Указывает, следует ли кэшировать последние данные диаграммы. |
| [SetRefreshChartCache](./setrefreshchartcache/) | Указывает, следует ли кэшировать последние данные диаграммы. |
| [GetCheckExcelRestriction](./getcheckexcelrestriction/) | Проверять ограничения файла Excel, когда пользователь изменяет связанные с ячейками объекты. Например, Excel не позволяет вводить строковое значение длиной более 32 КБ. Если ввести значение длиной более 32 КБ, оно будет усечено. |
| [SetCheckExcelRestriction](./setcheckexcelrestriction/) | Проверять ограничения файла Excel, когда пользователь изменяет связанные с ячейками объекты. Например, Excel не позволяет вводить строковое значение длиной более 32 КБ. Если ввести значение длиной более 32 КБ, оно будет усечено. |
| [GetUpdateSmartArt](./getupdatesmartart/) | Указывает, следует ли обновлять настройки SmartArt. Значение по умолчанию — false. |
| [SetUpdateSmartArt](./setupdatesmartart/) | Указывает, следует ли обновлять настройки SmartArt. Значение по умолчанию — false. |
| [GetEncryptDocumentProperties](./getencryptdocumentproperties/) | Указывает, следует ли шифровать свойства документа при сохранении в файл .xls. Значение по умолчанию — true. |
| [SetEncryptDocumentProperties](./setencryptdocumentproperties/) | Указывает, следует ли шифровать свойства документа при сохранении в файл .xls. Значение по умолчанию — true. |
