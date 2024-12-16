---
title: GetExcludeUnusedStyles Method 
linktitle: GetExcludeUnusedStyles
second_title: Aspose.Cells for Go via C++ API Reference
description: 'GetExcludeUnusedStyles method. Encapsulates the function that represents getexcludeunusedstyles in Go.'
type: docs
weight: 200
url: /go-cpp/ebooksaveoptions/getexcludeunusedstyles/
---

## GetExcludeUnusedStyles function

Indicating whether excludes unused styles.For the generated html files, excluding unused styles can make the file size smallerwithout affecting the visual effects. So the default value of this property is true.If user needs to keep all styles in the workbook for the generated html(such as the scenario that userneeds to restore the workbook from the generated html later), please set this property as false.

```go

func (instance *EbookSaveOptions) GetExcludeUnusedStyles()  (bool,  error) 

```

## Remarks


## See Also

* Class [EbookSaveOptions](../)
* Namespace [Aspose.Cells.Saving](../../)
* Library [Aspose.Cells for Go](../../../)
