---
title: "Workbook.SetThemeColor"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Workbook. Imposta il colore del tema"
type: docs
url: /it/net/aspose.cells/workbook/setthemecolor/
---
## Workbook.SetThemeColor method

Imposta il colore del tema

```csharp
public void SetThemeColor(ThemeColorType type, Color color)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| type | ThemeColorType | Il tipo di colore del tema. |
| colore | Color | il colore del tema |

### Esempi

```csharp
using System;
using System.Drawing;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodSetThemeColorWithThemeColorTypeColorDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Imposta il colore del tema per Text1 a Verde
            workbook.SetThemeColor(ThemeColorType.Text1, Color.Green);
            
            // Applica il colore del tema allo stile predefinito
            Style style = workbook.DefaultStyle;
            style.Font.ThemeColor = new ThemeColor(ThemeColorType.Text1, 0);
            workbook.DefaultStyle = style;
            
            // Salva la cartella di lavoro
            workbook.Save("output.xlsx");
            
            Console.WriteLine("Workbook with theme color saved successfully.");
        }
    }
}
```

### Vedi anche

* enum [ThemeColorType](../../themecolortype/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


