---
title: "WorksheetCollection.RemoveAt"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode WorksheetCollection. Supprime l'élément à un nom spécifié"
type: docs
url: /fr/net/aspose.cells/worksheetcollection/removeat/
---
## RemoveAt(string) {#removeat_2}

Supprime l'élément à un nom spécifié.

```csharp
public void RemoveAt(string name)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| name | String | Le nom de l'élément à supprimer. |

### Exemples

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetCollectionMethodRemoveAtWithStringDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook wb = new Workbook();
            
            // Ajouter plusieurs feuilles de calcul
            wb.Worksheets.Add("Sheet2");
            wb.Worksheets.Add("Sheet3");
            
            // Ajouter une plage nommée (fixe)
            int nameIndex = wb.Worksheets.Names.Add("testname");
            wb.Worksheets.Names[nameIndex].RefersTo = "=[Book1.xlsx]Sheet1!$A1";
            
            // Démontrer RemoveAt avec un paramètre de chaîne
            Console.WriteLine($"Before removal - Worksheet count: {wb.Worksheets.Count}");
            wb.Worksheets.RemoveAt("Sheet1");
            Console.WriteLine($"After removal - Worksheet count: {wb.Worksheets.Count}");
            
            // Enregistrez le classeur
            using (MemoryStream ms = new MemoryStream())
            {
                wb.Save(ms, SaveFormat.Xlsx);
            }
        }
    }
}
```

### Voir aussi

* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## RemoveAt(int) {#removeat}

Supprime l'élément à un index spécifié.

```csharp
public void RemoveAt(int index)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| indice | Int32 | La valeur d'index de l'élément à supprimer. |

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetCollectionMethodRemoveAtWithInt32Demo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook wb = new Workbook();
            
            // Ajouter plusieurs feuilles de calcul
            wb.Worksheets.Add("Sheet1");
            wb.Worksheets.Add("Sheet2");
            wb.Worksheets.Add("Sheet3");

            // Afficher le nombre de feuilles de calcul d'origine
            Console.WriteLine($"Original worksheet count: {wb.Worksheets.Count}");

            // Supprimer la feuille de calcul à l'index 1 (deuxième feuille)
            wb.Worksheets.RemoveAt(1);

            // Afficher le nombre de feuilles de calcul mis à jour
            Console.WriteLine($"After removal, worksheet count: {wb.Worksheets.Count}");

            // Enregistrez le classeur
            wb.Save("output.xlsx");
        }
    }
}
```

### Voir aussi

* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


