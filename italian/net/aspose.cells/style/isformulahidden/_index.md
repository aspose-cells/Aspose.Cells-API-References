---
title: "Style.IsFormulaHidden"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Style. Rappresenta se la formula sarà nascosta quando il foglio di lavoro è protetto"
type: docs
url: /it/net/aspose.cells/style/isformulahidden/
---
## Style.IsFormulaHidden property

Rappresenta se la formula sarà nascosta quando il foglio di lavoro è protetto.

```csharp
public bool IsFormulaHidden { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StylePropertyIsFormulaHiddenDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Crea uno stile con IsFormulaHidden impostato su true
            Style style = workbook.CreateStyle();
            style.IsFormulaHidden = true;
            
            // Applica lo stile a una cella
            cells["A1"].SetStyle(style);
            cells["A1"].Formula = "=1+1";

            // Crea un altro stile con IsFormulaHidden impostato su false
            Style style2 = workbook.CreateStyle();
            style2.IsFormulaHidden = false;
            
            // Applica il secondo stile a un'altra cella
            cells["B1"].SetStyle(style2);
            cells["B1"].Formula = "=2+2";

            // Proteggi il foglio di lavoro per vedere l'effetto
            worksheet.Protect(ProtectionType.All, "password", null);

            // Salva la cartella di lavoro
            workbook.Save("IsFormulaHiddenDemo.xlsx");

            Console.WriteLine("Workbook saved with IsFormulaHidden examples.");
        }
    }
}
```

### Vedi anche

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


