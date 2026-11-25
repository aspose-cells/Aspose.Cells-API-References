---
title: "Row.CopySettings"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Row. Copia le impostazioni della riga come stile, altezza, visibilità ...ecc"
type: docs
url: /it/net/aspose.cells/row/copysettings/
---
## Row.CopySettings method

Copia le impostazioni della riga, come stile, altezza, visibilità, ...ecc.

```csharp
public void CopySettings(Row source, bool checkStyle)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| origine | Row | la riga di origine le cui impostazioni saranno copiate in questa |
| checkStyle | Booleano | se controllare e raccogliere lo stile. Ha effetto e risulta necessario solo quando due oggetti riga appartengono a cartelle di lavoro diverse e gli stili delle due cartelle di lavoro sono differenti. |

### Esempi

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class RowMethodCopySettingsWithRowBooleanDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crea e stila la riga di origine
            Row sourceRow = worksheet.Cells.Rows[0];
            Style sourceStyle = workbook.CreateStyle();
            sourceStyle.BackgroundColor = Color.Blue;
            sourceRow.ApplyStyle(sourceStyle, new StyleFlag { All = true });
            sourceRow.Height = 25;
            sourceRow.IsHidden = false;

            // Crea la riga di destinazione
            Row targetRow = worksheet.Cells.Rows[1];
            
            // Dimostra CopySettings con copyStyle=true
            targetRow.CopySettings(sourceRow, true);

            // Verifica che le impostazioni siano state copiate
            Console.WriteLine($"Target row height: {targetRow.Height}");
            Console.WriteLine($"Target row is hidden: {targetRow.IsHidden}");

            workbook.Save("RowCopySettingsDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Row](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


