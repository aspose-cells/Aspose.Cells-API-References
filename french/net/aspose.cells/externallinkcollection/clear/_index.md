---
title: "ExternalLinkCollection.Clear"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode ExternalLinkCollection. Supprime tous les liens externes"
type: docs
url: /fr/net/aspose.cells/externallinkcollection/clear/
---
## Clear() {#clear}

Supprime tous les liens externes.

```csharp
public void Clear()
```

### Remarques

Lors de la suppression des liens externes, toutes les formules qui y font référence seront également supprimées car les références deviennent invalides.

### Voir aussi

* class [ExternalLinkCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Clear(bool) {#clear_1}

Supprime tous les liens externes.

```csharp
public void Clear(bool updateReferencesAsLocal)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| updateReferencesAsLocal | Boolean | Indique s'il faut mettre à jour toutes les références des liens externes dans les formules vers les références du classeur actuel lui‑même. |

### Remarques

Si les références doivent être mises à jour, ces références des liens externes dans les formules seront remplacées par le classeur actuel lorsqu'il est possible. Par exemple, la formule originale d'une cellule est "='externalsource.xlam'!customfunction()", après la suppression des liens externes, la formule deviendra "=customfunction()" ; lorsque la formule originale est "='[externalsource.xlam]Sheet1'!$A$1", selon qu'il existe ou non une feuille nommée "Sheet1" dans le classeur actuel : si oui, la formule deviendra "=Sheet1!$A$1" ; sinon, elle deviendra "=#REF!$A$1". Si les références ne doivent pas être mises à jour, toutes les formules contenant des références aux liens externes seront également supprimées car ces références deviennent invalides.

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ExternalLinkCollectionMethodClearWithBooleanDemo
    {
        public static void Run()
        {
            // Créer un classeur
            Workbook workbook = new Workbook();
            
            // Ajouter quelques liens externes
            ExternalLinkCollection externalLinks = workbook.Worksheets.ExternalLinks;
            externalLinks.Add("externalWorkbook.xlsx", new string[] { "Sheet1" });
            externalLinks.Add("anotherExternal.xlsx", new string[] { "Sheet1" });
            
            Console.WriteLine("External links count before clear: " + externalLinks.Count);
            
            // Effacer avec updateReferences = true
            externalLinks.Clear(true);
            Console.WriteLine("External links count after clear (updateReferences=true): " + externalLinks.Count);
            
            // Ajouter à nouveau les liens
            externalLinks.Add("externalWorkbook.xlsx", new string[] { "Sheet1" });
            externalLinks.Add("anotherExternal.xlsx", new string[] { "Sheet1" });
            
            // Effacer avec updateReferences = false
            externalLinks.Clear(false);
            Console.WriteLine("External links count after clear (updateReferences=false): " + externalLinks.Count);
        }
    }
}
```

### Voir aussi

* class [ExternalLinkCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


