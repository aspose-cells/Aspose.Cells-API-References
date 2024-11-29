---
title: EbookLoadOptions Class 
linktitle: EbookLoadOptions
second_title: Aspose.Cells for Go API Reference
description: 'EbookLoadOptions class. Encapsulates the object that represents ebookloadoptions in Go.'
type: docs
weight: 200
url: /go/ebookloadoptions/
---

## EbookLoadOptions class

Represents options when importing an ebook file.

```go

type EbookLoadOptions struct  {
	ptr unsafe.Pointer
}

```
## Constructors

| Method | Description |
| --- | --- |
|[NewEbookLoadOptions](./newebookloadoptions/) | Creates an options of loading the ebook file. | 
|[NewEbookLoadOptions_LoadFormat](./newebookloadoptions_loadformat/) | Creates an options of loading the ebook file. | 
|[NewEbookLoadOptions_HtmlLoadOptions](./newebookloadoptions_htmlloadoptions/) | Constructs from a parent object. | 

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
