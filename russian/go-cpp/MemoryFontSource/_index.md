---
title: "Класс MemoryFontSource"
linktitle: "MemoryFontSource"
second_title: "Справочник API Aspose.Cells for Go через C++"
description: "Класс MemoryFontSource. Инкапсулирует объект, представляющий memoryfontsource в Go."
type: docs
weight: 200
url: /ru/go-cpp/memoryfontsource/
---

## MemoryFontSource class

Представляет один файл шрифта TrueType, хранящийся в памяти.

```go

type MemoryFontSource struct  {
	ptr unsafe.Pointer
}

```
## Конструкторы

| Метод | Описание |
| --- | --- |
| [NewMemoryFontSource_Stream](./newmemoryfontsource_stream/) | Конструктор. |
| [NewMemoryFontSource_FontSourceBase](./newmemoryfontsource_fontsourcebase/) | Создаётся из родительского объекта. |

## Методы

| Метод | Описание |
| --- | --- |
| [IsNull](./isnull/) | Проверяет, является ли объект реализации nullptr. |
| [GetFontData](./getfontdata/) | Двоичные данные шрифта. |
| [GetType](./gettype/) | Возвращает тип источника шрифта. |
