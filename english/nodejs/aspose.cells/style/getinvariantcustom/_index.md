---
title: "Style.getInvariantCustom"
linktitle: "getInvariantCustom"
second_title: "Aspose.Cells for Node.js via Java API Reference"
description: "Gets the culture-independent pattern string for number format."
type: docs
weight: 170
url: /nodejs/aspose.cells/style/getinvariantcustom/
---

## getInvariantCustom()

Gets the culture-independent pattern string for number format. If no number format has been set for this object, null will be returned. If number format is builtin, the pattern string corresponding to the builtin number will be returned. For builtin number formats, the returned pattern content is still culture-dependent, such as, for some locales it returns "m/d/y" and for some other locales it returns "d/m/y". The difference from CultureCustom is(that is also what culture-independent means): the format specifiers and separators are kept as standard, such as '/' will always be used as datetime separator and "y" will always be used as the "year" part no matter what other special character is used for the specific locale.
