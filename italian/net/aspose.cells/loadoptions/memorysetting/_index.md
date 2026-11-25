---
title: "LoadOptions.MemorySetting"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà LoadOptions. Ottiene o imposta la modalità di memoria per la cartella di lavoro caricata"
type: docs
url: /it/net/aspose.cells/loadoptions/memorysetting/
---
## LoadOptions.MemorySetting property

Ottiene o imposta la modalità di memoria per il workbook caricato.

```csharp
public MemorySetting MemorySetting { get; set; }
```

### Osservazioni

Per ulteriori dettagli sulla modalità di memoria, consulta [`MemorySetting`](../../cells/memorysetting/).

### Esempi

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class LoadOptionsPropertyMemorySettingDemo
    {
        public static void Run()
        {
            // Crea opzioni di caricamento con impostazione della preferenza di memoria
            LoadOptions loadOptions = new LoadOptions(LoadFormat.Auto);
            loadOptions.MemorySetting = MemorySetting.MemoryPreference;

            // Carica la cartella di lavoro con impostazioni ottimizzate per la memoria
            Workbook workbook = new Workbook(new MemoryStream(), loadOptions);
            
            // Accedi al foglio di lavoro e aggiungi alcuni dati di esempio
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Memory Setting Demo");
            worksheet.Cells["A2"].PutValue(DateTime.Now.ToString());
            
            // Salva la cartella di lavoro
            workbook.Save("MemorySettingDemo.xlsx", SaveFormat.Xlsx);
            
            Console.WriteLine("Workbook saved with MemoryPreference setting.");
        }
    }
}
```

### Vedi anche

* enum [MemorySetting](../../memorysetting/)
* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


