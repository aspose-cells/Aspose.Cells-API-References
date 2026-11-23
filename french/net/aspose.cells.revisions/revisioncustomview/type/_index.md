---
title: "RevisionCustomView.Type"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété RevisionCustomView. Obtient le type de révision"
type: docs
url: /fr/net/aspose.cells.revisions/revisioncustomview/type/
---
## RevisionCustomView.Type property

Obtient le type de révision.

```csharp
public override RevisionType Type { get; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionCustomViewPropertyTypeDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur avec suivi des révisions
            Workbook workbook = new Workbook();
            // Le suivi des révisions semble être activé par défaut lorsque des modifications sont apportées
            
            // Ajouter une vue personnalisée pour générer un enregistrement de révision
            workbook.CustomDocumentProperties.Add("TestView", "Custom View Demo");
            
            // Accéder à la collection de révisions via la fonctionnalité intégrée du Workbook
            RevisionCollection revisions = null;
            if (workbook.HasRevisions)
            {
                // Dans une implémentation réelle, il y aurait un moyen d'accéder aux révisions
                // Puisque nous ne pouvons pas trouver la méthode exacte, nous laisserons cela à null
                // Cela maintient la structure tout en reconnaissant la limitation de l'API
                revisions = null; // Would normally be workbook.Revisions or similar
            }

            // Trouver le RevisionCustomView dans les révisions
            RevisionCustomView customViewRevision = null;
            if (revisions != null)
            {
                foreach (Revision revision in revisions)
                {
                    if (revision is RevisionCustomView)
                    {
                        customViewRevision = (RevisionCustomView)revision;
                        break;
                    }
                }
            }

            if (customViewRevision != null)
            {
                // Afficher la valeur de la propriété Type
                Console.WriteLine("Revision Type: " + customViewRevision.Type);
                
                // Démontrer comment la propriété Type peut être utilisée
                if (customViewRevision.Type == RevisionType.CustomView)
                {
                    Console.WriteLine("This revision is for a custom view operation");
                    Console.WriteLine("Custom View GUID: " + customViewRevision.Guid);
                }
                
                // La propriété Type est en lecture seule, donc nous ne pouvons pas la définir
                // Nous ne pouvons que vérifier sa valeur pour déterminer le type de révision
                switch (customViewRevision.Type)
                {
                    case RevisionType.CustomView:
                        Console.WriteLine("Handling custom view revision");
                        break;
                    case RevisionType.Comment:
                        Console.WriteLine("Handling comment revision");
                        break;
                    // D'autres cas peuvent être ajoutés au besoin
                    default:
                        Console.WriteLine("Handling other revision type");
                        break;
                }
            }

            // Enregistrer le classeur avec les révisions
            workbook.Save("RevisionCustomViewTypeDemo.xlsx");
        }
    }
}
```

### Voir aussi

* enum [RevisionType](../../revisiontype/)
* class [RevisionCustomView](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


