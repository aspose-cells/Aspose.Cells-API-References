---
title: "GlobalizationSettings.GetLocalBuiltInName"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo GlobalizationSettings. Ottiene il testo dipendente dalla locale per il nome incorporato secondo il testo standard fornito"
type: docs
url: /it/net/aspose.cells/globalizationsettings/getlocalbuiltinname/
---
## GlobalizationSettings.GetLocalBuiltInName method

Ottiene il testo dipendente dalla locale per il Nome incorporato in base al testo standard fornito.

```csharp
public virtual string GetLocalBuiltInName(string standardName)
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

    public class GlobalizationSettingsMethodGetLocalBuiltInNameWithStringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            workbook.Settings.GlobalizationSettings = new CustomGlobalizationSettings();

            try
            {
                string standardName = "Total";
                string localizedName = ((CustomGlobalizationSettings)workbook.Settings.GlobalizationSettings).GetLocalBuiltInName(standardName);

                Console.WriteLine($"Standard Name: {standardName}");
                Console.WriteLine($"Localized Name: {localizedName}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetLocalBuiltInName method: {ex.Message}");
            }

            workbook.Save("LocalizedBuiltInNameDemo.xlsx");
        }
    }

    public class CustomGlobalizationSettings : GlobalizationSettings
    {
        public override string GetLocalBuiltInName(string standardName)
        {
            switch (standardName)
            {
                case "Total":
                    return "LocalizedTotal";
                case "Average":
                    return "LocalizedAverage";
                default:
                    return base.GetLocalBuiltInName(standardName);
            }
        }
    }
}
```

### Vedi anche

* class [GlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


