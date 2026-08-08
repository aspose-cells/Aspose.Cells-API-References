---
title: "Style.getCultureCustom"
linktitle: "getCultureCustom"
second_title: "Aspose.Cells for Node.js via Java API Reference"
description: "Gets and sets the culture-dependent pattern string for number format."
type: docs
weight: 90
url: /nodejs/aspose.cells/style/getculturecustom/
---

## getCultureCustom()

Gets and sets the culture-dependent pattern string for number format. If no number format has been set for this object, null will be returned. If number format is builtin, the pattern string corresponding to the builtin number will be returned. For builtin number format, both the pattern content(such as, one builtin date format is "m/d/y" for some locales, but for some other locales it becomes "d/m/y") and the format specifier(such as, some locales is using character other than 'y' to represent the year part for date formatting) are culture-dependent; For user specified custom format, only format specifiers are changed according to the culture, other parts of the formatting pattern will not be modified.
