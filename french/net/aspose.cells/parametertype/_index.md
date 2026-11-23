---
title: "Énumération ParameterType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Aspose.Cells.ParameterType enum. Représente tous les types de paramètres ou le type de valeur de retour d'une fonction"
type: docs
url: /fr/net/aspose.cells/parametertype/
---
## ParameterType enumeration

Représente le type de tous les paramètres ou le type de valeur de retour d'une fonction.

```csharp
public enum ParameterType
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| Reference | `0` |  |
| Value | `1` |  |
| Array | `2` |  |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ParameterTypeDemo
    {
        public static void ParameterTypeExample()
        {
            // Création d'un classeur et d'une feuille de calcul pour démontrer l'utilisation
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Exemple d'utilisation de l'énumération ParameterType dans une fonction de formule
            // Supposons que nous définissions une fonction personnalisée avec des types de paramètres spécifiques

            // Définir un tableau de types de paramètres
            ParameterType[] parameterTypes = new ParameterType[]
            {
                ParameterType.Reference,
                ParameterType.Value,
                ParameterType.Array
            };

            // Fonction d'exemple qui utilise ces types de paramètres
            // Par exemple, définir une fonction personnalisée hypothétique avec des types de paramètres définis
            // (Remarque : la gestion des fonctions personnalisées dépendrait des capacités de l'API Aspose.Cells)

            // Enregistrer le classeur pour démontrer les modifications
            workbook.Save("ParameterTypeExample.xlsx");
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


