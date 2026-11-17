---
title: "Перечисление DirectoryType"
linktitle: "DirectoryType"
second_title: "Справочник API Aspose.Cells for Go через C++"
description: "Перечисление DirectoryType. Инкапсулирует объект, представляющий тип каталога в Go."
type: docs
weight: 200
url: /ru/go-cpp/directorytype/
---

## DirectoryType Enum

Представляет тип каталога имени файла.

```go

type DirectoryType int32


```

## Поля

| Поле | Описание |
| --- | --- |
| [Volume](./volume/) | Представляет букву диска MS-DOS. За ней следует буква диска. Или имена UNC‑файлов, например \\server\share\myfile.xls |
| [SameVolume](./samevolume/) | Указывает, что исходная рабочая книга находится на том же диске, что и зависимая рабочая книга (буква диска опущена). |
| [DownDirectory](./downdirectory/) | Указывает, что исходная рабочая книга находится в подкаталоге текущего каталога. |
| [UpDirectory](./updirectory/) | Указывает, что исходная рабочая книга находится в родительском каталоге текущего каталога. |
