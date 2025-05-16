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
namespace AsposeCellsExamples.CellsClassAbstractGlobalizationSettingsDemo
{
    using Aspose.Cells;
    using System;

    public class CellsClassAbstractGlobalizationSettingsDemo
    {
        public class CustomGlobalizationSettings : GlobalizationSettings
        {
            public override int Compare(string v1, string v2, bool ignoreCase)
            {
                return String.Compare(v1, v2, ignoreCase);
            }

            public override IComparable GetCollationKey(string v, bool ignoreCase)
            {
                return ignoreCase ? v.ToLower() : v;
            }
        }

        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            CustomGlobalizationSettings settings = new CustomGlobalizationSettings();
            workbook.Settings.GlobalizationSettings = settings;

            worksheet.Cells["A1"].PutValue("Apple");
            worksheet.Cells["A2"].PutValue("banana");
            worksheet.Cells["A3"].PutValue("Cherry");

            DataSorter sorter = workbook.DataSorter;
            sorter.Sort(worksheet.Cells, 0, 0, 2, 0);

            workbook.Save("AbstractGlobalizationSettingsDemo.xlsx");
        }
    }
}
```

### See Also

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


