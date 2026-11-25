---
title: "DataBar.BarBorder"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà DataBar. Ottiene un oggetto che specifica il bordo di una barra dei dati"
type: docs
url: /it/net/aspose.cells/databar/barborder/
---
## DataBar.BarBorder property

Ottiene un oggetto che specifica il bordo di una barra dati.

```csharp
public DataBarBorder BarBorder { get; }
```

### Esempi

```csharp
using System;
using System.Drawing;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DataBarPropertyBarBorderDemo
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
            int conditionIdx = fcc.AddCondition(FormatConditionType.DataBar);
            FormatCondition fc = fcc[conditionIdx];

            // Imposta le proprietà della barra dati
            fc.DataBar.MinCfvo.Type = FormatConditionValueType.AutomaticMin;
            fc.DataBar.MaxCfvo.Type = FormatConditionValueType.AutomaticMax;
            fc.DataBar.Color = Color.Blue;
            fc.DataBar.ShowValue = true;

            // Imposta le proprietà del bordo della barra
            fc.DataBar.BarBorder.Type = DataBarBorderType.Solid;
            fc.DataBar.BarBorder.Color = Color.Black;

            // Salva la cartella di lavoro
            workbook.Save("DataBarBorderDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [DataBarBorder](../../databarborder/)
* class [DataBar](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


