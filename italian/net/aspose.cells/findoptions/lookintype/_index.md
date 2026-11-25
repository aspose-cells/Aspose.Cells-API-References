---
title: "FindOptions.LookInType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà FindOptions. Tipo di ricerca"
type: docs
url: /it/net/aspose.cells/findoptions/lookintype/
---
## FindOptions.LookInType property

Cerca nel tipo.

```csharp
public LookInType LookInType { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FindOptionsPropertyLookInTypeDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro e aggiungi dati di esempio
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Imposta valori e formule nelle celle
            worksheet.Cells["A1"].PutValue("SearchValue");
            worksheet.Cells["A2"].Formula = "=A1";
            worksheet.Cells["B1"].PutValue("OtherValue");

            // Crea opzioni di ricerca per cercare solo nelle formule
            FindOptions options = new FindOptions
            {
                LookInType = LookInType.OnlyFormulas,
                LookAtType = LookAtType.Contains
            };

            // Cerca il valore nelle formule
            Cell foundCell = worksheet.Cells.Find("SearchValue", null, options);

            // Restituisci il risultato
            if (foundCell != null)
            {
                Console.WriteLine($"Found at: Row {foundCell.Row}, Column {foundCell.Column}");
            }
            else
            {
                Console.WriteLine("Value not found in formulas");
            }
        }
    }
}
```

### Vedi anche

* enum [LookInType](../../lookintype/)
* class [FindOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


