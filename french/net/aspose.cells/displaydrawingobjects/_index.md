---
title: "Enum DisplayDrawingObjects"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Aspose.Cells.DisplayDrawingObjects enum. Représente si et comment afficher les objets dans le classeur"
type: docs
url: /fr/net/aspose.cells/displaydrawingobjects/
---
## DisplayDrawingObjects enumeration

Représente si et comment afficher les objets dans le classeur.

```csharp
public enum DisplayDrawingObjects
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| DisplayShapes | `0` | Afficher tous les objets |
| Placeholders | `1` | Afficher les espaces réservés |
| Hide | `2` | Masquer toutes les formes. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class DisplayDrawingObjectsDemo
    {
        public static void DisplayDrawingObjectsExample()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();

            // Accéder aux paramètres du classeur
            WorkbookSettings settings = workbook.Settings;

            // Définir la propriété DisplayDrawingObjects pour afficher tous les objets
            settings.DisplayDrawingObjects = DisplayDrawingObjects.DisplayShapes;

            // Enregistrez le classeur
            workbook.Save("DisplayDrawingObjectsExample_DisplayShapes.xlsx");

            // Définir la propriété DisplayDrawingObjects pour afficher les espaces réservés
            settings.DisplayDrawingObjects = DisplayDrawingObjects.Placeholders;

            // Enregistrez le classeur
            workbook.Save("DisplayDrawingObjectsExample_Placeholders.xlsx");

            // Définir la propriété DisplayDrawingObjects pour masquer toutes les formes
            settings.DisplayDrawingObjects = DisplayDrawingObjects.Hide;

            // Enregistrez le classeur
            workbook.Save("DisplayDrawingObjectsExample_Hide.xlsx");
            workbook.Save("DisplayDrawingObjectsExample_Hide.pdf");
            return;
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


