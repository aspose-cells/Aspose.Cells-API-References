---
title: "ValidationCollection.Add"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode ValidationCollection. Ajoute une validation de données à la collection"
type: docs
url: /fr/net/aspose.cells/validationcollection/add/
---
## Add() {#add}

Ajoute une validation de données à la collection.

```csharp
[Obsolete("Use ValidationCollection.Add(CellArea) method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int Add()
```

### Valeur de retour

[`Validation`](../../validation/) object index.

### Remarques

NOTE : Cette méthode est maintenant obsolète. À la place, veuillez utiliser la méthode ValidationCollection.Add(CellArea). Cette méthode sera supprimée 12 mois plus tard depuis JANVIER 2015. Aspose s'excuse pour tout désagrément que vous avez pu rencontrer.

### Voir aussi

* class [ValidationCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Add(CellArea) {#add_1}

Ajoute une validation de données à la collection.

```csharp
public int Add(CellArea ca)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| ca | CellArea | La zone contient cette validation. |

### Valeur de retour

[`Validation`](../../validation/) object index.

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ValidationCollectionMethodAddWithCellAreaDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Créer une zone de cellules pour la validation
            CellArea cellarea = new CellArea();
            cellarea.StartRow = 0;
            cellarea.StartColumn = 0;
            cellarea.EndRow = 1;
            cellarea.EndColumn = 1;
            
            // Ajouter la validation à la collection
            int index = sheet.Validations.Add(cellarea);
            Validation validation = sheet.Validations[index];
            
            // Configurer les paramètres de validation
            validation.Type = ValidationType.List;
            validation.Formula1 = "Yes,No";
            validation.AlertStyle = ValidationAlertType.Information;
            
            // Enregistrez le classeur
            workbook.Save("ValidationCollectionMethodAddWithCellAreaDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Voir aussi

* struct [CellArea](../../cellarea/)
* class [ValidationCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


