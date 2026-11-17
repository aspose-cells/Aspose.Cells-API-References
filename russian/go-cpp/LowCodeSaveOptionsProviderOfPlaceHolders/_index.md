---
title: "Класс LowCodeSaveOptionsProviderOfPlaceHolders"
linktitle: "LowCodeSaveOptionsProviderOfPlaceHolders"
second_title: "Справочник API Aspose.Cells for Go через C++"
description: "Класс LowCodeSaveOptionsProviderOfPlaceHolders. Инкапсулирует объект, представляющий lowcodesaveoptionsproviderofplaceholders в Go."
type: docs
weight: 200
url: /ru/go-cpp/lowcodesaveoptionsproviderofplaceholders/
---

## LowCodeSaveOptionsProviderOfPlaceHolders class

Реализация для предоставления вариантов сохранения, которые сохраняют разделённые части в файлы, а путь результирующего файла определяется с помощью заполнителей.

```go

type LowCodeSaveOptionsProviderOfPlaceHolders struct  {
	ptr unsafe.Pointer
}

```
## Конструкторы

| Метод | Описание |
| --- | --- |
| [NewLowCodeSaveOptionsProviderOfPlaceHolders_String](./newlowcodesaveoptionsproviderofplaceholders_string/) | Создаёт экземпляр для предоставления параметров сохранения в соответствии с указанными шаблонами. |
| [NewLowCodeSaveOptionsProviderOfPlaceHolders_AbstractLowCodeSaveOptionsProvider](./newlowcodesaveoptionsproviderofplaceholders_abstractlowcodesaveoptionsprovider/) | Создаётся из родительского объекта. |

## Методы

| Метод | Описание |
| --- | --- |
| [IsNull](./isnull/) | Проверяет, является ли объект реализации nullptr. |
| [GetSheetIndexOffset](./getsheetindexoffset/) | Смещение индекса листа между тем, что используется в пути к файлу, и его фактическим значением (SplitPartInfo.SheetIndex). |
| [SetSheetIndexOffset](./setsheetindexoffset/) | Смещение индекса листа между тем, что используется в пути к файлу, и его фактическим значением (SplitPartInfo.SheetIndex). |
| [GetSplitPartIndexOffset](./getsplitpartindexoffset/) | Смещение индекса части разбиения между тем, что используется в пути к файлу, и его фактическим значением (SplitPartInfo.PartIndex). |
| [SetSplitPartIndexOffset](./setsplitpartindexoffset/) | Смещение индекса части разбиения между тем, что используется в пути к файлу, и его фактическим значением (SplitPartInfo.PartIndex). |
| [GetBuildPathWithSheetAlways](./getbuildpathwithsheetalways/) | Определяет, добавлять ли индекс листа или его имя к пути файла всегда. Значение по умолчанию — false, то есть когда существует только один лист, индекс листа и имя, а также соответствующий префикс (SheetNamePrefix), не будут добавляться к пути файла. |
| [SetBuildPathWithSheetAlways](./setbuildpathwithsheetalways/) | Определяет, добавлять ли индекс листа или его имя к пути файла всегда. Значение по умолчанию — false, то есть когда существует только один лист, индекс листа и имя, а также соответствующий префикс (SheetNamePrefix), не будут добавляться к пути файла. |
| [GetBuildPathWithSplitPartAlways](./getbuildpathwithsplitpartalways/) | Определяет, добавлять ли индекс части разбиения к пути файла всегда. Значение по умолчанию — false, то есть когда существует только одна часть разбиения, индекс части разбиения и соответствующий префикс (SplitPartPrefix) не будут добавляться к пути файла. |
| [SetBuildPathWithSplitPartAlways](./setbuildpathwithsplitpartalways/) | Определяет, добавлять ли индекс части разбиения к пути файла всегда. Значение по умолчанию — false, то есть когда существует только одна часть разбиения, индекс части разбиения и соответствующий префикс (SplitPartPrefix) не будут добавляться к пути файла. |
| [GetSheetNamePrefix](./getsheetnameprefix/) | Префикс для индекса листа. |
| [SetSheetNamePrefix](./setsheetnameprefix/) | Префикс для индекса листа. |
| [GetSheetIndexPrefix](./getsheetindexprefix/) | Префикс для индекса листа. |
| [SetSheetIndexPrefix](./setsheetindexprefix/) | Префикс для индекса листа. |
| [GetSplitPartPrefix](./getsplitpartprefix/) | Префикс для индекса части разбиения. |
| [SetSplitPartPrefix](./setsplitpartprefix/) | Префикс для индекса части разбиения. |
| [GetSaveOptionsTemplate](./getsaveoptionstemplate/) | Шаблон для создания экземпляра параметров сохранения в GetSaveOptions(SplitPartInfo). |
| [SetSaveOptionsTemplate](./setsaveoptionstemplate/) | Шаблон для создания экземпляра параметров сохранения в GetSaveOptions(SplitPartInfo). |
| [GetSaveOptions](./getsaveoptions/) | Получает параметры сохранения, из которых берутся настройки вывода для текущей части разбиения. |
| [Finish](./finish/) | Освобождает ресурсы после обработки текущей части. |
