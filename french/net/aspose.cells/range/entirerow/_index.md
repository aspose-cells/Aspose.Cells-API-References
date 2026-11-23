---
title: "Range.EntireRow"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Range. Obtient un objet Range qui représente la ou les lignes entières contenant la plage spécifiée"
type: docs
url: /fr/net/aspose.cells/range/entirerow/
---
## Range.EntireRow property

Obtient un objet Range qui représente la ligne entière (ou les lignes) contenant la plage spécifiée.

```csharp
public Range EntireRow { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangePropertyEntireRowDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Remplissez quelques données d'exemple dans la première ligne
            for (int col = 0; col < 5; col++)
            {
                sheet.Cells[0, col].PutValue($"Header {col + 1}");
            }

            // Obtenez la première ligne entière en utilisant la propriété EntireRow
            Aspose.Cells.Range entireRow = sheet.Cells.CreateRange("A1").EntireRow;

            // Copiez la première ligne vers la troisième ligne
            Aspose.Cells.Range destination = sheet.Cells.CreateRange("A3").EntireRow;
            destination.Copy(entireRow);

            // Enregistrez le classeur
            workbook.Save("EntireRowDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


