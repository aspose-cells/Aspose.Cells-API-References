---
title: "Worksheet.AutoFitColumn"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Worksheet. Ajuste automatiquement la largeur de la colonne"
type: docs
url: /fr/net/aspose.cells/worksheet/autofitcolumn/
---
## AutoFitColumn(int, int, int) {#autofitcolumn_1}

Ajuste automatiquement la largeur de la colonne.

```csharp
public void AutoFitColumn(int columnIndex, int firstRow, int lastRow)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| columnIndex | Int32 | Index de colonne. |
| firstRow | Int32 | Indice de la première ligne. |
| lastRow | Int32 | Indice de la dernière ligne. |

### Remarques

Cette méthode ajuste automatiquement une ligne en fonction du contenu d'une plage de cellules de la ligne.

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class WorksheetMethodAutoFitColumnWithInt32Int32Int32Demo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Remplir les cellules avec des données d'exemple qui nécessiteront un ajustement de la largeur de colonne
            worksheet.Cells["A1"].PutValue("Short text");
            worksheet.Cells["A2"].PutValue("This is a much longer piece of text that will require column width adjustment");
            worksheet.Cells["A3"].PutValue("Another long text entry to demonstrate AutoFitColumn");
            
            try
            {

                Console.WriteLine($"Column width before: {worksheet.Cells.GetColumnWidth(0)}");
                // Appeler AutoFitColumn sur la colonne A (indice 0) pour les lignes 0 à 2 (indexation à partir de zéro)
                worksheet.AutoFitColumn(0, 0, 2);
                
                Console.WriteLine("AutoFitColumn method executed successfully on column A for rows 1-3");
                
                // Afficher l'effet en montrant la largeur de la colonne avant et après                
                Console.WriteLine($"Column width after: {worksheet.Cells.GetColumnWidth(0)}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing AutoFitColumn method: {ex.Message}");
            }
            
            // Enregistrer le résultat
            workbook.Save("AutoFitColumnWithInt32Int32Int32Demo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## AutoFitColumn(int) {#autofitcolumn}

Ajuste automatiquement la largeur de la colonne.

```csharp
public void AutoFitColumn(int columnIndex)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| columnIndex | Int32 | Index de colonne. |

### Remarques

AutoFitColumn est une fonction imprécise.

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodAutoFitColumnWithInt32Demo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajouter des données d'exemple aux cellules de la colonne 4 (indice basé sur 0)
            worksheet.Cells["D1"].PutValue("This is a test");
            worksheet.Cells["D2"].PutValue("AutoFitColumn demonstration");
            worksheet.Cells["D3"].PutValue("Aspose.Cells for .NET");
            
            // Ajuster automatiquement la colonne 4 (indice basé sur 0)
            worksheet.AutoFitColumn(3);
            
            // Enregistrez le classeur
            workbook.Save("output.xlsx");
        }
    }
}
```

### Voir aussi

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


