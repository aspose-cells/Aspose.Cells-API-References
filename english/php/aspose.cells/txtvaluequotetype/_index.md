---
title: "TxtValueQuoteType Enum"
linktitle: "TxtValueQuoteType"
articleTitle: "TxtValueQuoteType"
second_title: "Aspose.Cells for PHP via Java"
description: "Utility class containing constants."
type: docs
weight: 7180
url: /php/aspose.cells/txtvaluequotetype/
---

## TxtValueQuoteType enumeration

Utility class containing constants. Specifies the type of using quotation marks for values in text format files.

## Values

| Name | Description |
| --- | --- |
| NORMAL | All values that contain special characters such as quotation mark, separator character will be quoted. Same with the behavior of ms excel for exporting text file. |
| ALWAYS | All values will be quoted always. |
| MINIMUM | Only quote values when needed. Such as, if one value contains quotation mark but the quotation mark is not at the begin of this value, this value will not be quoted. |
| NEVER | All values will not be quoted. The exported text file with this type may not be read back correctly because the needed quotation marks being absent. |
