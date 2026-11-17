---
title: "Класс CellsHelper"
linktitle: "CellsHelper"
second_title: "Справочник API Aspose.Cells for Go через C++"
description: "Класс CellsHelper. Инкапсулирует объект, представляющий cellshelper в Go."
type: docs
weight: 200
url: /ru/go-cpp/cellshelper/
---

## CellsHelper class

Предоставляет вспомогательные функции.

```go

type CellsHelper struct  {
	ptr unsafe.Pointer
}

```
## Конструкторы

| Метод | Описание |
| --- | --- |

## Методы

| Метод | Описание |
| --- | --- |
| [CellsHelper_GetSignificantDigitsType](./cellshelper_getsignificantdigitstype/) | Получает и задает тип значимых цифр по умолчанию для вывода числовых значений. Значение по умолчанию — SignificantDigitsType.G17. |
| [CellsHelper_SetSignificantDigitsType](./cellshelper_setsignificantdigitstype/) | Получает и задает тип значимых цифр по умолчанию для вывода числовых значений. Значение по умолчанию — SignificantDigitsType.G17. |
| [CellsHelper_GetDPI](./cellshelper_getdpi/) | Получает DPI устройства. |
| [CellsHelper_SetDPI](./cellshelper_setdpi/) | Получает DPI устройства. |
| [CellsHelper_GetTextWidth](./cellshelper_gettextwidth/) | Получает ширину текста в единицах пунктов. |
| [CellsHelper_GetVersion](./cellshelper_getversion/) | Получает версию выпуска. |
| [CellsHelper_CellNameToIndex](./cellshelper_cellnametoindex/) | Получает индексы строки и столбца ячейки по её имени. |
| [CellsHelper_CellIndexToName](./cellshelper_cellindextoname/) | Получает имя ячейки по её индексам строки и столбца. |
| [CellsHelper_ColumnIndexToName](./cellshelper_columnindextoname/) | Получает имя столбца по индексу столбца. |
| [CellsHelper_ColumnNameToIndex](./cellshelper_columnnametoindex/) | Получает индекс столбца по его имени. |
| [CellsHelper_RowIndexToName](./cellshelper_rowindextoname/) | Получает имя строки по её индексу. |
| [CellsHelper_RowNameToIndex](./cellshelper_rownametoindex/) | Получает индекс строки по её имени. |
| [CellsHelper_GetDateTimeFromDouble](./cellshelper_getdatetimefromdouble/) | Преобразует значение double в значение даты и времени. |
| [CellsHelper_GetDoubleFromDateTime](./cellshelper_getdoublefromdatetime/) | Преобразует дату и время в значение double. |
| [CellsHelper_GetStartupPath](./cellshelper_getstartuppath/) | Получает или задает путь запуска, на который ссылаются некоторые внешние формульные ссылки. |
| [CellsHelper_SetStartupPath](./cellshelper_setstartuppath/) | Получает или задает путь запуска, на который ссылаются некоторые внешние формульные ссылки. |
| [CellsHelper_GetAltStartPath](./cellshelper_getaltstartpath/) | Получает или задает альтернативный путь запуска, на который ссылаются некоторые внешние формульные ссылки. |
| [CellsHelper_SetAltStartPath](./cellshelper_setaltstartpath/) | Получает или задает альтернативный путь запуска, на который ссылаются некоторые внешние формульные ссылки. |
| [CellsHelper_GetLibraryPath](./cellshelper_getlibrarypath/) | Получает или задает путь к библиотеке, на который ссылаются некоторые внешние формульные ссылки. |
| [CellsHelper_SetLibraryPath](./cellshelper_setlibrarypath/) | Получает или задает путь к библиотеке, на который ссылаются некоторые внешние формульные ссылки. |
| [CellsHelper_GetUsedColors](./cellshelper_getusedcolors/) | Получает все используемые цвета в рабочей книге. |
| [CellsHelper_MergeFiles](./cellshelper_mergefiles/) | Объединяет несколько больших файлов xls в один файл xls. |
| [CellsHelper_GetCacheFolder](./cellshelper_getcachefolder/) | Получает папку для временных файлов, которые могут использоваться в качестве кэша данных. |
| [CellsHelper_SetCacheFolder](./cellshelper_setcachefolder/) | Задает папку для временных файлов, которые могут использоваться в качестве кэша данных. |
| [CellsHelper_CreateSafeSheetName_String](./cellshelper_createsafesheetname_string/) | Проверяет указанное имя листа и при необходимости создает корректное. Если указанное имя листа соответствует правилам имен листов Excel, возвращает его. В противном случае строка будет усечена, если её длина превышает ограничение, а недопустимые символы будут заменены на ' ', затем возвращается восстановленное значение строки. |
| [CellsHelper_CreateSafeSheetName_String_Char](./cellshelper_createsafesheetname_string_char/) | Проверяет указанное имя листа и при необходимости создает корректное. Если указанное имя листа соответствует правилам имен листов Excel, возвращает его. В противном случае строка будет усечена, если её длина превышает ограничение, а недопустимые символы будут заменены заданным символом, затем возвращается восстановленное значение строки. |
| [CellsHelper_NeedQuoteInFormula](./cellshelper_needquoteinformula/) | Указывает, следует ли заключать имя листа в одинарные кавычки |
| [CellsHelper_IsCloudPlatform](./cellshelper_iscloudplatform/) | Пожалуйста, установите это свойство в значение True при работе на облачной платформе, такой как: Azure, AWSLambda и т.д., |
| [CellsHelper_SetIsCloudPlatform](./cellshelper_setiscloudplatform/) | Пожалуйста, установите это свойство в значение True при работе на облачной платформе, такой как: Azure, AWSLambda и т.д., |
