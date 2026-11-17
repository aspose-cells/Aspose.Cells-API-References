---
title: "Класс WorkbookSettings"
linktitle: "WorkbookSettings"
second_title: "Справочник API Aspose.Cells for Go через C++"
description: "Класс WorkbookSettings. Инкапсулирует объект, представляющий настройки рабочей книги в Go."
type: docs
weight: 200
url: /ru/go-cpp/workbooksettings/
---

## WorkbookSettings class

Представляет все настройки рабочей книги.

```go

type WorkbookSettings struct  {
	ptr unsafe.Pointer
}

```
## Конструкторы

| Метод | Описание |
| --- | --- |

## Методы

| Метод | Описание |
| --- | --- |
| [IsNull](./isnull/) | Проверяет, является ли объект реализации nullptr. |
| [Dispose](./dispose/) | Освобождает ресурсы. |
| [GetThemeFont](./getthemefont/) | Получает имя шрифта темы по умолчанию. |
| [GetAuthor](./getauthor/) | Получает и задает автора файла. |
| [SetAuthor](./setauthor/) | Получает и задает автора файла. |
| [GetCheckCustomNumberFormat](./getcheckcustomnumberformat/) | Указывает, проверять ли пользовательский числовой формат при установке Style.Custom. |
| [SetCheckCustomNumberFormat](./setcheckcustomnumberformat/) | Указывает, проверять ли пользовательский числовой формат при установке Style.Custom. |
| [GetEnableMacros](./getenablemacros/) | Включить макросы; |
| [SetEnableMacros](./setenablemacros/) | Включить макросы; |
| [GetDate1904](./getdate1904/) | Получает или задает значение, которое указывает, использует ли рабочая книга систему дат 1904 года. |
| [SetDate1904](./setdate1904/) | Получает или задает значение, которое указывает, использует ли рабочая книга систему дат 1904 года. |
| [GetProtectionType](./getprotectiontype/) | Получает тип защиты рабочей книги. |
| [GetDisplayDrawingObjects](./getdisplaydrawingobjects/) | Указывает, показывать ли и как отображать объекты в рабочей книге. |
| [SetDisplayDrawingObjects](./setdisplaydrawingobjects/) | Указывает, показывать ли и как отображать объекты в рабочей книге. |
| [GetSheetTabBarWidth](./getsheettabbarwidth/) | Ширина панели вкладок листов (в 1/1000 ширины окна). |
| [SetSheetTabBarWidth](./setsheettabbarwidth/) | Ширина панели вкладок листов (в 1/1000 ширины окна). |
| [GetShowTabs](./getshowtabs/) | Получает или задает значение, отображаются ли вкладки Workbook. |
| [SetShowTabs](./setshowtabs/) | Получает или задает значение, отображаются ли вкладки Workbook. |
| [GetFirstVisibleTab](./getfirstvisibletab/) | Получает или задает первую видимую вкладку листа. |
| [SetFirstVisibleTab](./setfirstvisibletab/) | Получает или задает первую видимую вкладку листа. |
| [IsHScrollBarVisible](./ishscrollbarvisible/) | Получает или задает значение, указывающее, будет ли в сгенерированной таблице горизонтальная полоса прокрутки. |
| [SetIsHScrollBarVisible](./setishscrollbarvisible/) | Получает или задает значение, указывающее, будет ли в сгенерированной таблице горизонтальная полоса прокрутки. |
| [IsVScrollBarVisible](./isvscrollbarvisible/) | Получает или задает значение, указывающее, будет ли в сгенерированной таблице вертикальная полоса прокрутки. |
| [SetIsVScrollBarVisible](./setisvscrollbarvisible/) | Получает или задает значение, указывающее, будет ли в сгенерированной таблице вертикальная полоса прокрутки. |
| [GetShared](./getshared/) | Получает или задает значение, указывающее, является ли Workbook совместным. |
| [SetShared](./setshared/) | Получает или задает значение, указывающее, является ли Workbook совместным. |
| [GetLanguageCode](./getlanguagecode/) | Получает или задает язык пользовательского интерфейса версии Workbook на основе CountryCode, в которой был сохранён файл. |
| [SetLanguageCode](./setlanguagecode/) | Получает или задает язык пользовательского интерфейса версии Workbook на основе CountryCode, в которой был сохранён файл. |
| [GetRegion](./getregion/) | Получает или задает региональные настройки для рабочей книги. |
| [SetRegion](./setregion/) | Получает или задает региональные настройки для рабочей книги. |
| [GetGlobalizationSettings](./getglobalizationsettings/) | Получает и задает настройки глобализации. |
| [SetGlobalizationSettings](./setglobalizationsettings/) | Получает и задает настройки глобализации. |
| [GetNumberDecimalSeparator](./getnumberdecimalseparator/) | Получает или задает десятичный разделитель для форматирования/парсинга числовых значений. По умолчанию используется десятичный разделитель текущего региона. |
| [SetNumberDecimalSeparator](./setnumberdecimalseparator/) | Получает или задает десятичный разделитель для форматирования/парсинга числовых значений. По умолчанию используется десятичный разделитель текущего региона. |
| [GetNumberGroupSeparator](./getnumbergroupseparator/) | Получает или задает символ, разделяющий группы цифр слева от десятичной точки в числовых значениях. По умолчанию используется разделитель групп текущего региона. |
| [SetNumberGroupSeparator](./setnumbergroupseparator/) | Получает или задает символ, разделяющий группы цифр слева от десятичной точки в числовых значениях. По умолчанию используется разделитель групп текущего региона. |
| [GetPassword](./getpassword/) | Представляет пароль шифрования файла Workbook. |
| [SetPassword](./setpassword/) | Представляет пароль шифрования файла Workbook. |
| [GetWriteProtection](./getwriteprotection/) | Предоставляет доступ к параметрам защиты записи рабочей книги. |
| [IsEncrypted](./isencrypted/) | Получает значение, указывающее, требуется ли пароль для открытия этой книги. |
| [IsProtected](./isprotected/) | Получает значение, указывающее, защищена ли структура или окно книги. |
| [IsDefaultEncrypted](./isdefaultencrypted/) | Указывает, следует ли шифровать книгу с паролем по умолчанию, если структура и окна книги заблокированы. |
| [SetIsDefaultEncrypted](./setisdefaultencrypted/) | Указывает, следует ли шифровать книгу с паролем по умолчанию, если структура и окна книги заблокированы. |
| [IsMinimized](./isminimized/) | Представляет, будет ли сгенерированная таблица открыта в свернутом виде. |
| [SetIsMinimized](./setisminimized/) | Представляет, будет ли сгенерированная таблица открыта в свернутом виде. |
| [IsHidden](./ishidden/) | Указывает, скрыта ли эта книга. |
| [SetIsHidden](./setishidden/) | Указывает, скрыта ли эта книга. |
| [GetAutoCompressPictures](./getautocompresspictures/) | Указывает логическое значение, обозначающее, автоматически ли приложение сжимает изображения в книге. |
| [SetAutoCompressPictures](./setautocompresspictures/) | Указывает логическое значение, обозначающее, автоматически ли приложение сжимает изображения в книге. |
| [GetRemovePersonalInformation](./getremovepersonalinformation/) | Истина, если из указанной книги можно удалить личную информацию. |
| [SetRemovePersonalInformation](./setremovepersonalinformation/) | Истина, если из указанной книги можно удалить личную информацию. |
| [GetShapeDisplayType](./getshapedisplaytype/) | Получает и задает способ отображения фигур приложением в этой книге. |
| [SetShapeDisplayType](./setshapedisplaytype/) | Получает и задает способ отображения фигур приложением в этой книге. |
| [GetHidePivotFieldList](./gethidepivotfieldlist/) | Получает и задает, скрывать ли список полей для сводной таблицы. |
| [SetHidePivotFieldList](./sethidepivotfieldlist/) | Получает и задает, скрывать ли список полей для сводной таблицы. |
| [GetMaxUniqueItemsPerField](./getmaxuniqueitemsperfield/) | Получает и задает ограничение уникальных элементов на поле. |
| [SetMaxUniqueItemsPerField](./setmaxuniqueitemsperfield/) | Получает и задает ограничение уникальных элементов на поле. |
| [GetUpdateLinksType](./getupdatelinkstype/) | Получает и задает, как обновлять внешние ссылки при открытии книги. |
| [SetUpdateLinksType](./setupdatelinkstype/) | Получает и задает, как обновлять внешние ссылки при открытии книги. |
| [SetPageOrientationType](./setpageorientationtype/) | Устанавливает тип ориентации печати для всей книги. |
| [GetMaxRow](./getmaxrow/) | Получает максимальный индекс строки, начиная с нуля. |
| [GetMaxColumn](./getmaxcolumn/) | Получает максимальный индекс столбца, начиная с нуля. |
| [GetSmartTagOptions](./getsmarttagoptions/) | Получает параметры смарт-тега. |
| [GetDefaultStyleSettings](./getdefaultstylesettings/) | Получает настройки значений по умолчанию для свойств, связанных со стилем, в этой книге. |
| [GetWindowLeft](./getwindowleft/) | Расстояние от левого края клиентской области до левого края окна в пунктах. |
| [SetWindowLeft](./setwindowleft/) | Расстояние от левого края клиентской области до левого края окна в пунктах. |
| [GetWindowLeftInch](./getwindowleftinch/) | Расстояние от левого края клиентской области до левого края окна в дюймах. |
| [SetWindowLeftInch](./setwindowleftinch/) | Расстояние от левого края клиентской области до левого края окна в дюймах. |
| [GetWindowLeftCM](./getwindowleftcm/) | Расстояние от левого края клиентской области до левого края окна в сантиметрах. |
| [SetWindowLeftCM](./setwindowleftcm/) | Расстояние от левого края клиентской области до левого края окна в сантиметрах. |
| [GetWindowTop](./getwindowtop/) | Расстояние от верхнего края клиентской области до верхнего края окна в пунктах. |
| [SetWindowTop](./setwindowtop/) | Расстояние от верхнего края клиентской области до верхнего края окна в пунктах. |
| [GetWindowTopInch](./getwindowtopinch/) | Расстояние от верхнего края клиентской области до верхнего края окна в дюймах. |
| [SetWindowTopInch](./setwindowtopinch/) | Расстояние от верхнего края клиентской области до верхнего края окна в дюймах. |
| [GetWindowTopCM](./getwindowtopcm/) | Расстояние от верхнего края клиентской области до верхнего края окна в сантиметрах. |
| [SetWindowTopCM](./setwindowtopcm/) | Расстояние от верхнего края клиентской области до верхнего края окна в сантиметрах. |
| [GetWindowWidth](./getwindowwidth/) | Ширина окна в пунктах. |
| [SetWindowWidth](./setwindowwidth/) | Ширина окна в пунктах. |
| [GetWindowWidthInch](./getwindowwidthinch/) | Ширина окна в дюймах. |
| [SetWindowWidthInch](./setwindowwidthinch/) | Ширина окна в дюймах. |
| [GetWindowWidthCM](./getwindowwidthcm/) | Ширина окна в сантиметрах. |
| [SetWindowWidthCM](./setwindowwidthcm/) | Ширина окна в сантиметрах. |
| [GetWindowHeight](./getwindowheight/) | Высота окна в единицах пункта. |
| [SetWindowHeight](./setwindowheight/) | Высота окна в единицах пункта. |
| [GetWindowHeightInch](./getwindowheightinch/) | Высота окна в дюймах. |
| [SetWindowHeightInch](./setwindowheightinch/) | Высота окна в дюймах. |
| [GetWindowHeightCM](./getwindowheightcm/) | Высота окна в сантиметрах. |
| [SetWindowHeightCM](./setwindowheightcm/) | Высота окна в сантиметрах. |
| [GetUpdateAdjacentCellsBorder](./getupdateadjacentcellsborder/) | Указывает, следует ли обновлять границы соседних ячеек. |
| [SetUpdateAdjacentCellsBorder](./setupdateadjacentcellsborder/) | Указывает, следует ли обновлять границы соседних ячеек. |
| [GetSignificantDigitsType](./getsignificantdigitstype/) | Получает и задает тип значимых цифр для вывода числовых значений в этой книге. Значение по умолчанию — CellsHelper.SignificantDigitsType. |
| [SetSignificantDigitsType](./setsignificantdigitstype/) | Получает и задает тип значимых цифр для вывода числовых значений в этой книге. Значение по умолчанию — CellsHelper.SignificantDigitsType. |
| [GetCheckCompatibility](./getcheckcompatibility/) | Указывает, проверять ли совместимость с более ранними версиями при сохранении книги. |
| [SetCheckCompatibility](./setcheckcompatibility/) | Указывает, проверять ли совместимость с более ранними версиями при сохранении книги. |
| [GetCheckExcelRestriction](./getcheckexcelrestriction/) | Определяет, проверять ли ограничения файла Excel, когда пользователь изменяет связанные с ячейками объекты. Например, Excel не позволяет вводить строковое значение длиной более 32 КБ. Если вы вводите значение длиной более 32 КБ, например с помощью Cell.PutValue(string), и это свойство установлено в true, будет выброшено исключение. Если свойство установлено в false, мы примем введённую строку как значение ячейки, чтобы позже вы могли вывести полное строковое значение в другие форматы файлов, такие как CSV. Однако, если вы задали значение, которое недействительно для формата Excel, не следует сохранять рабочую книгу в формате Excel позже. В противном случае может возникнуть непредвиденная ошибка в сгенерированном файле Excel. |
| [SetCheckExcelRestriction](./setcheckexcelrestriction/) | Определяет, проверять ли ограничения файла Excel, когда пользователь изменяет связанные с ячейками объекты. Например, Excel не позволяет вводить строковое значение длиной более 32 КБ. Если вы вводите значение длиной более 32 КБ, например с помощью Cell.PutValue(string), и это свойство установлено в true, будет выброшено исключение. Если свойство установлено в false, мы примем введённую строку как значение ячейки, чтобы позже вы могли вывести полное строковое значение в другие форматы файлов, такие как CSV. Однако, если вы задали значение, которое недействительно для формата Excel, не следует сохранять рабочую книгу в формате Excel позже. В противном случае может возникнуть непредвиденная ошибка в сгенерированном файле Excel. |
| [GetAutoRecover](./getautorecover/) | Указывает, помечен ли файл для автоматического восстановления. |
| [SetAutoRecover](./setautorecover/) | Указывает, помечен ли файл для автоматического восстановления. |
| [GetCrashSave](./getcrashsave/) | Указывает, сохранило ли приложение файл книги после сбоя. |
| [SetCrashSave](./setcrashsave/) | Указывает, сохранило ли приложение файл книги после сбоя. |
| [GetDataExtractLoad](./getdataextractload/) | Указывает, открыло ли приложение книгу для восстановления данных. |
| [SetDataExtractLoad](./setdataextractload/) | Указывает, открыло ли приложение книгу для восстановления данных. |
| [GetRepairLoad](./getrepairload/) | Указывает, открыло ли приложение книгу в безопасном или режиме восстановления. |
| [SetRepairLoad](./setrepairload/) | Указывает, открыло ли приложение книгу в безопасном или режиме восстановления. |
| [GetBuildVersion](./getbuildversion/) | Указывает инкрементальный публичный релиз приложения. |
| [SetBuildVersion](./setbuildversion/) | Указывает инкрементальный публичный релиз приложения. |
| [GetMemorySetting](./getmemorysetting/) | Получает или задает параметры использования памяти. Новый параметр будет использоваться по умолчанию для вновь созданных листов, но не будет применяться к существующим листам. |
| [SetMemorySetting](./setmemorysetting/) | Получает или задает параметры использования памяти. Новый параметр будет использоваться по умолчанию для вновь созданных листов, но не будет применяться к существующим листам. |
| [GetPaperSize](./getpapersize/) | Получает и задает размер бумаги по умолчанию для печати. |
| [SetPaperSize](./setpapersize/) | Получает и задает размер бумаги по умолчанию для печати. |
| [GetMaxRowsOfSharedFormula](./getmaxrowsofsharedformula/) | Получает и задает максимальный номер строки общей формулы. |
| [SetMaxRowsOfSharedFormula](./setmaxrowsofsharedformula/) | Получает и задает максимальный номер строки общей формулы. |
| [GetCompliance](./getcompliance/) | Указывает версию OOXML для выходного документа. Значение по умолчанию — Ecma376_2006. |
| [SetCompliance](./setcompliance/) | Указывает версию OOXML для выходного документа. Значение по умолчанию — Ecma376_2006. |
| [GetQuotePrefixToStyle](./getquoteprefixtostyle/) | Указывает, следует ли устанавливать свойство Style.QuotePrefix при вводе строкового значения (которое начинается с одинарной кавычки) в ячейку. |
| [SetQuotePrefixToStyle](./setquoteprefixtostyle/) | Указывает, следует ли устанавливать свойство Style.QuotePrefix при вводе строкового значения (которое начинается с одинарной кавычки) в ячейку. |
| [GetFormulaSettings](./getformulasettings/) | Получает настройки функций, связанных с формулами. |
| [GetPropertiesFollowChartPoint](./getpropertiesfollowchartpoint/) | Указывает, следуют ли свойства точек данных и подписи данных во всех диаграммах этой книги их ссылкам. |
| [SetPropertiesFollowChartPoint](./setpropertiesfollowchartpoint/) | Указывает, следуют ли свойства точек данных и подписи данных во всех диаграммах этой книги их ссылкам. |
| [GetDiscardImageEditData](./getdiscardimageeditdata/) | Указывает, следует ли отбрасывать редактируемые данные изображения. |
| [SetDiscardImageEditData](./setdiscardimageeditdata/) | Указывает, следует ли отбрасывать редактируемые данные изображения. |
| [GetDefaultImageResolution](./getdefaultimageresolution/) | Получает и задает разрешение изображения по умолчанию. |
| [SetDefaultImageResolution](./setdefaultimageresolution/) | Получает и задает разрешение изображения по умолчанию. |
| [GetWpsCompatibility](./getwpscompatibility/) | Указывает, следует ли обеспечивать совместимость с WPS. |
| [SetWpsCompatibility](./setwpscompatibility/) | Указывает, следует ли обеспечивать совместимость с WPS. |
