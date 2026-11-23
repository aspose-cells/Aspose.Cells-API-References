---
title: "Classe GroupFill"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Aspose.Cells.Drawing.GroupFill class. Représente ce format de remplissage qui doit hériter des propriétés de remplissage du groupe"
type: docs
url: /fr/net/aspose.cells.drawing/groupfill/
---
## GroupFill class

Représente que ce format de remplissage doit hériter des propriétés de remplissage du groupe.

```csharp
public class GroupFill : Fill
```

## Méthodes

| Nom | Description |
| --- | --- |
| override [Equals](../../aspose.cells.drawing/fill/equals/)(object) | /(Hérité de [`Fill`](../fill/).) |
| override [GetHashCode](../../aspose.cells.drawing/fill/gethashcode/)() | Obtient le code de hachage.(Hérité de [`Fill`](../fill/).) |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class DrawingClassGroupFillDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur pour la démonstration
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // GroupFill n'expose pas de constructeur public sans paramètres.
                // À des fins de démonstration, nous obtenons une référence (null) du type.
                GroupFill groupFill = null;

                // Montrez que la variable de type GroupFill existe.
                Console.WriteLine($"GroupFill variable declared. Type: {typeof(GroupFill).FullName}");

                // Enregistrez le classeur (même si nous ne l'avons pas modifié, cela démontre un flux de travail complet)
                workbook.Save("GroupFillDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with GroupFill: {ex.Message}");
            }
        }
    }
}
```

### Voir aussi

* class [Fill](../fill/)
* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


