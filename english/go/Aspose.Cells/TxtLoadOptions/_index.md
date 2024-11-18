---
title: TxtLoadOptions Class 
linktitle: TxtLoadOptions
second_title: Aspose.Cells for Go API Reference
description: 'TxtLoadOptions class. Encapsulates the object that represents txtloadoptions in Go.'
type: docs
weight: 200
url: /go/aspose.cells/txtloadoptions/
---

## TxtLoadOptions class

Represents the options for loading text file.

```go

type TxtLoadOptions struct 

txtloadoptions, _ := asposecells.NewTxtLoadOptions()

```

## Methods

| Method | Description |
| --- | --- |
|[IsNull](./isnull/) | Checks whether the implementation object is nullptr. | 
|[GetSeparator](./getseparator/) | Gets and sets character separator of text file. | 
|[SetSeparator](./setseparator/) | Gets and sets character separator of text file. | 
|[GetSeparatorString](./getseparatorstring/) | Gets and sets a string value as separator. | 
|[SetSeparatorString](./setseparatorstring/) | Gets and sets a string value as separator. | 
|[IsMultiEncoded](./ismultiencoded/) | True means that the file contains several encoding. | 
|[SetIsMultiEncoded](./setismultiencoded/) | True means that the file contains several encoding. | 
|[GetHasFormula](./gethasformula/) | Indicates whether the text is formula if it starts with "=". | 
|[SetHasFormula](./sethasformula/) | Indicates whether the text is formula if it starts with "=". | 
|[GetHasTextQualifier](./gethastextqualifier/) | Whether there is text qualifier for cell value. Default is true. | 
|[SetHasTextQualifier](./sethastextqualifier/) | Whether there is text qualifier for cell value. Default is true. | 
|[GetTextQualifier](./gettextqualifier/) | Specifies the text qualifier for cell values. Default qualifier is '"'. | 
|[SetTextQualifier](./settextqualifier/) | Specifies the text qualifier for cell values. Default qualifier is '"'. | 
|[GetTreatConsecutiveDelimitersAsOne](./gettreatconsecutivedelimitersasone/) | Whether consecutive delimiters should be treated as one. | 
|[SetTreatConsecutiveDelimitersAsOne](./settreatconsecutivedelimitersasone/) | Whether consecutive delimiters should be treated as one. | 
|[GetTreatQuotePrefixAsValue](./gettreatquoteprefixasvalue/) | Indicates whether the leading single quote sign should be taken as part of the value of one cell.Default is true. If it is false, the leading single quote will be removed from corresponding cell's valueand <see cref="Style.QuotePrefix"/> will be set as true for the cell. | 
|[SetTreatQuotePrefixAsValue](./settreatquoteprefixasvalue/) | Indicates whether the leading single quote sign should be taken as part of the value of one cell.Default is true. If it is false, the leading single quote will be removed from corresponding cell's valueand <see cref="Style.QuotePrefix"/> will be set as true for the cell. | 
|[GetExtendToNextSheet](./getextendtonextsheet/) | Whether extends data to next sheet when the rows or columns of data exceed limit.Default is false. | 
|[SetExtendToNextSheet](./setextendtonextsheet/) | Whether extends data to next sheet when the rows or columns of data exceed limit.Default is false. | 
|[GetHeaderRowsCount](./getheaderrowscount/) | The count of header rows to be repeated for extended sheets. | 
|[SetHeaderRowsCount](./setheaderrowscount/) | The count of header rows to be repeated for extended sheets. | 
|[GetHeaderColumnsCount](./getheadercolumnscount/) | The count of header columns to be repeated for extended sheets. | 
|[SetHeaderColumnsCount](./setheadercolumnscount/) | The count of header columns to be repeated for extended sheets. | 
|[GetMaxRowCount](./getmaxrowcount/) | The maximum count of rows to be imported for one sheet. | 
|[SetMaxRowCount](./setmaxrowcount/) | The maximum count of rows to be imported for one sheet. | 
|[GetMaxColumnCount](./getmaxcolumncount/) | The maximum count of columns to be imported for one sheet. | 
|[SetMaxColumnCount](./setmaxcolumncount/) | The maximum count of columns to be imported for one sheet. | 
|[GetEncoding](./getencoding/) | Gets and sets the default encoding. Only applies for csv file. | 
|[SetEncoding](./setencoding/) | Gets and sets the default encoding. Only applies for csv file. | 
|[GetLoadStyleStrategy](./getloadstylestrategy/) | Indicates the strategy to apply style for parsed values when converting string value to number or datetime. | 
|[SetLoadStyleStrategy](./setloadstylestrategy/) | Indicates the strategy to apply style for parsed values when converting string value to number or datetime. | 
|[GetConvertNumericData](./getconvertnumericdata/) | Gets or sets a value that indicates whether the string in text file is converted to numeric data. | 
|[SetConvertNumericData](./setconvertnumericdata/) | Gets or sets a value that indicates whether the string in text file is converted to numeric data. | 
|[GetConvertDateTimeData](./getconvertdatetimedata/) | Gets or sets a value that indicates whether the string in text file is converted to date data. | 
|[SetConvertDateTimeData](./setconvertdatetimedata/) | Gets or sets a value that indicates whether the string in text file is converted to date data. | 
|[GetKeepPrecision](./getkeepprecision/) | Indicates whether not parsing a string value if the length is 15. | 
|[SetKeepPrecision](./setkeepprecision/) | Indicates whether not parsing a string value if the length is 15. | 
