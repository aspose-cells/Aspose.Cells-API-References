---
title: "LowCodeSaveOptionsProviderOfAssembling Класс"
linktitle: "LowCodeSaveOptionsProviderOfAssembling"
second_title: "Справочник API Aspose.Cells for Go через C++"
description: "LowCodeSaveOptionsProviderOfAssembling class. Инкапсулирует объект, представляющий lowcodesaveoptionsproviderofassembling в Go."
type: docs
weight: 200
url: /ru/go-cpp/lowcodesaveoptionsproviderofassembling/
---

## LowCodeSaveOptionsProviderOfAssembling class

Реализация для предоставления вариантов сохранения, которые сохраняют разделённые части в файлы, а путь результирующего файла формируется как (может содержать каталоги):<see cref="PathHeader"/>+<see cref="SheetPrefix"/>+SheetIndex(или SheetName)+<see cref="SplitPartPrefix"/>+SplitPartIndex+<see cref="PathTail"/>.

```go

type LowCodeSaveOptionsProviderOfAssembling struct  {
	ptr unsafe.Pointer
}

```
## Конструкторы

| Метод | Описание |
| --- | --- |
| [NewLowCodeSaveOptionsProviderOfAssembling](./newlowcodesaveoptionsproviderofassembling/) | Конструктор по умолчанию. |
| [NewLowCodeSaveOptionsProviderOfAssembling_AbstractLowCodeSaveOptionsProvider](./newlowcodesaveoptionsproviderofassembling_abstractlowcodesaveoptionsprovider/) | Создаётся из родительского объекта. |

## Методы

| Метод | Описание |
| --- | --- |
| [IsNull](./isnull/) | Проверяет, является ли объект реализации nullptr. |
| [GetPathHeader](./getpathheader/) | Часть заголовка (до добавленного содержимого листа и части разбиения) пути к файлу. |
| [SetPathHeader](./setpathheader/) | Часть заголовка (до добавленного содержимого листа и части разбиения) пути к файлу. |
| [GetPathTail](./getpathtail/) | Конечная часть (после последовательных номеров) пути к файлу.Она должна включать расширение имени файла. |
| [SetPathTail](./setpathtail/) | Конечная часть (после последовательных номеров) пути к файлу.Она должна включать расширение имени файла. |
| [GetUseSheetName](./getusesheetname/) | Определяет, строит ли путь к файлу с именем листа вместо индекса листа. Значение по умолчанию — false. |
| [SetUseSheetName](./setusesheetname/) | Определяет, строит ли путь к файлу с именем листа вместо индекса листа. Значение по умолчанию — false. |
| [GetSheetPrefix](./getsheetprefix/) | Префикс для индекса листа. |
| [SetSheetPrefix](./setsheetprefix/) | Префикс для индекса листа. |
| [GetSplitPartPrefix](./getsplitpartprefix/) | Префикс для индекса части разбиения. |
| [SetSplitPartPrefix](./setsplitpartprefix/) | Префикс для индекса части разбиения. |
| [GetSheetIndexOffset](./getsheetindexoffset/) | Смещение индекса листа между тем, что используется в пути к файлу, и его фактическим значением (SplitPartInfo.SheetIndex). |
| [SetSheetIndexOffset](./setsheetindexoffset/) | Смещение индекса листа между тем, что используется в пути к файлу, и его фактическим значением (SplitPartInfo.SheetIndex). |
| [GetSplitPartIndexOffset](./getsplitpartindexoffset/) | Смещение индекса части разбиения между тем, что используется в пути к файлу, и его фактическим значением (SplitPartInfo.PartIndex). |
| [SetSplitPartIndexOffset](./setsplitpartindexoffset/) | Смещение индекса части разбиения между тем, что используется в пути к файлу, и его фактическим значением (SplitPartInfo.PartIndex). |
| [GetBuildPathWithSheetAlways](./getbuildpathwithsheetalways/) | Определяет, добавлять ли всегда индекс листа или его имя к пути к файлу. Значение по умолчанию — false, то есть когда существует только один лист, индекс листа (или имя) и соответствующий префикс не будут добавлены к пути к файлу. |
| [SetBuildPathWithSheetAlways](./setbuildpathwithsheetalways/) | Определяет, добавлять ли всегда индекс листа или его имя к пути к файлу. Значение по умолчанию — false, то есть когда существует только один лист, индекс листа (или имя) и соответствующий префикс не будут добавлены к пути к файлу. |
| [GetBuildPathWithSplitPartAlways](./getbuildpathwithsplitpartalways/) | Определяет, добавлять ли всегда индекс части разбиения к пути к файлу. Значение по умолчанию — false, то есть когда существует только одна часть разбиения, её индекс и соответствующий префикс не будут добавлены к пути к файлу. |
| [SetBuildPathWithSplitPartAlways](./setbuildpathwithsplitpartalways/) | Определяет, добавлять ли всегда индекс части разбиения к пути к файлу. Значение по умолчанию — false, то есть когда существует только одна часть разбиения, её индекс и соответствующий префикс не будут добавлены к пути к файлу. |
| [GetSaveOptionsTemplate](./getsaveoptionstemplate/) | Шаблон для создания экземпляра параметров сохранения в GetSaveOptions(SplitPartInfo). |
| [SetSaveOptionsTemplate](./setsaveoptionstemplate/) | Шаблон для создания экземпляра параметров сохранения в GetSaveOptions(SplitPartInfo). |
| [GetSaveOptions](./getsaveoptions/) | Получает параметры сохранения, из которых берутся настройки вывода для текущей части разбиения. |
| [Finish](./finish/) | Освобождает ресурсы после обработки текущей части. |
