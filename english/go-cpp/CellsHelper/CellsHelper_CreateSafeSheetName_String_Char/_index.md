---
title: CellsHelper_CreateSafeSheetName_String_Char Method 
linktitle: CreateSafeSheetName
second_title: Aspose.Cells for Go API Reference
description: 'CellsHelper_CreateSafeSheetName_String_Char method. Encapsulates the function that represents createsafesheetname in Go.'
type: docs
weight: 200
url: /go/cellshelper/cellshelper_createsafesheetname_string_char/
---

## CellsHelper_CreateSafeSheetName_String_Char function

Checks given sheet name and create a valid one when needed.If given sheet name conforms to the rules of excel sheet name, then return it.Otherwise string will be truncated if length exceeds the limitand invalid characters will be replaced with given character, then return the rebuilt string value.

```go

func CellsHelper_CreateSafeSheetName_String_Char(nameproposal string, replacechar byte)  (string,  error) 

```

## Remarks


## See Also

* Class [CellsHelper](../)
* Namespace [Aspose.Cells](../../)
* Library [Aspose.Cells for Go](../../../)
