---
title: "CellsHelper_CreateSafeSheetName_String Метод"
linktitle: "CreateSafeSheetName"
second_title: "Справочник API Aspose.Cells for Go через C++"
description: "CellsHelper_CreateSafeSheetName_String метод. Инкапсулирует функцию, представляющую createsafesheetname в Go."
type: docs
weight: 200
url: /ru/go-cpp/cellshelper/cellshelper_createsafesheetname_string/
---

## CellsHelper_CreateSafeSheetName_String function

Проверяет указанное имя листа и при необходимости создает корректное. Если указанное имя листа соответствует правилам имен листов Excel, возвращает его. В противном случае строка будет усечена, если её длина превышает ограничение, а недопустимые символы будут заменены на ' ', затем возвращается восстановленное значение строки.

```go

func CellsHelper_CreateSafeSheetName_String(nameproposal string)  (string,  error) 

```

## Примечания


## См. также

* Class [CellsHelper](../)
* Library [Aspose.Cells for Go](../../)
