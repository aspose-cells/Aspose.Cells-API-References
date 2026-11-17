---
title: "Класс FontConfigs"
linktitle: "FontConfigs"
second_title: "Справочник API Aspose.Cells for Go через C++"
description: "Класс FontConfigs. Инкапсулирует объект, представляющий fontconfigs в Go."
type: docs
weight: 200
url: /ru/go-cpp/fontconfigs/
---

## FontConfigs class

Указывает параметры шрифта

```go

type FontConfigs struct  {
	ptr unsafe.Pointer
}

```
## Конструкторы

| Метод | Описание |
| --- | --- |
| [NewFontConfigs](./newfontconfigs/) | Конструктор по умолчанию. |

## Методы

| Метод | Описание |
| --- | --- |
| [IsNull](./isnull/) | Проверяет, является ли объект реализации nullptr. |
| [FontConfigs_IsFontAvailable](./fontconfigs_isfontavailable/) | Указывает, доступен ли шрифт. |
| [FontConfigs_GetFontFileDataInfo](./fontconfigs_getfontfiledatainfo/) | Получить информацию о данных файла шрифта. |
| [FontConfigs_GetDefaultFontName](./fontconfigs_getdefaultfontname/) | Получает или задает имя шрифта по умолчанию. |
| [FontConfigs_SetDefaultFontName](./fontconfigs_setdefaultfontname/) | Получает или задает имя шрифта по умолчанию. |
| [FontConfigs_GetPreferSystemFontSubstitutes](./fontconfigs_getprefersystemfontsubstitutes/) | Указывает, использовать ли системные заменители шрифтов в первую очередь, когда шрифт не представлен и заменитель этого шрифта не установлен. Например, в Ubuntu шрифт "Arial" обычно заменяется на "Liberation Sans". Значение по умолчанию — false. |
| [FontConfigs_SetPreferSystemFontSubstitutes](./fontconfigs_setprefersystemfontsubstitutes/) | Указывает, использовать ли системные заменители шрифтов в первую очередь, когда шрифт не представлен и заменитель этого шрифта не установлен. Например, в Ubuntu шрифт "Arial" обычно заменяется на "Liberation Sans". Значение по умолчанию — false. |
| [FontConfigs_SetFontSubstitutes](./fontconfigs_setfontsubstitutes/) | Имена заменяющих шрифтов для заданного оригинального имени шрифта. |
| [FontConfigs_GetFontSubstitutes](./fontconfigs_getfontsubstitutes/) | Возвращает массив, содержащий имена заменяющих шрифтов, которые будут использоваться, если оригинальный шрифт отсутствует. |
| [FontConfigs_SetFontFolder](./fontconfigs_setfontfolder/) | Устанавливает папку шрифтов |
| [FontConfigs_SetFontFolders](./fontconfigs_setfontfolders/) | Устанавливает папку шрифтов |
| [FontConfigs_SetFontSources](./fontconfigs_setfontsources/) | Устанавливает источники шрифтов. |
| [FontConfigs_GetFontSources](./fontconfigs_getfontsources/) | Получает копию массива, содержащего список источников |
