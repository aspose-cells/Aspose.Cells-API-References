---
title: Style.Name
second_title: Aspose.Cells for .NET API Reference
description: Style property. Gets or sets the name of the style
type: docs
url: /net/aspose.cells/style/name/
---
## Style.Name property

Gets or sets the name of the style.

```csharp
public string Name { get; set; }
```

### Examples

```csharp
// Called: boldStyle.Name = "CRMBoldStyle";
private static Style Property_Name(Workbook workbook)
        {

            Style boldStyle = workbook.GetNamedStyle("CRMBoldStyle");

            if (boldStyle == null)
            {
                boldStyle = workbook.CreateStyle();
                boldStyle.Name = "CRMBoldStyle";
                boldStyle.Font.IsBold = true;
            }

            return boldStyle;
        }
```

### See Also

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


