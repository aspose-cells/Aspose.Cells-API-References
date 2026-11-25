---
title: "SettableGlobalizationSettings.GetLocalBuiltInName"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo SettableGlobalizationSettings. Ottiene il testo dipendente dalla locale per il builtin Name secondo il testo standard fornito"
type: docs
url: /it/net/aspose.cells/settableglobalizationsettings/getlocalbuiltinname/
---
## SettableGlobalizationSettings.GetLocalBuiltInName method

Ottiene il testo dipendente dalla locale per il Nome incorporato in base al testo standard fornito.

```csharp
public override string GetLocalBuiltInName(string standardName)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| standardName | String | Testo Standard (locale en-US) del Nome incorporato. |

### Valore di ritorno

Testo dipendente dalla locale. La locale è stata specificata dalla Cartella di lavoro per la quale queste impostazioni sono utilizzate.

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettableGlobalizationSettingsMethodGetLocalBuiltInNameWithStringDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crea un'istanza di SettableGlobalizationSettings
            SettableGlobalizationSettings globalizationSettings = new SettableGlobalizationSettings();

            try
            {
                // Chiama il metodo GetLocalBuiltInName con un nome incorporato standard
                string standardName = "SUM";
                string localName = globalizationSettings.GetLocalBuiltInName(standardName);

                // Visualizza il risultato
                Console.WriteLine($"Standard name: {standardName}, Local name: {localName}");

                // Imposta un nome locale personalizzato per il nome incorporato standard
                globalizationSettings.SetLocalBuiltInName(standardName, "CustomSum", true);

                // Ottieni nuovamente il nome locale dopo averlo impostato
                localName = globalizationSettings.GetLocalBuiltInName(standardName);
                Console.WriteLine($"After setting - Standard name: {standardName}, Local name: {localName}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetLocalBuiltInName method: {ex.Message}");
            }

            // Salva la cartella di lavoro
            workbook.Save("MethodGetLocalBuiltInNameDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


