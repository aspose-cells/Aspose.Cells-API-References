---
title: "ProtectedRange.AddArea"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo ProtectedRange. Aggiunge un'area di riferimento a questo"
type: docs
url: /it/net/aspose.cells/protectedrange/addarea/
---
## ProtectedRange.AddArea method

Aggiunge un'area di riferimento a questo

```csharp
public void AddArea(int startRow, int startColumn, int endRow, int endColumn)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| startRow | Int32 | La riga iniziale. |
| startColumn | Int32 | La colonna iniziale. |
| endRow | Int32 | La riga finale. |
| endColumn | Int32 | La colonna finale. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ProtectedRangeMethodAddAreaWithInt32Int32Int32Int32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add restituisce l'indice del nuovo ProtectedRange nella collezione
            int protectedRangeIndex = worksheet.AllowEditRanges.Add("DemoProtectedRange", 0, 0, 0, 0);
            ProtectedRange protectedRange = worksheet.AllowEditRanges[protectedRangeIndex];

            try
            {
                protectedRange.AddArea(2, 2, 5, 5);
                Console.WriteLine("Added new area to protected range.");

                CellArea[] areas = protectedRange.GetAreas();
                Console.WriteLine($"Total protected areas: {areas.Length}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }

            worksheet.Protect(ProtectionType.All, "password123", null);
            workbook.Save("ProtectedRangeAddAreaDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [ProtectedRange](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


