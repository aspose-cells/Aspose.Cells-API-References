---
title: "Worksheet.AutoFitRow"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Worksheet. Ajuste automatiquement la hauteur des lignes dans une plage rectangulaire"
type: docs
url: /fr/net/aspose.cells/worksheet/autofitrow/
---
## AutoFitRow(int, int, int, int) {#autofitrow_3}

Ajuste automatiquement la hauteur de la ligne dans une plage rectangulaire.

```csharp
public void AutoFitRow(int startRow, int endRow, int startColumn, int endColumn)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| startRow | Int32 | Indice de ligne de départ. |
| endRow | Int32 | Indice de ligne de fin. |
| startColumn | Int32 | Indice de colonne de départ. |
| endColumn | Int32 | Indice de colonne de fin. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class WorksheetMethodAutoFitRowWithInt32Int32Int32Int32Demo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            RowCollection rows = worksheet.Cells.Rows;
            rows[0].Height = 20;
            rows[1].Height = 20;
            // Ajouter des données d'exemple aux cellules pour démontrer l'ajustement automatique des lignes
            worksheet.Cells["A1"].PutValue("This is a long text that will demonstrate row autofit");
            worksheet.Cells["B1"].PutValue("Additional column with text");
            worksheet.Cells["A2"].PutValue("Shorter text");
            worksheet.Cells["B2"].PutValue("More text");
            
            try
            {
                Console.WriteLine($"Row 1 height before autofit: {worksheet.Cells.Rows[0].Height}");
                Console.WriteLine($"Row 2 height before autofit: {worksheet.Cells.Rows[1].Height}");

                // Appeler AutoFitRow avec les paramètres : startRow, endRow, startColumn, endColumn
                worksheet.AutoFitRow(0, 1, 0, 1);
                
                Console.WriteLine("AutoFitRow method executed successfully with parameters (0, 1, 0, 1)");
                
                // Afficher l'effet en montrant les hauteurs des lignes
                Console.WriteLine($"Row 1 height after autofit: {worksheet.Cells.Rows[0].Height}");
                Console.WriteLine($"Row 2 height after autofit: {worksheet.Cells.Rows[1].Height}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing AutoFitRow method: {ex.Message}");
            }
            
            // Enregistrer le résultat
            workbook.Save("AutoFitRowWithInt32Int32Int32Int32Demo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## AutoFitRow(int) {#autofitrow}

Ajuste automatiquement la hauteur de la ligne.

```csharp
public void AutoFitRow(int rowIndex)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| rowIndex | Int32 | Index de ligne. |

### Remarques

AutoFitRow est une fonction imprécise.

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodAutoFitRowWithInt32Demo
    {
        public static void Run()
        {
            // Créer un classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Définir un texte long avec retour à la ligne dans la cellule A1
            worksheet.Cells["A1"].Value = "LOOOOOOOOOOOOOOOOOONG TEEEEEEEEEEXT";
            Style style = worksheet.Cells["A1"].GetStyle();
            style.IsTextWrapped = true;
            worksheet.Cells["A1"].SetStyle(style);

            // Ajuster automatiquement la première ligne
            worksheet.AutoFitRow(0);

            // Enregistrez le classeur
            workbook.Save("AutoFitRowDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## AutoFitRow(int, int, int) {#autofitrow_1}

Ajuste automatiquement la hauteur de la ligne.

```csharp
public void AutoFitRow(int rowIndex, int firstColumn, int lastColumn)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| rowIndex | Int32 | Index de ligne. |
| firstColumn | Int32 | Indice de première colonne. |
| lastColumn | Int32 | Indice de dernière colonne. |

### Remarques

Cette méthode ajuste automatiquement une ligne en fonction du contenu d'une plage de cellules de la ligne.

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodAutoFitRowWithInt32Int32Int32Demo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajouter des données d'exemple aux cellules qui affecteront la hauteur de la ligne
            worksheet.Cells["A2"].PutValue("This is a long text that will demonstrate AutoFitRow functionality");
            worksheet.Cells["B2"].PutValue("Additional text in another column");
            
            // Ajuster automatiquement la ligne (ligne 2) entre les colonnes 0 et 1 (A à B)
            worksheet.AutoFitRow(1, 0, 1);
            
            // Enregistrez le classeur
            workbook.Save("AutoFitRowDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## AutoFitRow(int, int, int, AutoFitterOptions) {#autofitrow_2}

Ajuste automatiquement la hauteur de la ligne.

```csharp
public void AutoFitRow(int rowIndex, int firstColumn, int lastColumn, AutoFitterOptions options)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| rowIndex | Int32 | Index de ligne. |
| firstColumn | Int32 | Indice de première colonne. |
| lastColumn | Int32 | Indice de dernière colonne. |
| options | AutoFitterOptions | Les options de l'ajusteur automatique |

### Remarques

Cette méthode ajuste automatiquement une ligne en fonction du contenu d'une plage de cellules de la ligne.

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodAutoFitRowWithInt32Int32Int32AutoFitterOptioDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajoutez des données d'exemple aux cellules
            worksheet.Cells["A1"].PutValue("This is a test string for autofit");
            worksheet.Cells["B1"].PutValue("Another test string in column B");
            
            // Créer AutoFitterOptions
            AutoFitterOptions options = new AutoFitterOptions
            {
                AutoFitMergedCells = true,
                IgnoreHidden = false,
                OnlyAuto = false
            };

            // Obtenir la hauteur originale de la ligne
            double originalHeight = worksheet.Cells.GetRowHeight(0);
            Console.WriteLine($"Original row height: {originalHeight}");

            // Ajuster automatiquement la première ligne
            worksheet.AutoFitRow(0, 0, 2, options);

            // Obtenir la nouvelle hauteur de ligne
            double newHeight = worksheet.Cells.GetRowHeight(0);
            Console.WriteLine($"New row height after AutoFit: {newHeight}");

            // Enregistrez le classeur
            workbook.Save("AutoFitRowExample.xlsx");
        }
    }
}
```

### Voir aussi

* class [AutoFitterOptions](../../autofitteroptions/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


