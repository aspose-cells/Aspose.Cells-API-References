---
title: "Range.Address"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Range. Obtient l'adresse de la plage"
type: docs
url: /fr/net/aspose.cells/range/address/
---
## Range.Address property

Obtient l'adresse de la plage.

```csharp
public string Address { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangePropertyAddressDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Créez une plage et démontrez la propriété Address
            Aspose.Cells.Range range = cells.CreateRange("A1");
            Console.WriteLine("Original range address: " + range.Address);

            // Démontrez GetOffset avec Address
            Aspose.Cells.Range offsetRange = range.GetOffset(1, 1);
            Console.WriteLine("Offset range address: " + offsetRange.Address);

            // Démontrez EntireRow Address
            Aspose.Cells.Range entireRow = range.EntireRow;
            Console.WriteLine("Entire row address: " + entireRow.Address);

            // Démontrez EntireColumn Address
            Aspose.Cells.Range entireColumn = range.EntireColumn;
            Console.WriteLine("Entire column address: " + entireColumn.Address);
        }
    }
}
```

### Voir aussi

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


