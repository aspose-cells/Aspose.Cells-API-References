---
title: "ThemeColor.ThemeColor"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Costruttore ThemeColor."
type: docs
url: /it/net/aspose.cells/themecolor/themecolor/
---
## ThemeColor constructor

```csharp
public ThemeColor(ThemeColorType type, double tint)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| type | ThemeColorType | Il tipo di tema. |
| tinta | Double | Il valore della tinta. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ThemeColorMethodCtorWithThemeColorTypeDoubleDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Chiama il metodo #ctor con i parametri ThemeColorType e Double
                ThemeColor themeColor = new ThemeColor(ThemeColorType.Accent1, 0.5);

                // Applica il colore del tema allo stile di una cella
                Style style = workbook.CreateStyle();
                style.ForegroundThemeColor = themeColor;
                style.Pattern = BackgroundType.Solid;
                
                Cell cell = worksheet.Cells["A1"];
                cell.PutValue("ThemeColor with Accent1 and 0.5 tint");
                cell.SetStyle(style);

                Console.WriteLine("ThemeColor constructor executed successfully with parameters (ThemeColorType.Accent1, 0.5)");
                Console.WriteLine($"ColorType: {themeColor.ColorType}, Tint: {themeColor.Tint}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing ThemeColor constructor: {ex.Message}");
            }
            
            // Salva il risultato
            workbook.Save("ThemeColorCtorDemo.xlsx");
        }
    }
}
```

### Vedi anche

* enum [ThemeColorType](../../themecolortype/)
* class [ThemeColor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


