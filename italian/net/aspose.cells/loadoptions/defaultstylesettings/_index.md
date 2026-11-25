---
title: "LoadOptions.DefaultStyleSettings"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà LoadOptions. Ottiene le impostazioni di stile predefinite per l'inizializzazione degli stili della cartella di lavoro"
type: docs
url: /it/net/aspose.cells/loadoptions/defaultstylesettings/
---
## LoadOptions.DefaultStyleSettings property

Ottiene le impostazioni di stile predefinite per l'inizializzazione degli stili della cartella di lavoro

```csharp
public DefaultStyleSettings DefaultStyleSettings { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class LoadOptionsPropertyDefaultStyleSettingsDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Imposta le opzioni di caricamento con le impostazioni di stile predefinite
            LoadOptions loadOptions = new LoadOptions(LoadFormat.Xlsx);
            loadOptions.DefaultStyleSettings.VerticalAlignment = TextAlignmentType.Bottom;
            
            // Crea un foglio di lavoro e ottieni le celle
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;
            
            // Imposta valori per dimostrare lo stile predefinito
            cells["A1"].PutValue("Default Style Applied");
            cells["A2"].PutValue("Should have bottom alignment");
            
            // Crea una cella con stile personalizzato (per confrontarlo con quello predefinito)
            Cell customCell = cells["B1"];
            customCell.PutValue("Custom Style");
            Style customStyle = customCell.GetStyle();
            customStyle.VerticalAlignment = TextAlignmentType.Center;
            customCell.SetStyle(customStyle);
            
            // Salva la cartella di lavoro
            workbook.Save("DefaultStyleSettingsDemo.xlsx");
            
            // Verifica gli stili
            Console.WriteLine("A1 Vertical Alignment: " + cells["A1"].GetStyle().VerticalAlignment);
            Console.WriteLine("B1 Vertical Alignment: " + cells["B1"].GetStyle().VerticalAlignment);
        }
    }
}
```

### Vedi anche

* class [DefaultStyleSettings](../../defaultstylesettings/)
* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


