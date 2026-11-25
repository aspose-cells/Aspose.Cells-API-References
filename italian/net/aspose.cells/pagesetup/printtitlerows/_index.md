---
title: "PageSetup.PrintTitleRows"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà PageSetup. Rappresenta le righe che contengono le celle da ripetere nella parte superiore di ogni pagina"
type: docs
url: /it/net/aspose.cells/pagesetup/printtitlerows/
---
## PageSetup.PrintTitleRows property

Rappresenta le righe che contengono le celle da ripetere nella parte superiore di ogni pagina.

```csharp
public string PrintTitleRows { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyPrintTitleRowsDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Imposta alcuni dati di esempio
            worksheet.Cells["A1"].PutValue("Header");
            for (int i = 2; i <= 10; i++)
            {
                worksheet.Cells["A" + i].PutValue("Data " + (i-1));
            }
            
            // Accedi alla configurazione della pagina
            PageSetup pageSetup = worksheet.PageSetup;
            
            // Imposta le righe di titolo di stampa (la prima riga verrà ripetuta su ogni pagina stampata)
            pageSetup.PrintTitleRows = "$1:$1";
            
            // Salva la cartella di lavoro
            workbook.Save("PrintTitleRowsDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


