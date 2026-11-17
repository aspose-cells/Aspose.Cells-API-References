---
title: "Метод GetExcludeUnusedStyles"
linktitle: "GetExcludeUnusedStyles"
second_title: "Справочник API Aspose.Cells for Go через C++"
description: "Метод GetExcludeUnusedStyles. Инкапсулирует функцию, представляющую getexcludeunusedstyles в Go."
type: docs
weight: 200
url: /ru/go-cpp/ebooksaveoptions/getexcludeunusedstyles/
---

## GetExcludeUnusedStyles function

Указывает, исключать ли неиспользуемые стили. Для генерируемых HTML‑файлов исключение неиспользуемых стилей может уменьшить размер файла без влияния на визуальные эффекты. Поэтому значение по умолчанию этого свойства — true. Если пользователю необходимо сохранить все стили в рабочей книге для генерируемого HTML (например, в сценарии, когда пользователь позже восстанавливает рабочую книгу из сгенерированного HTML), установите это свойство в false.

```go

func (instance *EbookSaveOptions) GetExcludeUnusedStyles()  (bool,  error) 

```

## Примечания


## См. также

* Class [EbookSaveOptions](../)
* Library [Aspose.Cells for Go](../../)
