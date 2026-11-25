---
title: "LoadOptions.LoadFilter"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà LoadOptions. Il filtro che indica come caricare i dati"
type: docs
url: /it/net/aspose.cells/loadoptions/loadfilter/
---
## LoadOptions.LoadFilter property

Il filtro per indicare come caricare i dati.

```csharp
public LoadFilter LoadFilter { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CustomLoadFilter : LoadFilter
    {
        public override void StartSheet(Worksheet sheet)
        {
            // Carica i dati solo se il foglio è visibile
            if (sheet.IsVisible)
            {
                base.StartSheet(sheet);
            }
        }
    }

    public class LoadOptionsPropertyLoadFilterDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro di prova
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            sheet.Name = "HiddenSheet";
            sheet.IsVisible = false;
            sheet.Cells["A1"].PutValue("This should not load");
            
            // Aggiungi un foglio visibile
            Worksheet visibleSheet = workbook.Worksheets.Add("VisibleSheet");
            visibleSheet.Cells["A1"].PutValue("This will load");
            
            // Salva il file di prova
            string filePath = "LoadFilterTest.xlsx";
            workbook.Save(filePath);
            workbook.Dispose();

            // Carica con filtro personalizzato
            LoadOptions options = new LoadOptions();
            options.LoadFilter = new CustomLoadFilter();
            
            Workbook loadedWorkbook = new Workbook(filePath, options);
            
            // Verifica che solo il foglio visibile sia caricato
            Console.WriteLine("Loaded Sheets:");
            foreach (Worksheet ws in loadedWorkbook.Worksheets)
            {
                Console.WriteLine($"- {ws.Name}: Visible={ws.IsVisible}");
                if (ws.IsVisible)
                {
                    Console.WriteLine($"  A1 Value: {ws.Cells["A1"].StringValue}");
                }
            }
            
            loadedWorkbook.Dispose();
        }
    }
}
```

### Vedi anche

* class [LoadFilter](../../loadfilter/)
* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


