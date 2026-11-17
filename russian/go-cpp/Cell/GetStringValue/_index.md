---
title: "GetStringValue Метод"
linktitle: "GetStringValue"
second_title: "Справочник API Aspose.Cells for Go через C++"
description: "GetStringValue метод. Инкапсулирует функцию, представляющую getstringvalue в Go."
type: docs
weight: 200
url: /ru/go-cpp/cell/getstringvalue/
---

## GetStringValue function

Получает строковое значение, содержащееся в ячейке. Если тип этой ячейки — строка, то возвращается само строковое значение. Для других типов ячеек будет возвращено отформатированное строковое значение (отформатированное согласно указанному стилю этой ячейки). Отформатированное значение ячейки совпадает с тем, что можно получить из Excel при копировании ячейки как текста (например, при копировании ячейки в текстовый редактор или экспорте в CSV).

```go

func (instance *Cell) GetStringValue()  (string,  error) 

```

## Примечания


## См. также

* Class [Cell](../)
* Library [Aspose.Cells for Go](../../)
