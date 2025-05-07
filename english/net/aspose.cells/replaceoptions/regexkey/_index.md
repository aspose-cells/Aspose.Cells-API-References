---
title: ReplaceOptions.RegexKey
second_title: Aspose.Cells for .NET API Reference
description: ReplaceOptions property. Indicates whether the searched key is regex. If true then the searched key will be taken as regex
type: docs
url: /net/aspose.cells/replaceoptions/regexkey/
---
## ReplaceOptions.RegexKey property

Indicates whether the searched key is regex. If true then the searched key will be taken as regex.

```csharp
public bool RegexKey { get; set; }
```

### Examples

```csharp
// Called: RegexKey = false
public static void Property_RegexKey()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Add some sample data to the worksheet
            sheet.Cells["A1"].PutValue("Hello World");
            sheet.Cells["A2"].PutValue("Hello Aspose");
            sheet.Cells["A3"].PutValue("Goodbye World");

            // Create ReplaceOptions
            ReplaceOptions options = new ReplaceOptions
            {
                CaseSensitive = false,
                MatchEntireCellContents = false,
                RegexKey = false
            };

            // Replace "Hello" with "Hi" in the worksheet
            int replacedCount = workbook.Replace("Hello", "Hi", options);

            // Output the number of replacements made
            Console.WriteLine($"Number of replacements made: {replacedCount}");

            // Save the workbook
            workbook.Save("ReplaceOptionsExample.xlsx");
        }
```

### See Also

* class [ReplaceOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


