---
title: "Style.IsLocked"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Style. Ottiene o imposta un valore che indica se una cella può essere modificata o meno"
type: docs
url: /it/net/aspose.cells/style/islocked/
---
## Style.IsLocked property

Ottiene o imposta un valore che indica se una cella può essere modificata o meno.

```csharp
public bool IsLocked { get; set; }
```

### Osservazioni

Bloccare le celle non ha effetto a meno che il foglio di lavoro non sia protetto.

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StylePropertyIsLockedDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Imposta la proprietà IsLocked per una cella
            Cell cell = cells["A1"];
            Style style = cell.GetStyle();
            style.IsLocked = true;
            cell.SetStyle(style);

            // Proteggi il foglio di lavoro per applicare il blocco
            worksheet.Protect(ProtectionType.All);

            // Verifica e stampa lo stato di IsLocked
            Console.WriteLine("Cell A1 IsLocked: " + cells["A1"].GetStyle().IsLocked);
            Console.WriteLine("Cell B1 IsLocked: " + cells["B1"].GetStyle().IsLocked);

            // Salva la cartella di lavoro
            workbook.Save("IsLockedDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


