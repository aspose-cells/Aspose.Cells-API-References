---
title: "Класс FileFormatInfo"
linktitle: "FileFormatInfo"
second_title: "Справочник API Aspose.Cells for Go через C++"
description: "Класс FileFormatInfo. Инкапсулирует объект, представляющий fileformatinfo в Go."
type: docs
weight: 200
url: /ru/go-cpp/fileformatinfo/
---

## FileFormatInfo class

Содержит данные, возвращаемые методами обнаружения формата файла <see cref="FileFormatUtil"/>.

```go

type FileFormatInfo struct  {
	ptr unsafe.Pointer
}

```
## Конструкторы

| Метод | Описание |
| --- | --- |
| [NewFileFormatInfo](./newfileformatinfo/) | Конструктор по умолчанию. |

## Методы

| Метод | Описание |
| --- | --- |
| [IsNull](./isnull/) | Проверяет, является ли объект реализации nullptr. |
| [IsProtectedByRMS](./isprotectedbyrms/) | Указывает, защищён ли файл сервером Microsoft Rights Management. |
| [IsEncrypted](./isencrypted/) | Возвращает true, если документ зашифрован и требует пароль для открытия. |
| [GetFileFormatType](./getfileformattype/) | Получает обнаруженный формат файла. |
| [GetLoadFormat](./getloadformat/) | Получает обнаруженный формат загрузки. |
