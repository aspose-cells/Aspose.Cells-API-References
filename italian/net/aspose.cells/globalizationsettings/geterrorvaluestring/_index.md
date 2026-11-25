---
title: "GlobalizationSettings.GetErrorValueString"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo GlobalizationSettings. Ottiene il valore stringa da visualizzare per il valore di errore delle celle"
type: docs
url: /it/net/aspose.cells/globalizationsettings/geterrorvaluestring/
---
## GlobalizationSettings.GetErrorValueString method

Ottiene il valore stringa visualizzato per il valore di errore della cella

```csharp
public virtual string GetErrorValueString(string err)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| err | String | valori di errore come #VALUE!,#NAME? |

### Valore di ritorno

Per impostazione predefinita restituisce il valore di errore stesso

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class GlobalizationSettingsMethodGetErrorValueStringWithStringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Imposta impostazioni di globalizzazione personalizzate
            workbook.Settings.GlobalizationSettings = new CustomErrorGlobalizationSettings();

            // Creare scenario di errore: divisione per zero
            Cell cell = worksheet.Cells["A1"];
            cell.Formula = "=1/0";  // This will generate #DIV/0! error

            try
            {
                workbook.CalculateFormula();
                string errorValue = cell.DisplayStringValue;
                
                Console.WriteLine($"Error display value: {errorValue}");
                Console.WriteLine("Method executed successfully - see custom error mapping");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetErrorValueString method: {ex.Message}");
            }

            workbook.Save("MethodGetErrorValueStringDemo.xlsx");
        }
    }

    public class CustomErrorGlobalizationSettings : GlobalizationSettings
    {
        public override string GetErrorValueString(string err)
        {
            // Mappature personalizzate dei valori di errore
            return err switch
            {
                "#DIV/0!" => "Custom Division Error",
                "#VALUE!" => "Custom Type Mismatch",
                "#NAME?" => "Custom Identifier Error",
                _ => base.GetErrorValueString(err)
            };
        }
    }
}
```

### Vedi anche

* class [GlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


