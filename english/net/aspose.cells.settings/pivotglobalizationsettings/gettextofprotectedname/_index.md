---
title: PivotGlobalizationSettings.GetTextOfProtectedName
second_title: Aspose.Cells for .NET API Reference
description: PivotGlobalizationSettings method. Gets the text for specified protected name
type: docs
url: /net/aspose.cells.settings/pivotglobalizationsettings/gettextofprotectedname/
---
## PivotGlobalizationSettings.GetTextOfProtectedName method

Gets the text for specified protected name.

```csharp
public virtual string GetTextOfProtectedName(string protectedName)
```

| Parameter | Type | Description |
| --- | --- | --- |
| protectedName | String | The protected name in PivotTable. |

### Return Value

The local prorected names of PivotTable.

### Remarks

In Ms Excel, some names are not allowed to be used as the name of PivotFields in PivotTable. They are different in different region, user may specify them explicitly according to the used region.

### Examples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Settings;

namespace AsposeCellsExamples
{
    public class PivotGlobalizationSettingsMethodGetTextOfProtectedNameWithStringDemo
    {
        public static void Run()
        {
            try
            {
                // Create an instance of PivotGlobalizationSettings
                PivotGlobalizationSettings globalizationSettings = new PivotGlobalizationSettings();

                // Define a protected name to retrieve its text
                string protectedName = "SensitiveData";

                // Call the GetTextOfProtectedName method
                string result = globalizationSettings.GetTextOfProtectedName(protectedName);

                // Output the result
                Console.WriteLine($"Text for protected name \"{protectedName}\": {result}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling GetTextOfProtectedName: {ex.Message}");
            }
        }
    }
}
```

### See Also

* class [PivotGlobalizationSettings](../)
* namespace [Aspose.Cells.Settings](../../../aspose.cells.settings/)
* assembly [Aspose.Cells](../../../)


