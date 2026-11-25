---
title: "PageSetup.Orientation"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà PageSetup. Rappresenta l'orientamento di stampa della pagina"
type: docs
url: /it/net/aspose.cells/pagesetup/orientation/
---
## PageSetup.Orientation property

Rappresenta l'orientamento di stampa della pagina.

```csharp
public PageOrientationType Orientation { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyOrientationDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Imposta l'orientamento della pagina su Landscape
            worksheet.PageSetup.Orientation = PageOrientationType.Landscape;
            
            // Aggiungi alcuni dati di esempio per dimostrare l'effetto
            worksheet.Cells["A1"].PutValue("Landscape Orientation Demo");
            for (int i = 1; i <= 10; i++)
            {
                worksheet.Cells[$"A{i}"].PutValue($"Data Row {i}");
            }
            
            // Salva la cartella di lavoro
            workbook.Save("PageOrientationDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Vedi anche

* enum [PageOrientationType](../../pageorientationtype/)
* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


