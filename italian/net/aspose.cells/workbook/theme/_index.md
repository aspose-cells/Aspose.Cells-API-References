---
title: "Workbook.Theme"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà del workbook. Ottiene il nome del tema"
type: docs
url: /it/net/aspose.cells/workbook/theme/
---
## Workbook.Theme property

Ottiene il nome del tema.

```csharp
public string Theme { get; }
```

### Esempi

```csharp
using System;
using System.Drawing;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookPropertyThemeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            
            // Dimostra il recupero del tema predefinito
            Console.WriteLine("Default theme: " + workbook.Theme);
            
            // Cambia il colore del tema e verifica
            workbook.SetThemeColor(ThemeColorType.Accent1, Color.Blue);
            Color accent1 = workbook.GetThemeColor(ThemeColorType.Accent1);
            Console.WriteLine("Modified Accent1 color: " + accent1);
            
            // Salva il workbook per dimostrare la persistenza del tema
            workbook.Save("ThemeDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


