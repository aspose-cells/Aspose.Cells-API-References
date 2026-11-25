---
title: "DataBar.ShowValue"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà DataBar. Ottieni o imposta il flag che indica se mostrare i valori delle celle a cui è applicata questa barra dati. Il valore predefinito è true"
type: docs
url: /it/net/aspose.cells/databar/showvalue/
---
## DataBar.ShowValue property

Ottieni o imposta il flag che indica se mostrare i valori delle celle a cui è applicata questa DataBar. Il valore predefinito è true.

```csharp
public bool ShowValue { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class DataBarPropertyShowValueDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio
            sheet.Cells["A1"].PutValue(10);
            sheet.Cells["A2"].PutValue(20);
            sheet.Cells["A3"].PutValue(30);
            sheet.Cells["A4"].PutValue(40);

            // Aggiungi formattazione condizionale della barra dati
            int idx = sheet.ConditionalFormattings.Add();
            FormatConditionCollection fcc = sheet.ConditionalFormattings[idx];
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.EndRow = 3;
            area.StartColumn = 0;
            area.EndColumn = 0;
            fcc.AddArea(area);

            // Aggiungi condizione barra dati
            int conditionIndex = fcc.AddCondition(FormatConditionType.DataBar);
            FormatCondition fc = fcc[conditionIndex];
            
            // Imposta le proprietà della barra dati
            fc.DataBar.MinCfvo.Type = FormatConditionValueType.Min;
            fc.DataBar.MaxCfvo.Type = FormatConditionValueType.Max;
            fc.DataBar.Color = Color.Green;
            
            // Dimostra la proprietà ShowValue
            fc.DataBar.ShowValue = true; // Show cell values along with data bars
            
            // Salva la cartella di lavoro
            workbook.Save("DataBarShowValueDemo.xlsx");
            
            Console.WriteLine("DataBar ShowValue demo completed. Output file: DataBarShowValueDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [DataBar](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


