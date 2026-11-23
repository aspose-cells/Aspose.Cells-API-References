---
title: "ErrorCheckOption.GetRange"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode ErrorCheckOption. Obtient la plage influencée de ce paramètre par l'index donné"
type: docs
url: /fr/net/aspose.cells/errorcheckoption/getrange/
---
## ErrorCheckOption.GetRange method

Obtient la plage influencée de ce paramètre selon l'index donné.

```csharp
public CellArea GetRange(int index)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| indice | Int32 | l'index de la plage |

### Valeur de retour

renvoie la plage influencée à l'index donné.

### Exemples

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

            // Créer un ErrorCheckOption en utilisant la collection ErrorCheckOptions de la feuille de calcul
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

### Voir aussi

* struct [CellArea](../../cellarea/)
* class [ErrorCheckOption](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


