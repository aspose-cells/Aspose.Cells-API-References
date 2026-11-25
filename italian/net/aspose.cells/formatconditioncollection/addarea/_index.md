---
title: "FormatConditionCollection.AddArea"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo FormatConditionCollection. Aggiunge un intervallo di celle formattate condizionalmente"
type: docs
url: /it/net/aspose.cells/formatconditioncollection/addarea/
---
## FormatConditionCollection.AddArea method

Aggiunge un intervallo di celle formattato condizionalmente.

```csharp
public int AddArea(CellArea cellArea)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| cellArea | CellArea | Intervallo di celle formattato condizionalmente. |

### Valore di ritorno

Indice dell'intervallo di celle formattate condizionalmente.

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FormatConditionCollectionMethodAddAreaWithCellAreaDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio
            for (int row = 0; row < 10; row++)
            {
                for (int col = 0; col < 10; col++)
                {
                    worksheet.Cells[row, col].PutValue(row * col);
                }
            }

            // Aggiungi formattazione condizionale
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection formatCollection = worksheet.ConditionalFormattings[index];
            
            // Crea una condizione di formattazione
            formatCollection.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "10", "100");
            
            // Crea aree di celle e aggiungile alla collezione di formattazione
            CellArea area1 = CellArea.CreateCellArea(0, 0, 4, 4);
            CellArea area2 = CellArea.CreateCellArea(5, 5, 9, 9);
            
            formatCollection.AddArea(area1);
            formatCollection.AddArea(area2);

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


