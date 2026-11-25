---
title: "LoadOptions.StandardFont"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà LoadOptions. Imposta il nome del carattere standard predefinito"
type: docs
url: /it/net/aspose.cells/loadoptions/standardfont/
---
## LoadOptions.StandardFont property

Imposta il nome del carattere standard predefinito

```csharp
[Obsolete("Use DefaultStyleSettings.FontName property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public string StandardFont { get; set; }
```

### Osservazioni

NOTA: Questo membro è ora obsoleto. Invece, si prega di utilizzare DefaultStyleSettings. Questa proprietà sarà rimossa tra 12 mesi a partire da marzo 2022. Aspose si scusa per eventuali disagi che potresti aver riscontrato.

### Esempi

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class LoadOptionsPropertyStandardFontDemo
    {
        public static void Run()
        {
            // Crea un file Excel di esempio in memoria
            MemoryStream ms = new MemoryStream();
            using (Workbook workbook = new Workbook())
            {
                workbook.Worksheets[0].Cells["A1"].PutValue("Standard Font Test");
                workbook.Save(ms, SaveFormat.Xlsx);
            }
            ms.Position = 0;

            // Imposta le opzioni di caricamento con StandardFont
            LoadOptions loadOptions = new LoadOptions();
            loadOptions.StandardFont = "SimSun";
            
            // Carica la cartella di lavoro con il carattere specificato
            Workbook workbookWithFont = new Workbook(ms, loadOptions);
            
            // Dimostra che il carattere è impostato controllando lo stile predefinito
            Console.WriteLine("Default font after loading: " + 
                workbookWithFont.DefaultStyle.Font.Name);
        }
    }
}
```

### Vedi anche

* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


