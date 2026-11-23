---
title: "SheetSet.SheetSet"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Constructeur SheetSet. Crée un ensemble de feuilles basé sur des index de feuilles exacts"
type: docs
url: /fr/net/aspose.cells.rendering/sheetset/sheetset/
---
## SheetSet(params int[]) {#constructor}

Crée un ensemble de feuilles basé sur les index de feuilles exacts.

```csharp
public SheetSet(params int[] sheetIndexes)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| sheetIndexes | Int32[] | index de feuilles basés sur zéro. |

### Remarques

Si une feuille est rencontrée qui n'est pas dans le classeur, une exception sera levée lors du rendu.

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class SheetSetMethodCtorWithInt32ArrayDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur avec 3 feuilles de calcul
            Workbook workbook = new Workbook();
            workbook.Worksheets.Add("Sheet2");
            workbook.Worksheets.Add("Sheet3");

            // Ajouter du texte d'identification à chaque feuille
            workbook.Worksheets[0].Cells["A1"].PutValue("This is Sheet 1");
            workbook.Worksheets[1].Cells["A1"].PutValue("This is Sheet 2");
            workbook.Worksheets[2].Cells["A1"].PutValue("This is Sheet 3");

            try
            {
                // Créer SheetSet avec des index de feuilles spécifiques (0 et 2)
                SheetSet sheetSet = new SheetSet(new int[] { 0, 2 });

                // Créer des options d'enregistrement PDF avec notre ensemble de feuilles
                PdfSaveOptions options = new PdfSaveOptions();
                options.SheetSet = sheetSet;

                // Enregistrer le classeur avec les feuilles sélectionnées
                workbook.Save("SheetSetDemo.pdf", options);
                Console.WriteLine("Created PDF containing Sheet 1 and Sheet 3");
            }
            catch (ArgumentOutOfRangeException ex)
            {
                Console.WriteLine($"Invalid sheet index specified: {ex.Message}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Voir aussi

* class [SheetSet](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)

---

## SheetSet(params string[]) {#constructor_1}

Crée un ensemble de feuilles basé sur les noms de feuilles exacts.

```csharp
public SheetSet(params string[] sheetNames)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| sheetNames | String[] | noms de feuilles. |

### Remarques

Si une feuille est rencontrée qui n'est pas dans le classeur, une exception sera levée lors du rendu.

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class SheetSetMethodCtorWithStringArrayDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur et ajouter des feuilles
            Workbook workbook = new Workbook();
            workbook.Worksheets[0].Name = "First";
            workbook.Worksheets.Add("Second");
            workbook.Worksheets.Add("Third");

            workbook.Worksheets["First"].Cells["A1"].PutValue("This is Sheet 1");
            workbook.Worksheets["Second"].Cells["A1"].PutValue("This is Sheet 2");
            workbook.Worksheets["Third"].Cells["A1"].PutValue("This is Sheet 3");

            // Préparer les noms de feuilles pour SheetSet
            string[] selectedSheets = { "First", "Third" };

            try
            {
                // Créer SheetSet avec un paramètre tableau de chaînes
                SheetSet sheetSet = new SheetSet(selectedSheets);

                // Configurer les options d’enregistrement PDF avec le SheetSet créé
                PdfSaveOptions pdfOptions = new PdfSaveOptions();
                pdfOptions.SheetSet = sheetSet;

                // Enregistrer le classeur en PDF avec les feuilles spécifiées
                workbook.Save("SheetSetOutput.pdf", pdfOptions);

                Console.WriteLine("Created PDF with sheets: " + string.Join(", ", selectedSheets));
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error creating SheetSet: {ex.Message}");
            }
        }
    }
}
```

### Voir aussi

* class [SheetSet](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


