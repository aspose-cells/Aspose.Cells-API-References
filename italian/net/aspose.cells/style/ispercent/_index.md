---
title: "Style.IsPercent"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Style. Indica se il formato numerico è un formato percentuale"
type: docs
url: /it/net/aspose.cells/style/ispercent/
---
## Style.IsPercent property

Indica se il formato numerico è un formato percentuale.

```csharp
public bool IsPercent { get; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class StylePropertyIsPercentDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Accedi alla cella A1 e imposta il suo valore
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue(0.5);
            
            // Ottieni lo stile della cella
            Style style = cell.GetStyle();
            
            // Visualizza il valore corrente di IsPercent
            Console.WriteLine("Current IsPercent value: " + style.IsPercent);
            
            // Imposta il formato numerico su percentuale (questo imposterà automaticamente IsPercent su true)
            style.Number = 10; // 10 is the built-in percentage format in Excel
            
            // Applica lo stile alla cella
            cell.SetStyle(style);
            
            // Verifica che IsPercent sia ora vero
            Console.WriteLine("After setting percentage format, IsPercent value: " + style.IsPercent);
            
            // Crea un'altra cella con formato diverso
            Cell cell2 = worksheet.Cells["A2"];
            cell2.PutValue(0.75);
            Style style2 = cell2.GetStyle();
            style2.Number = 3; // 3 is the built-in number format (not percentage)
            cell2.SetStyle(style2);
            
            // Verifica che IsPercent sia falso per un formato non percentuale
            Console.WriteLine("For non-percentage format, IsPercent value: " + style2.IsPercent);
            
            // Salva la cartella di lavoro
            workbook.Save("StylePropertyIsPercentDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


