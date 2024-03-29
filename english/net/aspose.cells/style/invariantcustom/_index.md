---
title: Style.InvariantCustom
second_title: Aspose.Cells for .NET API Reference
description: Style property. Gets the cultureindependent pattern string for number format. If no number format has been set for this object null will be returned. If number format is builtin the pattern string corresponding to the builtin number will be returned
type: docs
url: /net/aspose.cells/style/invariantcustom/
---
## Style.InvariantCustom property

Gets the culture-independent pattern string for number format. If no number format has been set for this object, null will be returned. If number format is builtin, the pattern string corresponding to the builtin number will be returned.

```csharp
public string InvariantCustom { get; }
```

### Remarks

For builtin number formats, the returned pattern content is still culture-dependent, such as, for some locales it returns "m/d/y" and for some other locales it returns "d/m/y". The difference from [`CultureCustom`](../culturecustom/) is(that is also what culture-independent means): the format specifiers and separators are kept as standard, such as '/' will always be used as datetime separator and "y" will always be used as the "year" part no matter what other special character is used for the specific locale.

### See Also

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


