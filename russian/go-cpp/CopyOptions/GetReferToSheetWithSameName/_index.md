---
title: "Метод GetReferToSheetWithSameName"
linktitle: "GetReferToSheetWithSameName"
second_title: "Справочник API Aspose.Cells for Go через C++"
description: "GetReferToSheetWithSameName метод. Инкапсулирует функцию, представляющую getrefertosheetwithsamename в Go."
type: docs
weight: 200
url: /ru/go-cpp/copyoptions/getrefertosheetwithsamename/
---

## GetReferToSheetWithSameName function

В MS Excel при копировании формул, которые ссылаются на другие листы, при копировании листа в другой лист, скопированные формулы должны ссылаться на исходную книгу. Однако в некоторых ситуациях пользователю может потребоваться, чтобы скопированные формулы ссылались на листы с тем же именем в той же книге, например когда эти листы были скопированы до этой операции копирования; тогда это свойство должно быть установлено в значение true.

```go

func (instance *CopyOptions) GetReferToSheetWithSameName()  (bool,  error) 

```

## Примечания


## См. также

* Class [CopyOptions](../)
* Library [Aspose.Cells for Go](../../)
