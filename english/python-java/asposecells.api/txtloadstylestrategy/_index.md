---
title: "TxtLoadStyleStrategy Enum"
linktitle: "TxtLoadStyleStrategy"
articleTitle: "TxtLoadStyleStrategy"
second_title: "Aspose.Cells for Python via Java"
description: "Utility class containing constants."
type: docs
weight: 7160
url: /python-java/asposecells.api/txtloadstylestrategy/
---

## TxtLoadStyleStrategy enumeration

Utility class containing constants. Specifies how to apply style for parsed values when converting string value to number or datetime.

## Values

| Name | Description |
| --- | --- |
| NONE | Does not set style for the parsed value. |
| BUILT_IN | Set the style as built-in number/datetime when the parsed value are plain numeric/datetime values. When ms excel parsing datetime or numeric values according to user's input(such as CSV file), the formatting of those values may be changed, such as leading/tailing zeros of number, year/month/day order of datetime, ...etc. This type is for simulating ms excel's behavior. |
| EXACT_FORMAT | Set the exact custom format for the parsed value to make the formatted value be same with the original input one. |
