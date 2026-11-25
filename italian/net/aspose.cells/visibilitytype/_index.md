---
title: "Enum VisibilityType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Aspose.Cells.VisibilityType enum. Rappresenta gli stati per la visibilità del foglio"
type: docs
url: /it/net/aspose.cells/visibilitytype/
---
## VisibilityType enumeration

Rappresenta gli stati per la visibilità del foglio.

```csharp
public enum VisibilityType
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| Visible | `0` | Indica che il foglio è visibile. |
| Hidden | `1` | Indica che il foglio è nascosto, ma può essere mostrato dall'utente tramite l'interfaccia utente. |
| VeryHidden | `2` | Indica che il foglio è nascosto e non può essere mostrato nell'interfaccia utente (UI). Questo stato è disponibile solo programmaticamente. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class VisibilityTypeDemo
    {
        public static void VisibilityTypeExample()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            workbook.Worksheets.Add("NewSheet");
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Imposta il nome del foglio di lavoro
            worksheet.Name = "DemoSheet";

            // Imposta la visibilità del foglio di lavoro su Nascosto
            worksheet.VisibilityType = VisibilityType.Hidden;

            // Salva la cartella di lavoro
            workbook.Save("VisibilityTypeExample.xlsx");

            // Output per indicare che il processo è completato
            Console.WriteLine("Workbook saved with the worksheet visibility set to Hidden.");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


