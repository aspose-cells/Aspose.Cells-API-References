---
title: "Cells.ConvertStringToNumericValue"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Cells. Convertit toutes les données de type chaîne dans la feuille de calcul en valeur numérique si possible"
type: docs
url: /fr/net/aspose.cells/cells/convertstringtonumericvalue/
---
## Cells.ConvertStringToNumericValue method

Convertit toutes les données de type chaîne dans la feuille de calcul en valeur numérique si possible.

```csharp
public void ConvertStringToNumericValue()
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodConvertStringToNumericValueDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Cells cells = wb.Worksheets[0].Cells;
            
            // Placez les valeurs de chaîne qui peuvent être converties en valeurs numériques
            cells[0, 0].PutValue("1.23");
            cells[0, 1].PutValue("1.24");
            cells[0, 2].PutValue("1.23");
            cells[0, 3].PutValue("6/20/2021");
            cells[0, 4].PutValue("def"); // This will remain as string
            cells[0, 5].PutValue("6/20/2021");

            // Convertissez les valeurs de chaîne en valeurs numériques lorsque cela est possible
            cells.ConvertStringToNumericValue();

            // Affichez les valeurs converties
            Console.WriteLine("A1: " + cells[0, 0].DoubleValue);
            Console.WriteLine("B1: " + cells[0, 1].DoubleValue);
            Console.WriteLine("C1: " + cells[0, 2].DoubleValue);
            Console.WriteLine("D1: " + cells[0, 3].DoubleValue);
            Console.WriteLine("E1: " + cells[0, 4].StringValue); // Remains as string
            Console.WriteLine("F1: " + cells[0, 5].DoubleValue);
        }
    }
}
```

### Voir aussi

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


