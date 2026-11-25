---
title: "ThemeColor.Tint"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ThemeColor. Ottiene e imposta il valore della tinta"
type: docs
url: /it/net/aspose.cells/themecolor/tint/
---
## ThemeColor.Tint property

Ottiene e imposta il valore della tinta.

```csharp
public double Tint { get; set; }
```

### Osservazioni

Il valore della tinta è memorizzato come double da -1.0 a 1.0, dove -1.0 significa 100% scurimento e 1.0 significa 100% schiarimento. Inoltre, 0.0 significa nessuna modifica.

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ThemeColorPropertyTintDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crea uno stile con colore del tema e tinta
            Style style = workbook.CreateStyle();
            style.BackgroundThemeColor = new ThemeColor(ThemeColorType.Accent1, 0.5); // 0.5 tint
            
            // Applica lo stile a una cella
            Cell cell = worksheet.Cells["A1"];
            cell.SetStyle(style);

            // Ottieni il valore della tinta dallo stile della cella
            double tintValue = cell.GetStyle().BackgroundThemeColor.Tint;
            Console.WriteLine("Tint value: " + tintValue);

            // Modifica il valore della tinta
            ThemeColor themeColor = cell.GetStyle().BackgroundThemeColor;
            themeColor.Tint = 0.8; // Change tint to 0.8
            cell.SetStyle(style);

            // Verifica il nuovo valore della tinta
            Console.WriteLine("Modified tint value: " + cell.GetStyle().BackgroundThemeColor.Tint);
        }
    }
}
```

### Vedi anche

* class [ThemeColor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


