---
title: AutoFitterOptions.DefaultEditLanguage
second_title: Aspose.Cells for .NET API Reference
description: AutoFitterOptions property. Gets or sets default edit language
type: docs
url: /net/aspose.cells/autofitteroptions/defaulteditlanguage/
---
## AutoFitterOptions.DefaultEditLanguage property

Gets or sets default edit language.

```csharp
public DefaultEditLanguage DefaultEditLanguage { get; set; }
```

### Remarks

It may display/render different layouts for text paragraph when different edit languages is set. Default is Auto.

### Examples

```csharp
// Called: autoFitterOptions.DefaultEditLanguage = DefaultEditLanguage.CJK;
public static void AutoFitterOptions_Property_DefaultEditLanguage()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Create AutoFitterOptions and set DefaultEditLanguage
            AutoFitterOptions autoFitterOptions = new AutoFitterOptions();
            autoFitterOptions.DefaultEditLanguage = DefaultEditLanguage.CJK;

            // Apply auto fit rows with the specified options
            worksheet.AutoFitRows(autoFitterOptions);

            // Save the workbook
            workbook.Save("DefaultEditLanguageExample.xlsx");
            workbook.Save("DefaultEditLanguageExample.pdf");

            // Output the set DefaultEditLanguage to the console
            Console.WriteLine("Default Edit Language set to: " + autoFitterOptions.DefaultEditLanguage);
        }
```

### See Also

* enum [DefaultEditLanguage](../../defaulteditlanguage/)
* class [AutoFitterOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


