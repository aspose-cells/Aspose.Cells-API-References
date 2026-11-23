---
title: "WorksheetCollection.AddCopy"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode WorksheetCollection. Ajoute une feuille de calcul à la collection et copie les données d'une feuille de calcul existante."
type: docs
url: /fr/net/aspose.cells/worksheetcollection/addcopy/
---
## AddCopy(string) {#addcopy_1}

Ajoute une feuille de calcul à la collection et copie les données d'une feuille de calcul existante.

```csharp
public int AddCopy(string sheetName)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| sheetName | String | Nom de la feuille de calcul source. |

### Valeur de retour

[`Worksheet`](../../worksheet/) object index.

### Exceptions

| exception | condition |
| --- | --- |
| [CellsException](../../cellsexception/) | Spécifie un nom de feuille de calcul invalide. |

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetCollectionMethodAddCopyWithStringDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Ajouter une feuille de calcul nommée "Original" au classeur
            Worksheet originalSheet = workbook.Worksheets.Add("Original");
            
            // Ajouter des données à la feuille de calcul originale
            originalSheet.Cells["A1"].PutValue("This is the original sheet");
            
            // Faire une copie de la feuille de calcul "Original"
            int copiedIndex = workbook.Worksheets.AddCopy("Original");
            Worksheet copiedSheet = workbook.Worksheets[copiedIndex];
            copiedSheet.Name = "CopiedSheet";
            
            // Modifier la feuille copiée pour démontrer qu'il s'agit d'une copie distincte
            copiedSheet.Cells["A1"].PutValue("This is the copied sheet");
            
            // Enregistrez le classeur
            workbook.Save("WorksheetCopyDemo.xlsx");
            
            Console.WriteLine("Worksheet copied successfully. Output file: WorksheetCopyDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## AddCopy(int) {#addcopy}

Ajoute une feuille de calcul à la collection et copie les données d'une feuille de calcul existante.

```csharp
public int AddCopy(int sheetIndex)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| sheetIndex | Int32 | Indice de la feuille de calcul source. |

### Valeur de retour

[`Worksheet`](../../worksheet/) object index.

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetCollectionMethodAddCopyWithInt32Demo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul et ajouter des données
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Original Worksheet");
            
            // Ajouter une copie de la première feuille de calcul
            workbook.Worksheets.AddCopy(0);
            
            // Vérifier que la copie a été créée
            Worksheet copiedWorksheet = workbook.Worksheets[1];
            copiedWorksheet.Cells["A1"].PutValue("Copied Worksheet");
            
            // Enregistrez le classeur
            workbook.Save("output.xlsx");
        }
    }
}
```

### Voir aussi

* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## AddCopy(Worksheet[], string[]) {#addcopy_2}

Copier un groupe de feuilles de calcul.

```csharp
public void AddCopy(Worksheet[] source, string[] destSheetNames)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| source | Worksheet[] | Les feuilles de calcul source. |
| destSheetNames | String[] | Les noms des feuilles copiées. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class WorksheetCollectionMethodAddCopyWithWorksheetStringDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Ajouter quelques feuilles de calcul d'exemple
            workbook.Worksheets.Add("Sheet2");
            workbook.Worksheets.Add("Sheet3");
            
            // Remplir certaines données dans les feuilles de calcul
            workbook.Worksheets["Sheet2"].Cells["A1"].PutValue("Original Sheet1 Data");
            workbook.Worksheets["Sheet3"].Cells["A1"].PutValue("Original Sheet2 Data");

            // Préparer le tableau des feuilles de calcul source
            Worksheet[] sourceSheets = new Worksheet[]
            {
                workbook.Worksheets["Sheet2"],
                workbook.Worksheets["Sheet3"]
            };

            // Préparer le tableau des noms de feuilles de destination
            string[] destSheetNames = new string[]
            {
                "CopyOfSheet2",
                "CopyOfSheet3"
            };

            try
            {
                // Appeler la méthode AddCopy avec les paramètres (Worksheet[], String[])
                workbook.Worksheets.AddCopy(sourceSheets, destSheetNames);
                
                Console.WriteLine("AddCopy method executed successfully with parameters (Worksheet[], String[])");
                
                // Vérifier que les copies ont été créées
                Console.WriteLine($"Total worksheets after copy: {workbook.Worksheets.Count}");
                foreach (Worksheet sheet in workbook.Worksheets)
                {
                    Console.WriteLine($"Worksheet name: {sheet.Name}");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing AddCopy method: {ex.Message}");
            }
            
            // Enregistrer le résultat
            workbook.Save("WorksheetCollectionMethodAddCopyDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Worksheet](../../worksheet/)
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


