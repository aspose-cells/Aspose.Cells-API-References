---
title: "Método CellsHelper_CreateSafeSheetName_String_Char"
linktitle: "CreateSafeSheetName"
second_title: "Aspose.Cells for Go via C++ API Reference"
description: "Método CellsHelper_CreateSafeSheetName_String_Char. Encapsula la función que representa createsafesheetname en Go."
type: docs
weight: 200
url: /es/go-cpp/cellshelper/cellshelper_createsafesheetname_string_char/
---

## CellsHelper_CreateSafeSheetName_String_Char function

Checks given sheet name and create a valid one when needed.If given sheet name conforms to the rules of excel sheet name, then return it.Otherwise string will be truncated if length exceeds the limitand invalid characters will be replaced with given character, then return the rebuilt string value.

```go

func CellsHelper_CreateSafeSheetName_String_Char(nameproposal string, replacechar byte)  (string,  error) 

```

## Observaciones


## Ver también

* Class [CellsHelper](../)
* Library [Aspose.Cells for Go](../../)
