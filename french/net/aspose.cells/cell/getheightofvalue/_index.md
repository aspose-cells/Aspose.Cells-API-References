---
title: "Cell.GetHeightOfValue"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Cell. Obtient la hauteur de la valeur en unités de pixels"
type: docs
url: /fr/net/aspose.cells/cell/getheightofvalue/
---
## Cell.GetHeightOfValue method

Obtient la hauteur de la valeur en pixels.

```csharp
public int GetHeightOfValue()
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodGetHeightOfValueDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Définir la valeur et mesurer la hauteur
            worksheet.Cells["A1"].PutValue("Sample Text");
            double height = worksheet.Cells["A1"].GetHeightOfValue();
            
            Console.WriteLine("Height of value in A1: " + height);
            
            // Ajuster la hauteur de la ligne et mesurer à nouveau
            worksheet.Cells.Rows[0].Height = 30;
            height = worksheet.Cells["A1"].GetHeightOfValue();
            
            Console.WriteLine("Height after row adjustment: " + height);
        }
    }
}
```

### Voir aussi

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


