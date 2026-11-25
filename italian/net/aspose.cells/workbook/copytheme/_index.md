---
title: "Workbook.CopyTheme"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Workbook. Copia il tema da un'altra cartella di lavoro"
type: docs
url: /it/net/aspose.cells/workbook/copytheme/
---
## Workbook.CopyTheme method

Copia il tema da un'altra cartella di lavoro.

```csharp
public void CopyTheme(Workbook source)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| origine | Cartella di lavoro | Cartella di lavoro di origine. |

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodCopyThemeWithWorkbookDemo
    {
        public static void Run()
        {
            // Crea la cartella di lavoro di origine (il tema viene impostato automaticamente all'apertura di un file modello)
            Workbook sourceWorkbook = new Workbook(FileFormatType.Xlsx);

            // Crea la cartella di lavoro di destinazione
            Workbook destWorkbook = new Workbook();
            
            // Copia il tema dalla cartella di lavoro di origine a quella di destinazione
            destWorkbook.CopyTheme(sourceWorkbook);

            // Salva il workbook di destinazione
            destWorkbook.Save("output_with_theme.xlsx");
        }
    }
}
```

### Vedi anche

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


