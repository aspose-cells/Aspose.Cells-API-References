---
title: "AutoFilter.ShowAll"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo AutoFilter. Mostra tutte le righe nascoste"
type: docs
url: /it/net/aspose.cells/autofilter/showall/
---
## AutoFilter.ShowAll method

Mostra tutte le righe.

```csharp
public void ShowAll()
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class AutoFilterMethodShowAllDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro con dati di esempio
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio
            worksheet.Cells["A1"].PutValue("Fruit");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Banana");
            worksheet.Cells["A4"].PutValue("Orange");
            worksheet.Cells["A5"].PutValue("Grape");
            
            // Applica filtro automatico
            worksheet.AutoFilter.Range = "A1:A5";
            
            // Filtra per mostrare solo "Apple"
            worksheet.AutoFilter.Filter(0, "Apple");
            
            // Mostra nuovamente tutti i dati
            worksheet.AutoFilter.ShowAll();
            
            // Salva la cartella di lavoro
            workbook.Save("ShowAllDemoOutput.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Vedi anche

* class [AutoFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


