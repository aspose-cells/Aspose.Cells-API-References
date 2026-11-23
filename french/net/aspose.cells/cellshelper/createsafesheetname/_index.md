---
title: "CellsHelper.CreateSafeSheetName"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode CellsHelper. Vérifie le nom de feuille fourni et crée un nom valide si nécessaire. Si le nom de feuille fourni respecte les règles des noms de feuilles Excel, il est renvoyé. Sinon, la chaîne sera tronquée si sa longueur dépasse la limite et les caractères invalides seront remplacés par   puis la chaîne reconstruite sera renvoyée."
type: docs
url: /fr/net/aspose.cells/cellshelper/createsafesheetname/
---
## CreateSafeSheetName(string) {#createsafesheetname}

Vérifie le nom de feuille fourni et crée un nom valide si nécessaire. Si le nom de feuille fourni respecte les règles de nommage des feuilles Excel, il est renvoyé. Sinon, la chaîne sera tronquée si sa longueur dépasse la limite et les caractères invalides seront remplacés par ' ', puis la valeur de chaîne reconstruite sera renvoyée.

```csharp
public static string CreateSafeSheetName(string nameProposal)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| nameProposal | String | nom de feuille à utiliser |

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsHelperMethodCreateSafeSheetNameWithStringDemo
    {
        public static void Run()
        {
            string unsafeName = "sheet*/test*/?#";
            string safeName = CellsHelper.CreateSafeSheetName(unsafeName);
            Console.WriteLine("Original name: " + unsafeName);
            Console.WriteLine("Safe name: " + safeName);
        }
    }
}
```

### Voir aussi

* class [CellsHelper](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## CreateSafeSheetName(string, char) {#createsafesheetname_1}

Vérifie le nom de feuille fourni et crée un nom valide si nécessaire. Si le nom de feuille fourni respecte les règles de nommage des feuilles Excel, il est renvoyé. Sinon, la chaîne sera tronquée si sa longueur dépasse la limite et les caractères invalides seront remplacés par le caractère fourni, puis la valeur de chaîne reconstruite sera renvoyée.

```csharp
public static string CreateSafeSheetName(string nameProposal, char replaceChar)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| nameProposal | String | nom de feuille à utiliser |
| replaceChar | Char | caractère qui sera utilisé pour remplacer les caractères invalides dans le nom de feuille donné |

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsHelperMethodCreateSafeSheetNameWithStringCharDemo
    {
        public static void Run()
        {
            // Exemple 1 : créer un nom de feuille sûr avec le caractère de remplacement par défaut
            string name1 = CellsHelper.CreateSafeSheetName("sheet*/test*/?#");
            Console.WriteLine("Safe sheet name (default replacement): " + name1);

            // Exemple 2 : créer un nom de feuille sûr avec le caractère de remplacement personnalisé 'A'
            string name2 = CellsHelper.CreateSafeSheetName("sheet*/test*/?#", 'A');
            Console.WriteLine("Safe sheet name (custom replacement): " + name2);
        }
    }
}
```

### Voir aussi

* class [CellsHelper](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


