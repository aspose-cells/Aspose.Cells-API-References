---
title: "Enum SheetType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Enum Aspose.Cells.SheetType. Specifica il tipo di foglio di lavoro"
type: docs
url: /it/net/aspose.cells/sheettype/
---
## SheetType enumeration

Specifica il tipo di foglio di lavoro.

```csharp
public enum SheetType
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| VB | `0` | Modulo Visual Basic |
| Worksheet | `1` |  |
| Chart | `2` | Grafico |
| BIFF4Macro | `3` | Foglio macro BIFF4 |
| InternationalMacro | `4` | Foglio macro internazionale |
| Other | `5` |  |
| Dialog | `6` | Foglio di lavoro della finestra di dialogo |

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassSheetTypeDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Inserisci un nuovo foglio di lavoro di tipo Worksheet all'indice 0
            Worksheet newWorksheet = workbook.Worksheets.Insert(0, SheetType.Worksheet);
            
            // Imposta il nome del nuovo foglio di lavoro
            newWorksheet.Name = "InsertedSheet";
            
            // Accedi alle celle nel nuovo foglio di lavoro e aggiungi alcuni dati
            newWorksheet.Cells["A1"].PutValue("This is a new worksheet");
            
            // Salva la cartella di lavoro
            workbook.Save("SheetTypeDemoOutput.xlsx");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


