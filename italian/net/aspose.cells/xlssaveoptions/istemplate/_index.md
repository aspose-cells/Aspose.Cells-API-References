---
title: "XlsSaveOptions.IsTemplate"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà XlsSaveOptions. Indica se salvare un file modello"
type: docs
url: /it/net/aspose.cells/xlssaveoptions/istemplate/
---
## XlsSaveOptions.IsTemplate property

Indica se salvare un file modello.

```csharp
[Obsolete("Use XlsSaveOptions(SaveFormat.Xlt) when it is template, otherwise use XlsSaveOptions().")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool IsTemplate { get; set; }
```

### Osservazioni

NOTA: Questo membro è ora obsoleto. Invece, crea XlsSaveOptions con il formato di salvataggio corrispondente (xlt per true e xls per false). Questo metodo sarà rimosso 12 mesi dopo, a partire da agosto 2020. Aspose si scusa per qualsiasi inconveniente tu possa aver riscontrato.

### Esempi

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class XlsSaveOptionsPropertyIsTemplateDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Aggiungi dati di esempio al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Sample Template");
            
            // Salva come file modello
            string outputPath = "output_template.xlt";
            XlsSaveOptions saveOptions = new XlsSaveOptions();
            saveOptions.IsTemplate = true;
            
            using (FileStream fs = File.Create(outputPath))
            {
                workbook.Save(fs, saveOptions);
            }
            
            // Verifica il formato del file salvato
            Workbook loadedWorkbook = new Workbook(outputPath);
            Console.WriteLine("File format: " + loadedWorkbook.FileFormat);
        }
    }
}
```

### Vedi anche

* class [XlsSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


