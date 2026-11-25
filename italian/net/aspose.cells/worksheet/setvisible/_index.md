---
title: "Worksheet.SetVisible"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Worksheet. Imposta le opzioni di visibilità"
type: docs
url: /it/net/aspose.cells/worksheet/setvisible/
---
## Worksheet.SetVisible method

Imposta le opzioni visibili.

```csharp
public void SetVisible(bool isVisible, bool ignoreError)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| isVisible | Booleano | Indica se il foglio di lavoro è visibile |
| ignoreError | Booleano | Indica se ignorare l'errore se questa opzione non è valida. |

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodSetVisibleWithBooleanBooleanDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Aggiungi alcuni fogli di lavoro
            workbook.Worksheets.Add("Sheet2");
            workbook.Worksheets.Add("Sheet3");

            // Imposta la visibilità dei fogli di lavoro
            // Primo parametro: isVisible - false per nascondere il foglio
            // Secondo parametro: ignoreError - true per ignorare l'errore se il foglio non può essere nascosto
            workbook.Worksheets["Sheet2"].SetVisible(false, true);
            workbook.Worksheets["Sheet3"].SetVisible(false, true);

            // Salva la cartella di lavoro
            workbook.Save("WorksheetVisibilityDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Vedi anche

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


