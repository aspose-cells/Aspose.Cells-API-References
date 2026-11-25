---
title: "GlobalizationSettings.GetProtectionNameOfPivotTable"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo GlobalizationSettings. Ottiene il nome di protezione nella PivotTable"
type: docs
url: /it/net/aspose.cells/globalizationsettings/getprotectionnameofpivottable/
---
## GlobalizationSettings.GetProtectionNameOfPivotTable method

Ottiene il nome di protezione nella PivotTable.

```csharp
[Obsolete("Use PivotGlobalizationSettings.GetTextOfProtectedName(string) method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public virtual string GetProtectionNameOfPivotTable()
```

### Valore di ritorno

Il nome di protezione della PivotTable

### Osservazioni

NOTA: Questo membro è ora obsoleto. Invece, si prega di utilizzare il metodo PivotGlobalizationSettings.GetTextOfProtectedName(string). Questa proprietà sarà rimossa tra 12 mesi a partire da dicembre 2022. Aspose si scusa per qualsiasi inconveniente tu possa aver sperimentato.

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class GlobalizationSettingsMethodGetProtectionNameOfPivotTableDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Crea impostazioni di globalizzazione standard
            GlobalizationSettings standardSettings = new GlobalizationSettings();
            
            // Crea impostazioni di globalizzazione personalizzate
            GlobalizationSettings customSettings = new CustomGlobalizationSettings();
            workbook.Settings.GlobalizationSettings = customSettings;

            try
            {
                // Ottieni il nome di protezione predefinito
                string defaultName = standardSettings.GetProtectionNameOfPivotTable();
                Console.WriteLine($"Default protection name: {defaultName}");

                // Ottieni il nome di protezione personalizzato
                string customName = customSettings.GetProtectionNameOfPivotTable();
                Console.WriteLine($"Custom protection name: {customName}");

                // Crea una tabella pivot per dimostrare l'applicazione delle impostazioni
                worksheet.Cells["A1"].Value = "Data";
                worksheet.Cells["A2"].Value = 1;
                worksheet.Cells["A3"].Value = 2;
                worksheet.Cells["A4"].Value = 3;
                int pivotIndex = worksheet.PivotTables.Add("A1", "A1:A4", "PivotTable");
                PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
                
                // La protezione verrebbe tipicamente applicata qui usando il nome recuperato
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetProtectionNameOfPivotTable: {ex.Message}");
            }
            
            workbook.Save("GlobalizationSettingsMethodGetProtectionNameOfPivotTableDemo.xlsx");
        }
    }

    public class CustomGlobalizationSettings : GlobalizationSettings
    {
        public new string GetProtectionNameOfPivotTable()
        {
            return "CustomPivotProtection";
        }
    }
}
```

### Vedi anche

* class [GlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


