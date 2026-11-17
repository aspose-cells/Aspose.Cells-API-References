---
title: "CellsHelper_CreateSafeSheetName_String Método"
linktitle: "CreateSafeSheetName"
second_title: "Aspose.Cells for Go via C++ API Reference"
description: "CellsHelper_CreateSafeSheetName_String método. Encapsula la función que representa createsafesheetname en Go."
type: docs
weight: 200
url: /es/go-cpp/cellshelper/cellshelper_createsafesheetname_string/
---

## CellsHelper_CreateSafeSheetName_String function

Checks given sheet name and create a valid one when needed.If given sheet name conforms to the rules of excel sheet name, then return it.Otherwise string will be truncated if length exceeds the limitand invalid characters will be replaced with ' ', then return the rebuilt string value.

```go

func CellsHelper_CreateSafeSheetName_String(nameproposal string)  (string,  error) 

```

## Observaciones


## Ver también

* Class [CellsHelper](../)
* Library [Aspose.Cells for Go](../../)
