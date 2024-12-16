---
title: HtmlLoadOptions Class 
linktitle: HtmlLoadOptions
second_title: Aspose.Cells for Go via C++ API Reference
description: 'HtmlLoadOptions class. Encapsulates the object that represents htmlloadoptions in Go.'
type: docs
weight: 200
url: /go-cpp/htmlloadoptions/
---

## HtmlLoadOptions class

Represents options when importing a html file.

```go

type HtmlLoadOptions struct  {
	ptr unsafe.Pointer
}

```
## Constructors

| Method | Description |
| --- | --- |
|[NewHtmlLoadOptions](./newhtmlloadoptions/) | Creates an options of loading the file. | 
|[NewHtmlLoadOptions_LoadFormat](./newhtmlloadoptions_loadformat/) | Creates an options of loading the file. | 
|[NewHtmlLoadOptions_AbstractTextLoadOptions](./newhtmlloadoptions_abstracttextloadoptions/) | Constructs from a parent object. | 

## Methods

| Method | Description |
| --- | --- |
|[IsNull](./isnull/) | Checks whether the implementation object is nullptr. | 
|[GetLoadFormulas](./getloadformulas/) | Indicates whether importing formulas if the original html file contains formulas | 
|[SetLoadFormulas](./setloadformulas/) | Indicates whether importing formulas if the original html file contains formulas | 
|[GetSupportDivTag](./getsupportdivtag/) | Indicates whether support the layout of <c>&lt;div&gt;</c> tag when the html file contains it.The default value is false. | 
|[SetSupportDivTag](./setsupportdivtag/) | Indicates whether support the layout of <c>&lt;div&gt;</c> tag when the html file contains it.The default value is false. | 
|[GetDeleteRedundantSpaces](./getdeleteredundantspaces/) | Indicates whether delete redundant spaces when the text wraps lines using <c>&lt;br&gt;</c> tag.The default value is false. | 
|[SetDeleteRedundantSpaces](./setdeleteredundantspaces/) | Indicates whether delete redundant spaces when the text wraps lines using <c>&lt;br&gt;</c> tag.The default value is false. | 
|[GetAutoFitColsAndRows](./getautofitcolsandrows/) | Indicates whether auto-fit columns and rows. The default value is false. | 
|[SetAutoFitColsAndRows](./setautofitcolsandrows/) | Indicates whether auto-fit columns and rows. The default value is false. | 
|[GetHasFormula](./gethasformula/) | Indicates whether the text is formula if it starts with "=". | 
|[SetHasFormula](./sethasformula/) | Indicates whether the text is formula if it starts with "=". | 
|[GetProgId](./getprogid/) | Gets the program id of creating the file.Only for MHT files. | 
|[GetTableLoadOptions](./gettableloadoptions/) | Get the HtmlTableLoadOptionCollection instance | 
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
