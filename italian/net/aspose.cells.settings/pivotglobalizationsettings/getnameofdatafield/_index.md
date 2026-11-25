---
title: "PivotGlobalizationSettings.GetNameOfDataField"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo PivotGlobalizationSettings. Ottiene il nome visualizzato del campo pivot dei dati. Il formato predefinito è Somma del Campo"
type: docs
url: /it/net/aspose.cells.settings/pivotglobalizationsettings/getnameofdatafield/
---
## PivotGlobalizationSettings.GetNameOfDataField method

Ottiene il nome visualizzato del campo pivot dei dati. Il formato predefinito è "Sum Of Field".

```csharp
public virtual string GetNameOfDataField(ConsolidationFunction function, string name)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| funzione | ConsolidationFunction | La funzione è usata per riassumere i valori del campo pivot. |
| name | String | Il nome originale del campo pivot. |

### Esempi

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
                // Crea un'istanza di PivotGlobalizationSettings
                PivotGlobalizationSettings globalizationSettings = new PivotGlobalizationSettings();

                // Definisci i parametri per il metodo GetNameOfDataField
                ConsolidationFunction function = ConsolidationFunction.Sum;
                string fieldName = "Sales";

                // Chiama il metodo GetNameOfDataField
                string result = globalizationSettings.GetNameOfDataField(function, fieldName);

                // Restituisci il risultato
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

### Vedi anche

* enum [ConsolidationFunction](../../../aspose.cells/consolidationfunction/)
* class [PivotGlobalizationSettings](../)
* namespace [Aspose.Cells.Settings](../../../aspose.cells.settings/)
* assembly [Aspose.Cells](../../../)


