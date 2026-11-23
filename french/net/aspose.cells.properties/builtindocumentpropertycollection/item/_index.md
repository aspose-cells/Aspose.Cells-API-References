---
title: "BuiltInDocumentPropertyCollection.Item"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété BuiltInDocumentPropertyCollection. Retourne un objet DocumentProperty par le nom de la propriété"
type: docs
url: /fr/net/aspose.cells.properties/builtindocumentpropertycollection/item/
---
## BuiltInDocumentPropertyCollection indexer

Retourne un objet [`DocumentProperty`](../../documentproperty/) par le nom de la propriété.

```csharp
public override DocumentProperty this[string name] { get; }
```

| Paramètre | Description |
| --- | --- |
| name | Le nom de la propriété à récupérer, insensible à la casse. |

### Remarques

Les noms de chaîne des propriétés correspondent aux noms des propriétés typées disponibles depuis [`BuiltInDocumentPropertyCollection`](../).

Si vous demandez une propriété qui n'est pas présente dans le document, mais que le nom de la propriété est reconnu comme un nom intégré valide, un nouveau [`DocumentProperty`](../../documentproperty/) est créé, ajouté à la collection et retourné. La propriété nouvellement créée reçoit une valeur par défaut (chaîne vide, zéro, false ou DateTime.MinValue selon le type de la propriété intégrée).

Si vous demandez une propriété qui n'est pas présente dans le document et que le nom n'est pas reconnu comme un nom intégré, null est retourné.

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class BuiltInDocumentPropertyCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Définissez une propriété de document intégrée en utilisant la méthode appropriée
            workbook.BuiltInDocumentProperties["Version"].Value = "15.0300";
            
            // Accédez et affichez la valeur de la propriété
            Console.WriteLine("Version: " + workbook.BuiltInDocumentProperties["Version"].Value);
            
            // Enregistrez le classeur
            workbook.Save("output.xlsx");
            
            // Chargez le classeur enregistré et vérifiez la propriété
            Workbook loadedWorkbook = new Workbook("output.xlsx");
            Console.WriteLine("Loaded Version: " + loadedWorkbook.BuiltInDocumentProperties["Version"].Value);
        }
    }
}
```

### Voir aussi

* class [DocumentProperty](../../documentproperty/)
* class [BuiltInDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


