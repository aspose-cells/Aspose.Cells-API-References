---
title: LoadOptions.StandardFont
second_title: Aspose.Cells for .NET API Reference
description: LoadOptions property. Sets the default standard font name
type: docs
url: /net/aspose.cells/loadoptions/standardfont/
---
## LoadOptions.StandardFont property

Sets the default standard font name

```csharp
[Obsolete("Use DefaultStyleSettings.FontName property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public string StandardFont { get; set; }
```

### Remarks

NOTE: This member is now obsolete. Instead, please use DefaultStyleSettings. This property will be removed 12 months later since March 2022. Aspose apologizes for any inconvenience you may have experienced.

### Examples

```csharp
// Called: loadOptions.StandardFont = "SimSun";
private Workbook LoadOptions_Property_StandardFont(Stream fileInputStream)
        {
            LoadOptions loadOptions = new LoadOptions();
            loadOptions.StandardFont = "SimSun";
            loadOptions.MemorySetting = MemorySetting.MemoryPreference;
            Workbook result = null;
            try
            {
                result = new Workbook(fileInputStream, loadOptions);
            }
            catch (Exception e)
            {

            }
            return result;
        }
```

### See Also

* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


