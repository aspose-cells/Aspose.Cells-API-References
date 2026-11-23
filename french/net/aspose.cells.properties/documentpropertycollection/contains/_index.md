---
title: "DocumentPropertyCollection.Contains"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode DocumentPropertyCollection. Retourne vrai si une propriété portant le nom spécifié existe dans la collection"
type: docs
url: /fr/net/aspose.cells.properties/documentpropertycollection/contains/
---
## DocumentPropertyCollection.Contains method

Renvoie true si une propriété portant le nom spécifié existe dans la collection.

```csharp
public bool Contains(string name)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| name | String | Le nom de la propriété, insensible à la casse. |

### Valeur de retour

Vrai si la propriété existe dans la collection ; faux sinon.

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DocumentPropertyCollectionMethodContainsWithStringDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Vérifier si la propriété "RevisionNumber" existe dans les propriétés de document intégrées
            bool containsRevision = workbook.BuiltInDocumentProperties.Contains("RevisionNumber");
            Console.WriteLine("Contains 'RevisionNumber': " + containsRevision);
            
            // Ajouter une propriété personnalisée et vérifier son existence
            workbook.CustomDocumentProperties.Add("CustomProperty", "Test Value");
            bool containsCustom = workbook.CustomDocumentProperties.Contains("CustomProperty");
            Console.WriteLine("Contains 'CustomProperty': " + containsCustom);
        }
    }
}
```

### Voir aussi

* class [DocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


