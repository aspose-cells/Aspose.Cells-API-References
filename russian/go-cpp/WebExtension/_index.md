---
title: "Класс WebExtension"
linktitle: "WebExtension"
second_title: "Справочник API Aspose.Cells for Go через C++"
description: "Класс WebExtension. Инкапсулирует объект, представляющий webextension в Go."
type: docs
weight: 200
url: /ru/go-cpp/webextension/
---

## WebExtension class

Представляет экземпляр Office Add-in.

```go

type WebExtension struct  {
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
| [GetId](./getid/) | Получает и задает уникальный идентификатор экземпляра Office Add-in в текущем документе. |
| [SetId](./setid/) | Получает и задает уникальный идентификатор экземпляра Office Add-in в текущем документе. |
| [IsFrozen](./isfrozen/) | Указывает, может ли пользователь взаимодействовать с Office Add-in или нет. |
| [SetIsFrozen](./setisfrozen/) | Указывает, может ли пользователь взаимодействовать с Office Add-in или нет. |
| [GetReference](./getreference/) | Получить основную ссылку на Office Add-in. |
| [GetAlterReferences](./getalterreferences/) | Получает список альтернативных ссылок. |
| [GetProperties](./getproperties/) | Получает все свойства web extension. |
| [GetBindings](./getbindings/) | Получает все связи привязки между Office Add-in и данными в документе. |
