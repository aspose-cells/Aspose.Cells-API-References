---
title: "Класс VbaProject"
linktitle: "VbaProject"
second_title: "Справочник API Aspose.Cells for Go через C++"
description: "Класс VbaProject. Инкапсулирует объект, представляющий VbaProject в Go."
type: docs
weight: 200
url: /ru/go-cpp/vbaproject/
---

## VbaProject class

Представляет проект VBA.

```go

type VbaProject struct  {
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
| [Sign](./sign/) | Подписать этот проект VBA цифровой подписью. |
| [IsValidSigned](./isvalidsigned/) | Указывает, действительна ли подпись проекта VBA. |
| [GetCertRawData](./getcertrawdata/) | Получает необработанные данные сертификата, если этот проект VBA подписан. |
| [GetEncoding](./getencoding/) | Получает и задает кодировку проекта VBA. |
| [SetEncoding](./setencoding/) | Получает и задает кодировку проекта VBA. |
| [GetName](./getname/) | Получает и задает имя проекта VBA. |
| [SetName](./setname/) | Получает и задает имя проекта VBA. |
| [IsSigned](./issigned/) | Указывает, подписан ли код VBA. |
| [Protect](./protect/) | Защищает или снимает защиту с этого проекта VBA. |
| [IsProtected](./isprotected/) | Указывает, защищён ли этот проект VBA. |
| [IsLockedForView](./islockedforview/) | Указывает, заблокирован ли этот проект VBA для просмотра. Если true, код не будет виден. |
| [Copy](./copy/) | Скопировать проект VBA из другого файла. |
| [GetModules](./getmodules/) | Получает все объекты VbaModule. |
| [GetReferences](./getreferences/) | Получает все ссылки проекта VBA. |
| [ValidatePassword](./validatepassword/) | Проверяет пароль защиты. |
