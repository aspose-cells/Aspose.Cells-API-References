---
title: "Метод GetCheckExcelRestriction"
linktitle: "GetCheckExcelRestriction"
second_title: "Справочник API Aspose.Cells for Go через C++"
description: "Метод GetCheckExcelRestriction. Инкапсулирует функцию, представляющую getcheckexcelrestriction в Go."
type: docs
weight: 200
url: /ru/go-cpp/htmlloadoptions/getcheckexcelrestriction/
---

## GetCheckExcelRestriction function

Определяет, проверять ли ограничения файла Excel, когда пользователь изменяет связанные с ячейками объекты. Например, Excel не позволяет вводить строковое значение длиной более 32 КБ. Если вы вводите значение длиной более 32 КБ, например с помощью Cell.PutValue(string), и это свойство установлено в true, будет выброшено исключение. Если свойство установлено в false, мы примем введённую строку как значение ячейки, чтобы позже вы могли вывести полное строковое значение в другие форматы файлов, такие как CSV. Однако, если вы задали значение, которое недействительно для формата Excel, не следует сохранять рабочую книгу в формате Excel позже. В противном случае может возникнуть непредвиденная ошибка в сгенерированном файле Excel.

```go

func (instance *HtmlLoadOptions) GetCheckExcelRestriction()  (bool,  error) 

```

## Примечания


## См. также

* Class [HtmlLoadOptions](../)
* Library [Aspose.Cells for Go](../../)
