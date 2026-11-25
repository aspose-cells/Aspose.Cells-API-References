---
title: "Workbook.GetThemeColor"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Workbook. Ottiene il colore del tema"
type: docs
url: /it/net/aspose.cells/workbook/getthemecolor/
---
## Workbook.GetThemeColor method

Ottiene il colore del tema.

```csharp
public Color GetThemeColor(ThemeColorType type)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| type | ThemeColorType | Il tipo di colore del tema. |

### Valore di ritorno

Il colore del tema.

### Esempi

```csharp
using System;
using System.Drawing;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodGetThemeColorWithThemeColorTypeDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Ottieni il colore del tema per Accent6
            Color color = workbook.GetThemeColor(ThemeColorType.Accent6);
            Console.WriteLine("Theme Color (Accent6): " + color.ToString());
            
            // Salva la cartella di lavoro
            workbook.Save("output.xlsx");
        }
    }
}
```

### Vedi anche

* enum [ThemeColorType](../../themecolortype/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


