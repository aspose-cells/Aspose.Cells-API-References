---
title: "ConditionalFormattingCollection.Copy"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo ConditionalFormattingCollection. Copia la formattazione condizionale"
type: docs
url: /it/net/aspose.cells/conditionalformattingcollection/copy/
---
## ConditionalFormattingCollection.Copy method

Copia la formattazione condizionale.

```csharp
public void Copy(ConditionalFormattingCollection cfs)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| cfs | ConditionalFormattingCollection | La formattazione condizionale |

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ConditionalFormattingCollectionMethodCopyWithConditionalFormattingCollectioDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook destWorkbook = new Workbook();
            Worksheet destSheet = destWorkbook.Worksheets[0];

            // Crea una cartella di lavoro di origine con formattazione condizionale
            Workbook sourceWorkbook = new Workbook();
            Worksheet sourceSheet = sourceWorkbook.Worksheets[0];

            // Aggiungi una formattazione condizionale di esempio al foglio di origine
            int index = sourceSheet.ConditionalFormattings.Add();
            FormatConditionCollection fcc = sourceSheet.ConditionalFormattings[index];
            fcc.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "10", "100");
            
            // Crea e applica lo stile alla condizione di formato
            Style style = sourceWorkbook.CreateStyle();
            style.BackgroundColor = System.Drawing.Color.Red;
            FormatCondition fc = fcc[0];
            fc.Style = style;

            // Applica a un intervallo
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.EndRow = 5;
            area.StartColumn = 0;
            area.EndColumn = 5;
            fcc.AddArea(area);

            // Copia la formattazione condizionale da origine a destinazione
            destSheet.ConditionalFormattings.Copy(sourceSheet.ConditionalFormattings);

            // Salva la cartella di lavoro
            destWorkbook.Save("output.xlsx");
        }
    }
}
```

### Vedi anche

* class [ConditionalFormattingCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


