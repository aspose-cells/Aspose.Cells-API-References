---
title: "ConditionalFormattingValue Class"
linktitle: "ConditionalFormattingValue"
articleTitle: "ConditionalFormattingValue"
second_title: "Aspose.Cells for PHP via Java"
description: "Describes the values of the interpolation points in a gradient scale, dataBar or iconSet."
type: docs
weight: 1130
url: /php/aspose.cells/conditionalformattingvalue/
---

## ConditionalFormattingValue class

Describes the values of the interpolation points in a gradient scale, dataBar or iconSet.

## Properties

| Name | Type | Description |
| --- | --- | --- |
| [Value](#value) | Object | Get or set the value of this conditional formatting value object. It should be used in conjunction with Type. If the val |
| [Type](#type) | Number | Get or set the type of this conditional formatting value object. Setting the type to FormatConditionValueType.Min or For |
| [IsGTE](#isgte) | boolean | Get or set the Greater Than Or Equal flag. Use only for icon sets, determines whether this threshold value uses the grea |

### ConditionalFormattingValue.Value property {#value}

Get or set the value of this conditional formatting value object. It should be used in conjunction with Type. If the value is string and start with "=", it will be processed as a formula, otherwise we will process it as a simple value.

**Type:** Object

### ConditionalFormattingValue.Type property {#type}

Get or set the type of this conditional formatting value object. Setting the type to FormatConditionValueType.Min or FormatConditionValueType.Max will auto set "Value" to null. The value of the property is FormatConditionValueType integer constant.

**Type:** Number

### ConditionalFormattingValue.IsGTE property {#isgte}

Get or set the Greater Than Or Equal flag. Use only for icon sets, determines whether this threshold value uses the greater than or equal to operator. 'false' indicates 'greater than' is used instead of 'greater than or equal to'. Default value is true.

**Type:** boolean
