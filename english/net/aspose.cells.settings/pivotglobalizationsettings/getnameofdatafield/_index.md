---
title: PivotGlobalizationSettings.GetNameOfDataField
second_title: Aspose.Cells for .NET API Reference
description: PivotGlobalizationSettings method. Gets the display name of data pivot field. The default format is Sum Of Field
type: docs
url: /net/aspose.cells.settings/pivotglobalizationsettings/getnameofdatafield/
---
## PivotGlobalizationSettings.GetNameOfDataField method

Gets the display name of data pivot field. The default format is "Sum Of Field".

```csharp
public virtual string GetNameOfDataField(ConsolidationFunction function, string name)
```

| Parameter | Type | Description |
| --- | --- | --- |
| function | ConsolidationFunction | The function is used to summarize values of pivot field. |
| name | String | The original name of the pivot field. |

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Settings;
    using System;

    public class PivotGlobalizationSettingsMethodGetNameOfDataFieldWithConsolidationFuStringDemo
    {
        public static void Run()
        {
            try
            {
                // Create an instance of PivotGlobalizationSettings
                PivotGlobalizationSettings globalizationSettings = new PivotGlobalizationSettings();

                // Define parameters for GetNameOfDataField method
                ConsolidationFunction function = ConsolidationFunction.Sum;
                string fieldName = "Sales";

                // Call the GetNameOfDataField method
                string result = globalizationSettings.GetNameOfDataField(function, fieldName);

                // Output the result
                Console.WriteLine($"Localized name for data field '{fieldName}' with function '{function}': {result}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling GetNameOfDataField: {ex.Message}");
            }
        }
    }
}
```

### See Also

* enum [ConsolidationFunction](../../../aspose.cells/consolidationfunction/)
* class [PivotGlobalizationSettings](../)
* namespace [Aspose.Cells.Settings](../../../aspose.cells.settings/)
* assembly [Aspose.Cells](../../../)


