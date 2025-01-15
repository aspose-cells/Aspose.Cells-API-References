---
title: SetHtmlCrossStringType Method 
linktitle: SetHtmlCrossStringType
second_title: Aspose.Cells for Go via C++ API Reference
description: 'SetHtmlCrossStringType method. Encapsulates the function that represents sethtmlcrossstringtype in Go.'
type: docs
weight: 200
url: /go-cpp/ebooksaveoptions/sethtmlcrossstringtype/
---

## SetHtmlCrossStringType function

Indicates if a cross-cell string will be displayed in the same way as MS Excel when saving an Excel file in html format.By default the value is Default, so, for cross-cell strings, there is little difference between the html files created by Aspose.Cells and MS Excel.But the performance for creating large html files,setting the value to Cross would be several times faster than setting it to Default or Fit2Cell.

```go

func (instance *EbookSaveOptions) SetHtmlCrossStringType(value HtmlCrossType)  error

```

## Remarks


## See Also

* Class [EbookSaveOptions](../)
* Library [Aspose.Cells for Go](../../)
