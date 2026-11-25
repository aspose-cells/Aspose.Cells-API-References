---
title: "StyleFlag.Locked"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà StyleFlag. Verrà applicata l'impostazione Locked"
type: docs
url: /it/net/aspose.cells/styleflag/locked/
---
## StyleFlag.Locked property

L'impostazione di blocco sarà applicata.

```csharp
public bool Locked { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StyleFlagPropertyLockedDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Crea uno stile e imposta la sua proprietà locked
            Style style = workbook.CreateStyle();
            style.IsLocked = true;

            // Crea un flag di stile e abilita il flag locked
            StyleFlag styleFlag = new StyleFlag();
            styleFlag.Locked = true;

            // Applica lo stile alla cella A1
            Cell cell = cells["A1"];
            cell.SetStyle(style, styleFlag);

            // Verifica lo stato locked
            Console.WriteLine("Cell A1 is locked: " + cell.GetStyle().IsLocked);

            // Proteggi il foglio di lavoro per vedere l'effetto del locking
            worksheet.Protect(ProtectionType.All);

            // Prova a modificare la cella locked (genererà un'eccezione quando il foglio di lavoro è protetto)
            try
            {
                cell.PutValue("Test");
                Console.WriteLine("Cell modified successfully (worksheet not properly protected)");
            }
            catch
            {
                Console.WriteLine("Could not modify locked cell (worksheet protected)");
            }
        }
    }
}
```

### Vedi anche

* class [StyleFlag](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


