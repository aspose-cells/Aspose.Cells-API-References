---
title: "ConditionalFormattingValue"
linktitle: "ConditionalFormattingValue"
second_title: "Aspose.Cells for Node.js via Java API Reference"
description: "Describes the values of the interpolation points in a gradient scale, dataBar or iconSet."
type: docs
weight: 800
url: /nodejs/aspose.cells/conditionalformattingvalue/
---

## ConditionalFormattingValue class

Describes the values of the interpolation points in a gradient scale, dataBar or iconSet.

## Methods

| Name | Description |
| --- | --- |
| [getType()](#gettype) | Get or set the type of this conditional formatting value object. Setting the type to FormatConditionValueType.Min or For |
| [getValue()](#getvalue) | Get or set the value of this conditional formatting value object. It should be used in conjunction with Type. If the val |
| [isGTE()](#isgte) | Get or set the Greater Than Or Equal flag. Use only for icon sets, determines whether this threshold value uses the grea |
| [setGTE()](#setgte) | Get or set the Greater Than Or Equal flag. Use only for icon sets, determines whether this threshold value uses the grea |
| [setType()](#settype) | Get or set the type of this conditional formatting value object. Setting the type to FormatConditionValueType.Min or For |
| [setValue()](#setvalue) | Get or set the value of this conditional formatting value object. It should be used in conjunction with Type. If the val |

### getType() {#gettype}

Get or set the type of this conditional formatting value object. Setting the type to FormatConditionValueType.Min or FormatConditionValueType.Max will auto set "Value" to null. The value of the property is FormatConditionValueType integer constant.

### getValue() {#getvalue}

Get or set the value of this conditional formatting value object. It should be used in conjunction with Type. If the value is string and start with "=", it will be processed as a formula, otherwise we will process it as a simple value.

### isGTE() {#isgte}

Get or set the Greater Than Or Equal flag. Use only for icon sets, determines whether this threshold value uses the greater than or equal to operator. 'false' indicates 'greater than' is used instead of 'greater than or equal to'. Default value is true.

### setGTE() {#setgte}

Get or set the Greater Than Or Equal flag. Use only for icon sets, determines whether this threshold value uses the greater than or equal to operator. 'false' indicates 'greater than' is used instead of 'greater than or equal to'. Default value is true.

### setType() {#settype}

Get or set the type of this conditional formatting value object. Setting the type to FormatConditionValueType.Min or FormatConditionValueType.Max will auto set "Value" to null. The value of the property is FormatConditionValueType integer constant.

### setValue() {#setvalue}

Get or set the value of this conditional formatting value object. It should be used in conjunction with Type. If the value is string and start with "=", it will be processed as a formula, otherwise we will process it as a simple value.
