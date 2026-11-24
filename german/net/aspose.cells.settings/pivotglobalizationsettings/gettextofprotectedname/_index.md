---
title: "PivotGlobalizationSettings.GetTextOfProtectedName"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PivotGlobalizationSettings-Methode. Gibt den Text für den angegebenen geschützten Namen zurück"
type: docs
url: /de/net/aspose.cells.settings/pivotglobalizationsettings/gettextofprotectedname/
---
## PivotGlobalizationSettings.GetTextOfProtectedName method

Ermittelt den Text für den angegebenen geschützten Namen.

```csharp
public virtual string GetTextOfProtectedName(string protectedName)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| protectedName | String | Der geschützte Name in der PivotTable. |

### Rückgabewert

Die lokalen geschützten Namen der PivotTable.

### Hinweise

In Ms Excel dürfen einige Namen nicht als Name von PivotFields in einer PivotTable verwendet werden. Sie unterscheiden sich je nach Region; der Benutzer kann sie je nach verwendeter Region explizit angeben.

### Beispiele

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
                // Erstelle eine Instanz von PivotGlobalizationSettings
                PivotGlobalizationSettings globalizationSettings = new PivotGlobalizationSettings();

                // Definieren Sie einen geschützten Namen, um dessen Text abzurufen
                string protectedName = "SensitiveData";

                // Rufen Sie die Methode GetTextOfProtectedName auf
                string result = globalizationSettings.GetTextOfProtectedName(protectedName);

                // Gib das Ergebnis aus
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

### Siehe auch

* class [PivotGlobalizationSettings](../)
* namespace [Aspose.Cells.Settings](../../../aspose.cells.settings/)
* assembly [Aspose.Cells](../../../)


