---
title: "ErrorCheckOption.GetRange"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo ErrorCheckOption. Ottiene l'intervallo influenzato da questa impostazione tramite l'indice fornito"
type: docs
url: /it/net/aspose.cells/errorcheckoption/getrange/
---
## ErrorCheckOption.GetRange method

Ottiene l'intervallo influenzato da questa impostazione per l'indice fornito.

```csharp
public CellArea GetRange(int index)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| indice | Int32 | l'indice dell'intervallo |

### Valore di ritorno

restituisce l'intervallo influenzato all'indice specificato.

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ErrorCheckOptionMethodGetRangeWithInt32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crea un ErrorCheckOption utilizzando la collezione ErrorCheckOptions del foglio di lavoro
            int errorCheckIndex = worksheet.ErrorCheckOptions.Add();
            ErrorCheckOption errorCheckOption = worksheet.ErrorCheckOptions[errorCheckIndex];

            CellArea area = new CellArea();
            area.StartRow = 1;
            area.StartColumn = 1;
            area.EndRow = 3;
            area.EndColumn = 3;
            int addedIndex = errorCheckOption.AddRange(area);

            try
            {
                int rangeCount = errorCheckOption.GetCountOfRange();
                if (rangeCount > 0)
                {
                    CellArea retrievedArea = errorCheckOption.GetRange(0);
                    Console.WriteLine($"Retrieved range: StartRow={retrievedArea.StartRow}, StartColumn={retrievedArea.StartColumn}, " +
                        $"EndRow={retrievedArea.EndRow}, EndColumn={retrievedArea.EndColumn}");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetRange method: {ex.Message}");
            }

            workbook.Save("ErrorCheckOptionMethodGetRangeWithInt32Demo.xlsx");
        }
    }
}
```

### Vedi anche

* struct [CellArea](../../cellarea/)
* class [ErrorCheckOption](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


