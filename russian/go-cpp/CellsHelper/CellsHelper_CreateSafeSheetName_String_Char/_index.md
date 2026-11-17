---
title: "CellsHelper_CreateSafeSheetName_String_Char Метод"
linktitle: "CreateSafeSheetName"
second_title: "Справочник API Aspose.Cells for Go через C++"
description: "Метод CellsHelper_CreateSafeSheetName_String_Char. Инкапсулирует функцию, представляющую createsafesheetname в Go."
type: docs
weight: 200
url: /ru/go-cpp/cellshelper/cellshelper_createsafesheetname_string_char/
---

## CellsHelper_CreateSafeSheetName_String_Char function

Проверяет указанное имя листа и при необходимости создает корректное. Если указанное имя листа соответствует правилам имен листов Excel, возвращает его. В противном случае строка будет усечена, если её длина превышает ограничение, а недопустимые символы будут заменены заданным символом, затем возвращается восстановленное значение строки.

```go

func CellsHelper_CreateSafeSheetName_String_Char(nameproposal string, replacechar byte)  (string,  error) 

```

## Примечания


## См. также

* Class [CellsHelper](../)
* Library [Aspose.Cells for Go](../../)
