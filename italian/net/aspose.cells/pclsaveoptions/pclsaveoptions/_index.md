---
title: "PclSaveOptions.PclSaveOptions"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Costruttore di PclSaveOptions. Crea le opzioni per salvare il file pcl"
type: docs
url: /it/net/aspose.cells/pclsaveoptions/pclsaveoptions/
---
## PclSaveOptions constructor

Crea le opzioni per salvare il file pcl.

```csharp
public PclSaveOptions()
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class PclSaveOptionsMethodCtorDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi alcuni dati di esempio al foglio di lavoro
            worksheet.Cells["A1"].PutValue("PCL Save Options Demo");
            worksheet.Cells["A2"].PutValue("This demonstrates PclSaveOptions constructor");
            
            try
            {
                // Chiama il metodo #ctor per creare un'istanza di PclSaveOptions
                PclSaveOptions pclOptions = new PclSaveOptions();
                
                // Configura opzioni aggiuntive se necessario
                pclOptions.AddPrinterFont("Arial", "ArialPCL");
                
                Console.WriteLine("PclSaveOptions created successfully");
                
                // Salva la cartella di lavoro con le opzioni PCL
                workbook.Save("PclSaveOptionsDemo.pcl", pclOptions);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error creating PclSaveOptions: {ex.Message}");
            }
        }
    }
}
```

### Vedi anche

* class [PclSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


