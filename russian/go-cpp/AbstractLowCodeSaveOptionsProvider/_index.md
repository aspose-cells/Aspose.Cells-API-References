---
title: "Класс AbstractLowCodeSaveOptionsProvider"
linktitle: "AbstractLowCodeSaveOptionsProvider"
second_title: "Справочник API Aspose.Cells for Go через C++"
description: "AbstractLowCodeSaveOptionsProvider class. Инкапсулирует объект, представляющий abstractlowcodesaveoptionsprovider в Go."
type: docs
weight: 200
url: /ru/go-cpp/abstractlowcodesaveoptionsprovider/
---

## AbstractLowCodeSaveOptionsProvider class

Реализация для предоставления нескольких вариантов сохранения для процессов, требующих множественных выходов. Например, функция <see cref="SpreadsheetSplitter"/> требует нескольких назначений для сохранения разделённых файлов.

```go

type AbstractLowCodeSaveOptionsProvider struct  {
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
| [GetSaveOptions](./getsaveoptions/) | Получает параметры сохранения, из которых берутся настройки вывода для текущей части. Возврат null означает пропустить данную часть. |
| [Finish](./finish/) | Освобождает ресурсы после обработки текущей части. |
