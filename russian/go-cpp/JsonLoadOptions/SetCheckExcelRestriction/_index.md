---
title: "Метод SetCheckExcelRestriction"
linktitle: "SetCheckExcelRestriction"
second_title: "Справочник API Aspose.Cells for Go через C++"
description: "Метод SetCheckExcelRestriction. Инкапсулирует функцию, представляющую setcheckexcelrestriction в Go."
type: docs
weight: 200
url: /ru/go-cpp/jsonloadoptions/setcheckexcelrestriction/
---

## SetCheckExcelRestriction function

Определяет, проверять ли ограничения файла Excel, когда пользователь изменяет связанные с ячейками объекты. Например, Excel не позволяет вводить строковое значение длиной более 32 КБ. Если вы вводите значение длиной более 32 КБ, например с помощью Cell.PutValue(string), и это свойство установлено в true, будет выброшено исключение. Если свойство установлено в false, мы примем введённую строку как значение ячейки, чтобы позже вы могли вывести полное строковое значение в другие форматы файлов, такие как CSV. Однако, если вы задали значение, которое недействительно для формата Excel, не следует сохранять рабочую книгу в формате Excel позже. В противном случае может возникнуть непредвиденная ошибка в сгенерированном файле Excel.

```go

func (instance *JsonLoadOptions) SetCheckExcelRestriction(value bool)  error

```

## Примечания


## См. также

* Class [JsonLoadOptions](../)
* Library [Aspose.Cells for Go](../../)
