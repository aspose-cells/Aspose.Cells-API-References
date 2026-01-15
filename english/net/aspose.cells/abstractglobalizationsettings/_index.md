---
title: Class AbstractGlobalizationSettings
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.AbstractGlobalizationSettings class. Represents the globalization settings
type: docs
url: /net/aspose.cells/abstractglobalizationsettings/
---
## AbstractGlobalizationSettings class

Represents the globalization settings.

```csharp
public abstract class AbstractGlobalizationSettings
```

## Methods

| Name | Description |
| --- | --- |
| virtual [Compare](../../aspose.cells/abstractglobalizationsettings/compare/)(string, string, bool) | Compares two string values according to certain collation rules. |
| virtual [GetCollationKey](../../aspose.cells/abstractglobalizationsettings/getcollationkey/)(string, bool) | Transforms the string into a comparable object according to certain collation rules. |

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsClassAbstractGlobalizationSettingsDemo
    {
        public static void Run()
        {
            // Create a custom implementation of AbstractGlobalizationSettings
            var customSettings = new CustomGlobalizationSettings();

            try
            {
                // Demonstrate the Compare method
                string str1 = "Hello";
                string str2 = "hello";
                bool ignoreCase = true;

                int comparisonResult = customSettings.Compare(str1, str2, ignoreCase);
                Console.WriteLine($"Comparison result ({str1} vs {str2}, ignoreCase={ignoreCase}): {comparisonResult}");

                // Demonstrate the GetCollationKey method
                string testString = "Sample";
                IComparable collationKey = customSettings.GetCollationKey(testString, ignoreCase);
                Console.WriteLine($"Collation key for '{testString}' (ignoreCase={ignoreCase}): {collationKey}");

                // Apply settings to a workbook
                Workbook workbook = new Workbook();
                workbook.Settings.GlobalizationSettings = customSettings;

                // Add some data to demonstrate the settings in action
                Worksheet worksheet = workbook.Worksheets[0];
                worksheet.Cells["A1"].PutValue("Apple");
                worksheet.Cells["A2"].PutValue("banana");
                worksheet.Cells["A3"].PutValue("Cherry");

                // Save the workbook
                workbook.Save("GlobalizationSettingsDemo.xlsx");
                Console.WriteLine("Workbook saved with custom globalization settings.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }

        private class CustomGlobalizationSettings : GlobalizationSettings
        {
            public override int Compare(string v1, string v2, bool ignoreCase)
            {
                return string.Compare(v1, v2, ignoreCase ? StringComparison.OrdinalIgnoreCase : StringComparison.Ordinal);
            }

            public override IComparable GetCollationKey(string v, bool ignoreCase)
            {
                return ignoreCase ? v.ToLowerInvariant() : v;
            }
        }
    }
}
```

### See Also

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


