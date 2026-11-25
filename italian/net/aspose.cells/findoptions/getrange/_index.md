---
title: "FindOptions.GetRange"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo FindOptions. Ottiene e imposta l'intervallo cercato"
type: docs
url: /it/net/aspose.cells/findoptions/getrange/
---
## FindOptions.GetRange method

Ottiene e imposta l'intervallo cercato.

```csharp
public CellArea GetRange()
```

### Valore di ritorno

Restituisce l'intervallo cercato.

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class FindOptionsMethodGetRangeDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Popola alcuni dati di esempio
            worksheet.Cells["A1"].PutValue("Apple");
            worksheet.Cells["A2"].PutValue("Banana");
            worksheet.Cells["A3"].PutValue("Cherry");
            worksheet.Cells["B1"].PutValue("Orange");
            worksheet.Cells["B2"].PutValue("Grape");
            worksheet.Cells["B3"].PutValue("Lemon");

            // Crea un'istanza di FindOptions
            FindOptions findOptions = new FindOptions();
            findOptions.LookInType = LookInType.Values;
            findOptions.LookAtType = LookAtType.Contains;

            // Imposta l'intervallo di ricerca su A1:B3
            CellArea searchArea = new CellArea();
            searchArea.StartRow = 0;
            searchArea.StartColumn = 0;
            searchArea.EndRow = 2;
            searchArea.EndColumn = 1;
            findOptions.SetRange(searchArea);

            try
            {
                // Ottieni l'intervallo impostato
                CellArea resultRange = findOptions.GetRange();

                // Visualizza le informazioni sull'intervallo
                Console.WriteLine($"Search range: StartRow={resultRange.StartRow}, StartColumn={resultRange.StartColumn}, " +
                    $"EndRow={resultRange.EndRow}, EndColumn={resultRange.EndColumn}");

                // Esegui un'operazione di ricerca per dimostrare che l'intervallo è in uso
                Cell foundCell = worksheet.Cells.Find("an", null, findOptions);
                if (foundCell != null)
                {
                    Console.WriteLine($"Found value '{foundCell.StringValue}' at {foundCell.Name}");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetRange method: {ex.Message}");
            }

            // Salva la cartella di lavoro
            workbook.Save("MethodGetRangeDemo.xlsx");
        }
    }
}
```

### Vedi anche

* struct [CellArea](../../cellarea/)
* class [FindOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


