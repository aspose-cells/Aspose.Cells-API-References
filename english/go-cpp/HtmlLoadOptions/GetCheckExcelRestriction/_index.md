---
title: GetCheckExcelRestriction Method 
linktitle: GetCheckExcelRestriction
second_title: Aspose.Cells for Go via C++ API Reference
description: 'GetCheckExcelRestriction method. Encapsulates the function that represents getcheckexcelrestriction in Go.'
type: docs
weight: 200
url: /go-cpp/htmlloadoptions/getcheckexcelrestriction/
---

## GetCheckExcelRestriction function

Whether check restriction of excel file when user modify cells related objects.For example, excel does not allow inputting string value longer than 32K.When you input a value longer than 32K such as by Cell.PutValue(string), if this property is true, you will get an Exception.If this property is false, we will accept your input string value as the cell's value so that lateryou can output the complete string value for other file formats such as CSV.However, if you have set such kind of value that is invalid for excel file format,you should not save the workbook as excel file format later. Otherwise there may be unexpected error for the generated excel file.

```go

func (instance *HtmlLoadOptions) GetCheckExcelRestriction()  (bool,  error) 

```

## Remarks


## See Also

* Class [HtmlLoadOptions](../)
* Library [Aspose.Cells for Go](../../)
