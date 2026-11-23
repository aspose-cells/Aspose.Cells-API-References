---
title: "Cell.DoubleValue"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Cell. Obtient la valeur double contenue dans la cellule"
type: docs
url: /fr/net/aspose.cells/cell/doublevalue/
---
## Cell.DoubleValue property

Obtient la valeur double contenue dans la cellule.

```csharp
public double DoubleValue { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellPropertyDoubleValueDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Définissez différents types de valeurs dans les cellules
            cells["A1"].PutValue(1); // Int value
            cells["A2"].PutValue(true); // Bool value
            cells["A3"].PutValue("abc"); // String value
            cells["A4"].PutValue(false); // Bool value
            cells["A5"].PutValue(2.56); // Double value

            // Démontrez la propriété DoubleValue
            Console.WriteLine("Double value from cell A5: " + cells["A5"].DoubleValue);
            
            // Vérifiez que d'autres types de valeurs peuvent être lus en tant que double
            Console.WriteLine("Int as double from A1: " + cells["A1"].DoubleValue);
            Console.WriteLine("Bool as double from A2: " + cells["A2"].DoubleValue);
        }
    }
}
```

### Voir aussi

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


