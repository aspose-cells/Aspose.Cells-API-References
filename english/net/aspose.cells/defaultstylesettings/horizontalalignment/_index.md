---
title: DefaultStyleSettings.HorizontalAlignment
second_title: Aspose.Cells for .NET API Reference
description: DefaultStyleSettings property. Gets/Sets the default value for horizontal alignment
type: docs
url: /net/aspose.cells/defaultstylesettings/horizontalalignment/
---
## DefaultStyleSettings.HorizontalAlignment property

Gets/Sets the default value for horizontal alignment

```csharp
public TextAlignmentType HorizontalAlignment { get; set; }
```

### Examples

```csharp
// Called: defaultStyleSettings.HorizontalAlignment = TextAlignmentType.Center;
public static void DefaultStyleSettings_Property_HorizontalAlignment()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            
            // Access the default style settings of the workbook
            DefaultStyleSettings defaultStyleSettings = workbook.Settings.DefaultStyleSettings;

            // Setting properties
            defaultStyleSettings.BuiltInPreference = false;
            defaultStyleSettings.FontName = "Arial";
            defaultStyleSettings.FontSize = 12.0;
            defaultStyleSettings.HorizontalAlignment = TextAlignmentType.Center;
            defaultStyleSettings.VerticalAlignment = TextAlignmentType.Center;

            // Apply the default style settings to the first worksheet
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells.ApplyStyle(workbook.CreateStyle(), new StyleFlag() { All = true });

            // Save the workbook
            workbook.Save("DefaultStyleSettingsExample.xlsx");
            workbook.Save("DefaultStyleSettingsExample.pdf");

            return;
        }
```

### See Also

* enum [TextAlignmentType](../../textalignmenttype/)
* class [DefaultStyleSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


