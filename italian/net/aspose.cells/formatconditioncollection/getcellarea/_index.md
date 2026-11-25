---
title: "FormatConditionCollection.GetCellArea"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo FormatConditionCollection. Ottiene l'intervallo di celle formattate condizionalmente per indice"
type: docs
url: /it/net/aspose.cells/formatconditioncollection/getcellarea/
---
## FormatConditionCollection.GetCellArea method

Ottiene l'intervallo di celle formattato condizionalmente per indice.

```csharp
public CellArea GetCellArea(int index)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| indice | Int32 | l'indice dell'intervallo di celle formattate condizionalmente. |

### Valore di ritorno

l'intervallo di celle formattate condizionalmente

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FormatConditionCollectionMethodGetCellAreaWithInt32Demo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio
            for (int i = 0; i < 10; i++)
            {
                for (int j = 0; j < 5; j++)
                {
                    worksheet.Cells[i, j].Value = i + j;
                }
            }

            // Aggiungi formattazione condizionale
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcc = worksheet.ConditionalFormattings[index];
            
            // Imposta l'intervallo di formattazione condizionale
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.StartColumn = 0;
            area.EndRow = 7;
            area.EndColumn = 3;
            fcc.AddArea(area);

            // Aggiungi condizione e imposta lo stile
            int conditionIndex = fcc.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "5", "10");
            Style style = workbook.CreateStyle();
            style.Pattern = BackgroundType.Solid;
            style.ForegroundColor = System.Drawing.Color.Yellow;
            fcc[conditionIndex].Style = style;

            // Ottieni e visualizza le informazioni sull'area della cella
            CellArea retrievedArea = fcc.GetCellArea(0);
            Console.WriteLine("Conditional Format Area:");
            Console.WriteLine($"StartRow: {retrievedArea.StartRow}");
            Console.WriteLine($"StartColumn: {retrievedArea.StartColumn}");
            Console.WriteLine($"EndRow: {retrievedArea.EndRow}");
            Console.WriteLine($"EndColumn: {retrievedArea.EndColumn}");

            // Salva la cartella di lavoro
            workbook.Save("output.xlsx");
        }
    }
}
```

### Vedi anche

* struct [CellArea](../../cellarea/)
* class [FormatConditionCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


