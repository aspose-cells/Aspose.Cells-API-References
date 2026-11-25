---
title: "Workbook.Combine"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Workbook. Combina un altro oggetto Workbook"
type: docs
url: /it/net/aspose.cells/workbook/combine/
---
## Workbook.Combine method

Combina un altro oggetto Workbook.

```csharp
public void Combine(Workbook secondWorkbook)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| secondWorkbook | Cartella di lavoro | Un altro oggetto Workbook. |

### Osservazioni

Unisci Excel, ODS, CSV e altri file in un unico file.

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodCombineWithWorkbookDemo
    {
        public static void Run()
        {
            // Crea il workbook di origine
            Workbook sourceWorkbook = new Workbook();
            sourceWorkbook.Worksheets[0].Cells["A1"].PutValue("Source Data");

            // Crea la cartella di lavoro di destinazione
            Workbook destWorkbook = new Workbook(FileFormatType.Xlsx);
            destWorkbook.Worksheets[0].Cells["B2"].PutValue("Destination Data");

            // Combina i workbook
            destWorkbook.Combine(sourceWorkbook);

            // Salva il workbook combinato
            destWorkbook.Save("CombinedWorkbook.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Vedi anche

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


