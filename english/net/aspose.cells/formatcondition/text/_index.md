---
title: FormatCondition.Text
second_title: Aspose.Cells for .NET API Reference
description: FormatCondition property. The text value in a text contains conditional formatting rule. Valid only for type  containsText notContainsText beginsWith and endsWith. The default value is null
type: docs
url: /net/aspose.cells/formatcondition/text/
---
## FormatCondition.Text property

The text value in a "text contains" conditional formatting rule. Valid only for type = containsText, notContainsText, beginsWith and endsWith. The default value is null.

```csharp
public string Text { get; set; }
```

### Examples

```csharp
// Called: return fc.Text;
public object Property_Text(object dest)
            {
                FormatCondition fc = ((FormatConditionCollection)dest)[0];
                switch (fc.Type)
                {
                    case FormatConditionType.ContainsText:
                    case FormatConditionType.BeginsWith:
                    case FormatConditionType.EndsWith:
                    case FormatConditionType.NotContainsText:
                    {
                        return fc.Text;
                    }
                }
                return fc.Formula1;
            }
```

### See Also

* class [FormatCondition](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


