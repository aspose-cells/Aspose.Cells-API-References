---
title: "LoadDataFilterOptions Enum"
linktitle: "LoadDataFilterOptions"
second_title: "Справочник API Aspose.Cells for Go через C++"
description: "LoadDataFilterOptions enum. Инкапсулирует объект, представляющий loaddatafilteroptions в Go."
type: docs
weight: 200
url: /ru/go-cpp/loaddatafilteroptions/
---

## LoadDataFilterOptions Enum

Представляет параметры фильтрации данных при загрузке рабочей книги из шаблона.

```go

type LoadDataFilterOptions int32


```

## Поля

| Поле | Описание |
| --- | --- |
| [All](./all/) | Загрузить всё |
| [CellBlank](./cellblank/) | Загрузить ячейки, значение которых пусто |
| [CellString](./cellstring/) | Загрузить ячейки, значение которых является строкой |
| [CellNumeric](./cellnumeric/) | Загрузить ячейки, значение которых числовое (включая дату и время) |
| [CellError](./cellerror/) | Загрузить ячейки, значение которых является ошибкой |
| [CellBool](./cellbool/) | Загрузить ячейки, значение которых логическое |
| [CellValue](./cellvalue/) | Загружать только значения ячеек (все типы значений) |
| [Formula](./formula/) | Загружать формулы ячеек. |
| [CellData](./celldata/) | Загружать данные ячеек, включая значения, формулы и форматирование |
| [Chart](./chart/) | Загружать диаграммы |
| [Drawing](./drawing/) | Графические объекты (включая Chart, Picture, OleObject и все остальные графические объекты) |
| [MergedArea](./mergedarea/) | Загружать объединённые ячейки |
| [ConditionalFormatting](./conditionalformatting/) | Загружать условное форматирование |
| [DataValidation](./datavalidation/) | Загружать проверку данных |
| [PivotTable](./pivottable/) | Загружать сводные таблицы |
| [Table](./table/) | Загружать таблицы |
| [Hyperlinks](./hyperlinks/) | Загружать гиперссылки |
| [SheetSettings](./sheetsettings/) | Загружать настройки листа |
| [SheetData](./sheetdata/) | Загружать все данные листа, такие как данные ячеек, настройки, объекты и т.д. |
| [BookSettings](./booksettings/) | Загрузить настройки рабочей книги |
| [Settings](./settings/) | Загрузить настройки рабочей книги и листа |
| [XmlMap](./xmlmap/) | Загрузить XmlMap |
| [Structure](./structure/) | Загрузить структуру рабочей книги |
| [Document_Properties](./document_properties/) | Загрузить свойства документа |
| [DefinedNames](./definednames/) | Загрузить определённые объекты Name |
| [VBA](./vba/) | Загрузить проекты VBA |
| [Style](./style/) | Загрузить стили для форматирования ячеек |
| [Picture](./picture/) | Загрузить изображения |
| [OleObject](./oleobject/) | Загрузить OleObjects |
| [Revision](./revision/) | Загрузить журналы изменений |
