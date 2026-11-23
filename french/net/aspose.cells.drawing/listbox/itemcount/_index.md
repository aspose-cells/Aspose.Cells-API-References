---
title: "ListBox.ItemCount"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ListBox. Obtient le nombre d'éléments dans la listbox"
type: docs
url: /fr/net/aspose.cells.drawing/listbox/itemcount/
---
## ListBox.ItemCount property

Obtient le nombre d'éléments dans la zone de liste.

```csharp
public int ItemCount { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ListBoxPropertyItemCountDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets.Add("Sheet1");

            // Ajoutez des données d'exemple
            worksheet.Cells["A1"].PutValue("Apple");
            worksheet.Cells["A2"].PutValue("Banana");
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["A4"].PutValue("Mango");

            // Créer une listbox et définir les propriétés
            Aspose.Cells.Drawing.ListBox listBox = worksheet.Shapes.AddListBox(1, 0, 10, 0, 100, 150);
            listBox.InputRange = "A1:A4";
            
            // Démontrer l'utilisation de ItemCount
            int itemCount = listBox.ItemCount;
            Console.WriteLine("ListBox contains {0} items", itemCount);
            
            // Ajuster la hauteur de la listbox en fonction du nombre d'éléments
            listBox.Height = itemCount * 15;

            workbook.Save("ListBoxItemCountDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [ListBox](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


