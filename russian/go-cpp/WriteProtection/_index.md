---
title: "Класс WriteProtection"
linktitle: "WriteProtection"
second_title: "Справочник API Aspose.Cells for Go через C++"
description: "Класс WriteProtection. Инкапсулирует объект, представляющий writeprotection в Go."
type: docs
weight: 200
url: /ru/go-cpp/writeprotection/
---

## WriteProtection class

Указывает параметры защиты от записи для рабочей книги.

```go

type WriteProtection struct  {
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
| [GetAuthor](./getauthor/) | Получает и задает автора. |
| [SetAuthor](./setauthor/) | Получает и задает автора. |
| [GetRecommendReadOnly](./getrecommendreadonly/) | Указывает, выбрана ли опция «Только чтение рекомендуется». |
| [SetRecommendReadOnly](./setrecommendreadonly/) | Указывает, выбрана ли опция «Только чтение рекомендуется». |
| [IsWriteProtected](./iswriteprotected/) | Указывает, защищена ли эта книга записываемой защитой. |
| [GetPassword](./getpassword/) | Устанавливает защищённый пароль для изменения файла. |
| [SetPassword](./setpassword/) | Устанавливает защищённый пароль для изменения файла. |
| [ValidatePassword](./validatepassword/) | Возвращает true, если указанный пароль совпадает с паролем записи, которым файл был защищён. |
