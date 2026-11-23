---
title: "Cell.Value"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Cell. Obtient/définit la valeur contenue dans cette cellule"
type: docs
url: /fr/net/aspose.cells/cell/value/
---
## Cell.Value property

Obtient/definit la valeur contenue dans cette cellule.

```csharp
public object Value { get; set; }
```

### Remarques

Type possible :

null,

Boolean,

DateTime,

Double,

Integer

String.

Pour une valeur int, elle peut être renvoyée sous forme d'un objet Integer ou d'un objet Double. Et il n'y a aucune garantie que la valeur renvoyée restera toujours du même type d'objet.

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellPropertyValueDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Définir les valeurs en utilisant la propriété Value
            cells[0, 0].Value = "Product ID";
            cells[0, 1].Value = "Product Name";
            
            // Démontrer les valeurs null
            cells[0, 2].Value = null;
            cells[1, 0].Value = null;
            cells[1, 1].Value = null;
            cells[1, 2].Value = null;

            // Afficher les valeurs
            Console.WriteLine("Cell[0,0] Value: " + cells[0, 0].Value);
            Console.WriteLine("Cell[0,1] Value: " + cells[0, 1].Value);
            Console.WriteLine("Cell[0,2] Value: " + (cells[0, 2].Value == null ? "null" : cells[0, 2].Value));
            Console.WriteLine("Cell[1,0] Value: " + (cells[1, 0].Value == null ? "null" : cells[1, 0].Value));
        }
    }
}
```

### Voir aussi

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


