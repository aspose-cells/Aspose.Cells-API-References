---
title: "Класс CopyOptions"
linktitle: "CopyOptions"
second_title: "Справочник API Aspose.Cells for Go через C++"
description: "Класс CopyOptions. Инкапсулирует объект, представляющий copyoptions в Go."
type: docs
weight: 200
url: /ru/go-cpp/copyoptions/
---

## CopyOptions class

Представляет параметры копирования.

```go

type CopyOptions struct  {
	ptr unsafe.Pointer
}

```
## Конструкторы

| Метод | Описание |
| --- | --- |
| [NewCopyOptions](./newcopyoptions/) | Конструктор CopyOptions. |

## Методы

| Метод | Описание |
| --- | --- |
| [IsNull](./isnull/) | Проверяет, является ли объект реализации nullptr. |
| [GetKeepMacros](./getkeepmacros/) | Указывает, сохраняются ли макросы; |
| [SetKeepMacros](./setkeepmacros/) | Указывает, сохраняются ли макросы; |
| [GetExtendToAdjacentRange](./getextendtoadjacentrange/) | Указывает, следует ли расширять диапазоны при копировании диапазона в соседний диапазон. |
| [SetExtendToAdjacentRange](./setextendtoadjacentrange/) | Указывает, следует ли расширять диапазоны при копировании диапазона в соседний диапазон. |
| [GetCopyNames](./getcopynames/) | Указывает, копировать ли имена. |
| [SetCopyNames](./setcopynames/) | Указывает, копировать ли имена. |
| [GetCopyInvalidFormulasAsValues](./getcopyinvalidformulasasvalues/) | Если формула недействительна для целевого назначения, копировать только значения. |
| [SetCopyInvalidFormulasAsValues](./setcopyinvalidformulasasvalues/) | Если формула недействительна для целевого назначения, копировать только значения. |
| [GetColumnCharacterWidth](./getcolumncharacterwidth/) | Указывает, копировать ли ширину столбца в единицах символов. |
| [SetColumnCharacterWidth](./setcolumncharacterwidth/) | Указывает, копировать ли ширину столбца в единицах символов. |
| [GetReferToSheetWithSameName](./getrefertosheetwithsamename/) | В MS Excel при копировании формул, которые ссылаются на другие листы, при копировании листа в другой лист, скопированные формулы должны ссылаться на исходную книгу. Однако в некоторых ситуациях пользователю может потребоваться, чтобы скопированные формулы ссылались на листы с тем же именем в той же книге, например когда эти листы были скопированы до этой операции копирования; тогда это свойство должно быть установлено в значение true. |
| [SetReferToSheetWithSameName](./setrefertosheetwithsamename/) | В MS Excel при копировании формул, которые ссылаются на другие листы, при копировании листа в другой лист, скопированные формулы должны ссылаться на исходную книгу. Однако в некоторых ситуациях пользователю может потребоваться, чтобы скопированные формулы ссылались на листы с тем же именем в той же книге, например когда эти листы были скопированы до этой операции копирования; тогда это свойство должно быть установлено в значение true. |
| [GetReferToDestinationSheet](./getrefertodestinationsheet/) | При копировании диапазона в том же файле и если диаграмма ссылается на исходный лист, False означает, что источник данных скопированной диаграммы не будет изменён. True означает, что источник данных скопированной диаграммы ссылается на лист назначения. |
| [SetReferToDestinationSheet](./setrefertodestinationsheet/) | При копировании диапазона в том же файле и если диаграмма ссылается на исходный лист, False означает, что источник данных скопированной диаграммы не будет изменён. True означает, что источник данных скопированной диаграммы ссылается на лист назначения. |
| [GetUpdateInvalidReferencesToTargetSheet](./getupdateinvalidreferencestotargetsheet/) | Указывает, следует ли ссылаться на целевой лист, если ссылка листа не была скопирована. |
| [SetUpdateInvalidReferencesToTargetSheet](./setupdateinvalidreferencestotargetsheet/) | Указывает, следует ли ссылаться на целевой лист, если ссылка листа не была скопирована. |
