---
title: "Cell.IsInArray"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Cell. Indica se la formula della cella è una formula di matrice"
type: docs
url: /it/net/aspose.cells/cell/isinarray/
---
## Cell.IsInArray property

Indica se la formula della cella è una formula array.

```csharp
[Obsolete("Use IsArrayFormula instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool IsInArray { get; }
```

### Osservazioni

NOTA: Questa classe è ora obsoleta. Invece, si prega di utilizzare Cell.IsArrayFormula per verificare se la formula della cella è una formula di matrice. Questa proprietà sarà rimossa 12 mesi dopo, a partire da maggio 2018. Aspose si scusa per qualsiasi inconveniente tu possa aver riscontrato.

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellPropertyIsInArrayDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crea dati di esempio con formule di matrice
            worksheet.Cells["A1"].PutValue("Header1");
            worksheet.Cells["B1"].PutValue("Header2");
            worksheet.Cells["A2"].PutValue(10);
            worksheet.Cells["B2"].PutValue(20);
            worksheet.Cells["A3"].PutValue(30);
            worksheet.Cells["B3"].PutValue(40);

            // Imposta una formula di matrice usando l'API corretta
            worksheet.Cells["C2"].SetArrayFormula("A2:A3*B2:B3", 2, 1);

            // Verifica la proprietà IsInArray
            Cell cellInArray = worksheet.Cells["C2"];
            Cell cellNotInArray = worksheet.Cells["A2"];

            Console.WriteLine("Cell C2 is in array: " + cellInArray.IsInArray);
            Console.WriteLine("Cell A2 is in array: " + cellNotInArray.IsInArray);

            // Dimostra la cancellazione delle celle non di matrice
            for (int row = 1; row <= 3; row++)
            {
                for (int col = 0; col < 3; col++)
                {
                    Cell cell = worksheet.Cells[row, col];
                    if (!cell.IsInArray && !cell.IsFormula)
                    {
                        cell.PutValue("");
                    }
                }
            }

            // Salva la cartella di lavoro
            workbook.Save("IsInArrayDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


