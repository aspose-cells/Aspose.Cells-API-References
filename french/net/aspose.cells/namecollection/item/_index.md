---
title: "NameCollection.Item"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété NameCollection. Obtient l'élément Name à l'index spécifié"
type: docs
url: /fr/net/aspose.cells/namecollection/item/
---
## NameCollection indexer (1 of 2)

Obtient l'élément [`Name`](../../name/) à l'index spécifié.

```csharp
public Name this[int index] { get; }
```

| Paramètre | Description |
| --- | --- |
| indice | L'indice à base zéro de l'élément. |

### Valeur de retour

L’élément à l’index spécifié.

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class NameCollectionPropertyItemDemo1
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Ajouter plusieurs feuilles de calcul
            workbook.Worksheets.Add("Sheet1");
            workbook.Worksheets.Add("Sheet2");
            workbook.Worksheets.Add("Sheet3");

            // Accéder à la collection de noms
            NameCollection names = workbook.Worksheets.Names;
            
            // Ajouter des plages nommées en utilisant la signature de méthode correcte
            int index1 = names.Add("Range1");
            names[index1].RefersTo = "=Sheet1!$A$1:$B$2";
            
            int index2 = names.Add("Range2");
            names[index2].RefersTo = "=Sheet2!$C$3:$D$4";
            
            int index3 = names.Add("Range3");
            names[index3].RefersTo = "=Sheet3!$E$5:$F$6";

            // Démontrer l'utilisation de la propriété Item
            Console.WriteLine("Named Ranges:");
            for (int i = 0; i < names.Count; i++)
            {
                Name name = names[i]; // Using Item property with index
                Console.WriteLine($"{name.Text}: {name.RefersTo}");
            }

            // Accéder par nom en utilisant la propriété Item
            Name specificName = names["Range2"];
            Console.WriteLine($"\nSpecific Range: {specificName.Text} refers to {specificName.RefersTo}");

            // Modifier une plage nommée
            names["Range3"].RefersTo = "=Sheet3!$A$1:$B$10";
            Console.WriteLine($"\nModified Range3 now refers to: {names["Range3"].RefersTo}");
        }
    }
}
```

### Voir aussi

* class [Name](../../name/)
* class [NameCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## NameCollection indexer (2 of 2)

Obtient l'élément [`Name`](../../name/) avec le nom spécifié.

```csharp
public Name this[string text] { get; }
```

| Paramètre | Description |
| --- | --- |
| texte | Texte du nom. |

### Valeur de retour

L'élément avec le nom spécifié.

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class NameCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la collection des noms des feuilles de calcul
            NameCollection names = workbook.Worksheets.Names;
            
            // Ajouter quelques plages nommées (corrigé pour utiliser la bonne signature de la méthode Add)
            int index1 = names.Add("Range1");
            names[index1].RefersTo = "=Sheet1!$A$1:$A$10";
            
            int index2 = names.Add("Range2");
            names[index2].RefersTo = "=Sheet1!$B$1:$B$10";
            
            // Accéder aux plages nommées en utilisant la propriété Item
            Name range1 = names["Range1"];
            Name range2 = names["Range2"];
            
            // Vérifier que les noms existent
            if (range1 != null && range2 != null)
            {
                Console.WriteLine("Named range 'Range1' refers to: " + range1.RefersTo);
                Console.WriteLine("Named range 'Range2' refers to: " + range2.RefersTo);
            }
            
            // Essayer d'accéder à un nom inexistant
            Name range3 = names["NonExistentRange"];
            if (range3 == null)
            {
                Console.WriteLine("Named range 'NonExistentRange' not found");
            }
        }
    }
}
```

### Voir aussi

* class [Name](../../name/)
* class [NameCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


