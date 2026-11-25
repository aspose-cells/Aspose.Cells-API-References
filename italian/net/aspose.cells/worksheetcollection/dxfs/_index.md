---
title: "WorksheetCollection.Dxfs"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "WorksheetCollection proprietà. Ottiene i record di formattazione differenziale master"
type: docs
url: /it/net/aspose.cells/worksheetcollection/dxfs/
---
## WorksheetCollection.Dxfs property

Ottiene i record di formattazione differenziale master.

```csharp
public DxfCollection Dxfs { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetCollectionPropertyDxfsDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi alcuni dati di esempio
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue(30);
            
            // Aggiungi formattazione condizionale
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcc = worksheet.ConditionalFormattings[index];
            
            // Imposta condizione e stile
            fcc.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "5", "15");
            Style style = workbook.CreateStyle();
            style.Pattern = BackgroundType.Solid;
            style.ForegroundColor = System.Drawing.Color.LightGreen;
            fcc[0].Style = style;
            
            // Dimostra la proprietà Dxfs
            Console.WriteLine("Dxfs count before applying formatting: " + workbook.Worksheets.Dxfs.Count);
            
            // Applica la formattazione che verrà aggiunta a Dxfs
            worksheet.ConditionalFormattings[0][0].Priority = 1;
            
            Console.WriteLine("Dxfs count after applying formatting: " + workbook.Worksheets.Dxfs.Count);
        }
    }
}
```

### Vedi anche

* class [DxfCollection](../../dxfcollection/)
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


