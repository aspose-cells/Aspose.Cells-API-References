---
title: CellsHelper_CreateSafeSheetName_String Method 
linktitle: CreateSafeSheetName
second_title: Aspose.Cells for Go API Reference
description: 'CellsHelper_CreateSafeSheetName_String method. Encapsulates the function that represents createsafesheetname in Go.'
type: docs
weight: 200
url: /go-cpp/cellshelper/cellshelper_createsafesheetname_string/
---

## CellsHelper_CreateSafeSheetName_String function

Checks given sheet name and create a valid one when needed.If given sheet name conforms to the rules of excel sheet name, then return it.Otherwise string will be truncated if length exceeds the limitand invalid characters will be replaced with ' ', then return the rebuilt string value.

```go

func CellsHelper_CreateSafeSheetName_String(nameproposal string)  (string,  error) 

```

## Remarks


## See Also

* Class [CellsHelper](../)
* Namespace [Aspose.Cells](../../)
* Library [Aspose.Cells for Go](../../../)
