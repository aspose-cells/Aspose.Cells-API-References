---
title: "Classe ProtectedRange"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.ProtectedRange. Une plage spécifiée autorisée à être modifiée lorsque la protection de la feuille est ACTIVÉE"
type: docs
url: /fr/net/aspose.cells/protectedrange/
---
## ProtectedRange class

Une plage spécifiée autorisée à être modifiée lorsque la protection de la feuille est ACTIVÉE.

```csharp
public class ProtectedRange
```

## Propriétés

| Nom | Description |
| --- | --- |
| [CellArea](../../aspose.cells/protectedrange/cellarea/) { get; } | Obtient l'objet [`CellArea`](./cellarea/) qui représente la zone de cellules à protéger. |
| [IsProtectedWithPassword](../../aspose.cells/protectedrange/isprotectedwithpassword/) { get; } | Indique si la feuille de calcul est protégée par un mot de passe. |
| [Name](../../aspose.cells/protectedrange/name/) { get; set; } | Obtient le titre de la plage. Il est utilisé comme un descripteur, pas comme une définition de plage nommée. |
| [Password](../../aspose.cells/protectedrange/password/) { get; set; } | Représente le mot de passe pour protéger la plage. |
| [SecurityDescriptor](../../aspose.cells/protectedrange/securitydescriptor/) { get; set; } | Le descripteur de sécurité définit les comptes d'utilisateur qui peuvent modifier cette plage sans fournir de mot de passe pour y accéder. |

## Méthodes

| Nom | Description |
| --- | --- |
| [AddArea](../../aspose.cells/protectedrange/addarea/)(int, int, int, int) | Ajoute une zone référencée à celle-ci |
| [GetAreas](../../aspose.cells/protectedrange/getareas/)() | Obtient toutes les zones référencées. |

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassProtectedRangeDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Obtenir la collection de plages protégées
            ProtectedRangeCollection protectedRanges = worksheet.AllowEditRanges;
            
            // Ajouter une nouvelle plage protégée (A1:J10)
            int index = protectedRanges.Add("MyProtectedRange", 0, 0, 10, 10);
            
            // Obtenir la plage protégée
            ProtectedRange protectedRange = protectedRanges[index];
            
            // Définir le descripteur de sécurité
            string securityDescriptor = "O:WDG:WDD:(D;;CC;;;S-1-5-21-2854911246-2539335229-2923752399-1000)(A;;CC;;;S-1-5-21-2854911246-2539335229-2923752399-1013)";
            protectedRange.SecurityDescriptor = securityDescriptor;
            
            // Enregistrez le classeur
            workbook.Save("ProtectedRangeDemo.xlsx");
            
            Console.WriteLine("Protected range demo completed successfully.");
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


