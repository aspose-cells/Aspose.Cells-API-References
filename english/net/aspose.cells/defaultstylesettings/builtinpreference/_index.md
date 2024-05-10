---
title: DefaultStyleSettings.BuiltInPreference
second_title: Aspose.Cells for .NET API Reference
description: DefaultStyleSettings property. Indicates whether property for number format is preferrable when the style defines both builtin number and custom pattern. Default value is false that means by default custom pattern will be used to format values as long as it is not empty for one style
type: docs
url: /net/aspose.cells/defaultstylesettings/builtinpreference/
---
## DefaultStyleSettings.BuiltInPreference property

Indicates whether property for number format is preferrable when the style defines both built-in number and custom pattern. Default value is false, that means by default custom pattern will be used to format values as long as it is not empty for one style.

```csharp
public bool BuiltInPreference { get; set; }
```

### Remarks

When loading workbook from existing template file, maybe both built-in number and custom pattern are defined for one style. This property determine whether we should use the built-in number or the custom pattern when formatting values with the style.

### See Also

* class [DefaultStyleSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


