---
title: "PageSetup.PrintTitleColumns"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà PageSetup. Rappresenta le colonne che contengono le celle da ripetere sul lato sinistro di ogni pagina"
type: docs
url: /it/net/aspose.cells/pagesetup/printtitlecolumns/
---
## PageSetup.PrintTitleColumns property

Rappresenta le colonne che contengono le celle da ripetere sul lato sinistro di ogni pagina.

```csharp
public string PrintTitleColumns { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyPrintTitleColumnsDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Accedi alla configurazione della pagina
            PageSetup pageSetup = worksheet.PageSetup;
            
            // Imposta le colonne del titolo di stampa per ripetere la colonna A su ogni pagina stampata
            pageSetup.PrintTitleColumns = "$A:$A";
            
            // Aggiungi alcuni dati alla colonna A per dimostrare l'effetto
            for (int i = 0; i < 50; i++)
            {
                worksheet.Cells[$"A{i + 1}"].PutValue($"Title Column - Row {i + 1}");
            }
            
            // Salva la cartella di lavoro
            workbook.Save("PrintTitleColumnsDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


