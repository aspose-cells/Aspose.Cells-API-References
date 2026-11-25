---
title: "SaveOptions.MergeAreas"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà SaveOptions. Indica se unire le aree di formattazione condizionale e convalida prima di salvare il file"
type: docs
url: /it/net/aspose.cells/saveoptions/mergeareas/
---
## SaveOptions.MergeAreas property

Indica se unire le aree di formattazione condizionale e convalida prima di salvare il file.

```csharp
public bool MergeAreas { get; set; }
```

### Osservazioni

Il valore predefinito è false.

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class SaveOptionsPropertyMergeAreasDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Inserisci dati e crea celle unite
            worksheet.Cells["A1"].PutValue("Merged Header");
            worksheet.Cells["A2"].PutValue("Data 1");
            worksheet.Cells["A3"].PutValue("Data 2");
            
            // Unisci le celle A1:B1
            worksheet.Cells.Merge(0, 0, 1, 2);

            // Crea le opzioni di salvataggio con MergeAreas abilitato
            XlsSaveOptions saveOptions = new XlsSaveOptions();
            saveOptions.MergeAreas = true;

            // Salva con ottimizzazione delle aree unite
            workbook.Save("MergeAreasDemo.xlsx", saveOptions);
        }
    }
}
```

### Vedi anche

* class [SaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


