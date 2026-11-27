---
title: "PivotGlobalizationSettings.GetTextOfProtectedName"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PivotGlobalizationSettings-metoden. Hämtar texten för angivet skyddat namn"
type: docs
url: /sv/net/aspose.cells.settings/pivotglobalizationsettings/gettextofprotectedname/
---
## PivotGlobalizationSettings.GetTextOfProtectedName method

Hämtar texten för angivet skyddat namn.

```csharp
public virtual string GetTextOfProtectedName(string protectedName)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| protectedName | String | Det skyddade namnet i pivottabellen. |

### Returvärde

De lokala skyddade namnen i pivottabellen.

### Anmärkningar

I Ms Excel är vissa namn inte tillåtna att användas som namn på PivotFields i en pivottabell. De varierar mellan regioner, och användaren kan ange dem explicit enligt den använda regionen.

### Exempel

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
                // Skapa en instans av PivotGlobalizationSettings
                PivotGlobalizationSettings globalizationSettings = new PivotGlobalizationSettings();

                // Definiera ett skyddat namn för att hämta dess text
                string protectedName = "SensitiveData";

                // Anropa GetTextOfProtectedName-metoden
                string result = globalizationSettings.GetTextOfProtectedName(protectedName);

                // Skriv ut resultatet
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

### Se även

* class [PivotGlobalizationSettings](../)
* namespace [Aspose.Cells.Settings](../../../aspose.cells.settings/)
* assembly [Aspose.Cells](../../../)


