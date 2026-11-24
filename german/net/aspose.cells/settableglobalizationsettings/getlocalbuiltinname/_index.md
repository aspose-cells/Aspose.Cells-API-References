---
title: "SettableGlobalizationSettings.GetLocalBuiltInName"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "SettableGlobalizationSettings-Methode. Gibt den lokalisierungsabhängigen Text für den integrierten Namen gemäß dem angegebenen Standardtext zurück."
type: docs
url: /de/net/aspose.cells/settableglobalizationsettings/getlocalbuiltinname/
---
## SettableGlobalizationSettings.GetLocalBuiltInName method

Gibt den lokalisierungsabhängigen Text für den integrierten Namen gemäß dem angegebenen Standardtext zurück.

```csharp
public override string GetLocalBuiltInName(string standardName)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| standardName | String | Standard (en-US-Locale) Text des integrierten Namens. |

### Rückgabewert

Lokalisierungsabhängiger Text. Die Locale wurde vom Arbeitsbuch angegeben, für das diese Einstellungen verwendet werden.

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettableGlobalizationSettingsMethodGetLocalBuiltInNameWithStringDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Erstelle eine Instanz von SettableGlobalizationSettings
            SettableGlobalizationSettings globalizationSettings = new SettableGlobalizationSettings();

            try
            {
                // Rufe die GetLocalBuiltInName-Methode mit einem standardmäßigen integrierten Namen auf
                string standardName = "SUM";
                string localName = globalizationSettings.GetLocalBuiltInName(standardName);

                // Ergebnis anzeigen
                Console.WriteLine($"Standard name: {standardName}, Local name: {localName}");

                // Setze einen benutzerdefinierten lokalen Namen für den standardmäßigen integrierten Namen
                globalizationSettings.SetLocalBuiltInName(standardName, "CustomSum", true);

                // Rufe den lokalen Namen erneut ab, nachdem er gesetzt wurde
                localName = globalizationSettings.GetLocalBuiltInName(standardName);
                Console.WriteLine($"After setting - Standard name: {standardName}, Local name: {localName}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetLocalBuiltInName method: {ex.Message}");
            }

            // Speichere die Arbeitsmappe
            workbook.Save("MethodGetLocalBuiltInNameDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


