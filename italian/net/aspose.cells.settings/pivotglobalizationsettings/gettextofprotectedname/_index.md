---
title: "PivotGlobalizationSettings.GetTextOfProtectedName"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo PivotGlobalizationSettings. Ottiene il testo per il nome protetto specificato"
type: docs
url: /it/net/aspose.cells.settings/pivotglobalizationsettings/gettextofprotectedname/
---
## PivotGlobalizationSettings.GetTextOfProtectedName method

Restituisce il testo per il nome protetto specificato.

```csharp
public virtual string GetTextOfProtectedName(string protectedName)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| protectedName | String | Il nome protetto nella PivotTable. |

### Valore di ritorno

I nomi protetti locali della PivotTable.

### Osservazioni

In Ms Excel, alcuni nomi non possono essere usati come nome dei PivotField nella PivotTable. Sono diversi a seconda della regione; l'utente può specificarli esplicitamente in base alla regione utilizzata.

### Esempi

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
                // Crea un'istanza di PivotGlobalizationSettings
                PivotGlobalizationSettings globalizationSettings = new PivotGlobalizationSettings();

                // Definire un nome protetto per recuperare il suo testo
                string protectedName = "SensitiveData";

                // Chiamare il metodo GetTextOfProtectedName
                string result = globalizationSettings.GetTextOfProtectedName(protectedName);

                // Restituisci il risultato
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

### Vedi anche

* class [PivotGlobalizationSettings](../)
* namespace [Aspose.Cells.Settings](../../../aspose.cells.settings/)
* assembly [Aspose.Cells](../../../)


