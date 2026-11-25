---
title: "DefaultStyleSettings.VerticalAlignment"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà DefaultStyleSettings. Ottiene/Imposta il valore predefinito per l'allineamento verticale"
type: docs
url: /it/net/aspose.cells/defaultstylesettings/verticalalignment/
---
## DefaultStyleSettings.VerticalAlignment property

Ottiene/Imposta il valore predefinito per l'allineamento verticale

```csharp
public TextAlignmentType VerticalAlignment { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DefaultStyleSettingsPropertyVerticalAlignmentDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Imposta l'allineamento verticale predefinito su Bottom
            LoadOptions options = new LoadOptions();
            options.DefaultStyleSettings.VerticalAlignment = TextAlignmentType.Bottom;

            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Imposta alcuni dati di esempio
            worksheet.Cells["A1"].PutValue("Sample Text 1");
            worksheet.Cells["B1"].PutValue("Sample Text 2");
            worksheet.Cells["C1"].PutValue("Sample Text 3");

            // Verifica che l'allineamento verticale sia applicato a tutte le celle
            foreach (Cell cell in worksheet.Cells)
            {
                Console.WriteLine($"Cell {cell.Name} Vertical Alignment: {cell.GetStyle().VerticalAlignment}");
            }

            // Salva la cartella di lavoro
            workbook.Save("VerticalAlignmentDemo.xlsx");
        }
    }
}
```

### Vedi anche

* enum [TextAlignmentType](../../textalignmenttype/)
* class [DefaultStyleSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


