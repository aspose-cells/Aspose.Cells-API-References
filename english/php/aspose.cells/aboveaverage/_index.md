---
title: "AboveAverage Class"
linktitle: "AboveAverage"
articleTitle: "AboveAverage"
second_title: "Aspose.Cells for PHP via Java"
description: "Describe the AboveAverage conditional formatting rule."
type: docs
weight: 10
url: /php/aspose.cells/aboveaverage/
---

## AboveAverage class

Describe the AboveAverage conditional formatting rule. This conditional formatting rule highlights cells that are above or below the average for all values in the range.

## Constructors

| Name | Description |
| --- | --- |
| [AboveAverage](#constructor) |  |

## Properties

| Name | Type | Description |
| --- | --- | --- |
| [IsAboveAverage](#isaboveaverage) | boolean | Get or set the flag indicating whether the rule is an "above average" rule. 'true' indicates 'above average'. Default va |
| [IsEqualAverage](#isequalaverage) | boolean | Get or set the flag indicating whether the 'aboveAverage' and 'belowAverage' criteria is inclusive of the average itself |
| [StdDev](#stddev) | Number | Get or set the number of standard deviations to include above or below the average in the conditional formatting rule. T |

### AboveAverage() {#constructor}

### AboveAverage.IsAboveAverage property {#isaboveaverage}

Get or set the flag indicating whether the rule is an "above average" rule. 'true' indicates 'above average'. Default value is true.

**Type:** boolean

### AboveAverage.IsEqualAverage property {#isequalaverage}

Get or set the flag indicating whether the 'aboveAverage' and 'belowAverage' criteria is inclusive of the average itself, or exclusive of that value. 'true' indicates to include the average value in the criteria. Default value is false.

**Type:** boolean

### AboveAverage.StdDev property {#stddev}

Get or set the number of standard deviations to include above or below the average in the conditional formatting rule. The input value must between 0 and 3 (include 0 and 3). Setting this value to 0 means stdDev is not set. The default value is 0.

**Type:** Number
