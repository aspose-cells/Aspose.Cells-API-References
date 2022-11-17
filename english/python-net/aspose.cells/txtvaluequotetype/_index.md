---
title: TxtValueQuoteType
second_title: Aspose.Cells for Python via .NET API Reference
description: 
type: docs
weight: 5140
url: /python-net/aspose.cells/txtvaluequotetype/
---

## TxtValueQuoteType enumeration

Specifies the type of using quotation marks for values in text format files.

## Members
| Member name | Description |
| :- | :- |
|NORMAL|All values that contain special characters such as quotation mark, separator character will be quoted.<br/>            Same with the behavior of ms excel for exporting text file.|
|ALWAYS|All values will be quoted always.|
|MINIMUM|Only quote values when needed. Such as, if one value contains quotation mark but the quotation mark is not at the begin of this value, this value will not be quoted.|
|NEVER|All values will not be quoted. The exported text file with this type may not be read back correctly because the needed quotation marks being absent.|

### See Also

* namespace [aspose.cells](/cells/python-net/aspose.cells/)
* assembly [Aspose.Cells](/cells/python-net/)

