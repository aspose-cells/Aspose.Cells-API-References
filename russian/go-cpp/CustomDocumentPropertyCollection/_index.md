---
title: "CustomDocumentPropertyCollection Класс"
linktitle: "CustomDocumentPropertyCollection"
second_title: "Справочник API Aspose.Cells for Go через C++"
description: "CustomDocumentPropertyCollection класс. Инкапсулирует объект, представляющий customdocumentpropertycollection в Go."
type: docs
weight: 200
url: /ru/go-cpp/customdocumentpropertycollection/
---

## CustomDocumentPropertyCollection class

Коллекция пользовательских свойств документа.

```go

type CustomDocumentPropertyCollection struct  {
	ptr unsafe.Pointer
}

```
## Конструкторы

| Метод | Описание |
| --- | --- |
| [NewCustomDocumentPropertyCollection](./newcustomdocumentpropertycollection/) | Создаётся из родительского объекта. |

## Методы

| Метод | Описание |
| --- | --- |
| [IsNull](./isnull/) | Проверяет, является ли объект реализации nullptr. |
| [Add_String_String](./add_string_string/) | Создаёт новое пользовательское свойство документа типа данных <b>PropertyType.String</b>. |
| [Add_String_Int](./add_string_int/) | Создаёт новое пользовательское свойство документа типа данных <b>PropertyType.Number</b>. |
| [Add_String_Date](./add_string_date/) | Создаёт новое пользовательское свойство документа типа данных <b>PropertyType.DateTime</b>. |
| [Add_String_Bool](./add_string_bool/) | Создаёт новое пользовательское свойство документа типа данных <b>PropertyType.Boolean</b>. |
| [Add_String_Double](./add_string_double/) | Создаёт новое пользовательское свойство документа типа данных <b>PropertyType.Float</b>. |
| [AddLinkToContent](./addlinktocontent/) | Создаёт новое пользовательское свойство документа, которое связывается с содержимым. |
| [UpdateLinkedPropertyValue](./updatelinkedpropertyvalue/) | Обновляет значения всех пользовательских свойств, связанных с содержимым (использует значение ячейки связанного диапазона для обновления значения пользовательского свойства). |
| [UpdateLinkedRange](./updatelinkedrange/) | Обновляет все диапазоны, связанные с пользовательскими свойствами (использует значение пользовательского свойства документа для обновления значения ячейки связанного диапазона). |
| [Get_Int](./get_int/) | Возвращает объект DocumentProperty по индексу. |
| [Contains](./contains/) | Возвращает true, если в коллекции существует свойство с указанным именем. |
| [IndexOf](./indexof/) | Получает индекс свойства по имени. |
| [Remove](./remove/) | Удаляет из коллекции свойство с указанным именем. |
| [RemoveAt](./removeat/) | Удаляет свойство по указанному индексу. |
| [GetCount](./getcount/) | Получает количество элементов, содержащихся в экземпляре. |
