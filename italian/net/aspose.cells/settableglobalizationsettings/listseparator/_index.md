---
title: "SettableGlobalizationSettings.ListSeparator"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà SettableGlobalizationSettings. Ottiene il separatore per i parametri elenco della funzione ...etc"
type: docs
url: /it/net/aspose.cells/settableglobalizationsettings/listseparator/
---
## SettableGlobalizationSettings.ListSeparator property

Ottiene il separatore per l'elenco, i parametri della funzione, ...etc.

```csharp
public override char ListSeparator { get; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettableGlobalizationSettingsPropertyListSeparatorDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Crea un'istanza di SettableGlobalizationSettings
            SettableGlobalizationSettings settings = new SettableGlobalizationSettings();
            
            // Visualizza il valore corrente di ListSeparator (il valore predefinito è la virgola nella maggior parte delle impostazioni locali)
            Console.WriteLine("Current ListSeparator value: " + settings.ListSeparator);
            
            // Imposta un nuovo valore di ListSeparator (ad es., punto e virgola)
            settings.SetListSeparator(';');
            
            // Applica le impostazioni alla cartella di lavoro
            workbook.Settings.GlobalizationSettings = settings;
            
            // Dimostra l'effetto di ListSeparator nell'analisi delle formule
            worksheet.Cells["A1"].PutValue("Test");
            worksheet.Cells["A2"].PutValue("Data");
            
            // Crea una formula che utilizza il separatore di elenco
            worksheet.Cells["A3"].Formula = "=CONCATENATE(A1,A2)";
            
            // La formula utilizzerà il separatore di elenco personalizzato durante l'analisi
            Console.WriteLine("Formula with custom separator: " + worksheet.Cells["A3"].Formula);
            
            // Salva la cartella di lavoro
            workbook.Save("PropertyListSeparatorDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


