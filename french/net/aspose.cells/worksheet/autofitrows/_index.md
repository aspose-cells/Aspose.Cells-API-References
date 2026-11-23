---
title: "Worksheet.AutoFitRows"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Worksheet. Ajuste automatiquement toutes les lignes de cette feuille de calcul"
type: docs
url: /fr/net/aspose.cells/worksheet/autofitrows/
---
## AutoFitRows(AutoFitterOptions) {#autofitrows_1}

Ajuste automatiquement toutes les lignes de cette feuille de calcul.

```csharp
public void AutoFitRows(AutoFitterOptions options)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| options | AutoFitterOptions | Les options de l'ajusteur automatique |

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodAutoFitRowsWithAutoFitterOptionsDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Définir des données d'exemple et le formatage
            worksheet.Cells["A1"].PutValue("This is a long text that will need auto-fitting");
            worksheet.Cells["A2"].PutValue("Another long text\nwith multiple lines\nfor demonstration");
            
            // Fusionner les cellules pour démontrer l'ajustement automatique des cellules fusionnées
            worksheet.Cells.Merge(3, 0, 2, 1);
            worksheet.Cells["A3"].PutValue("Merged cells text that needs to fit");

            // Ajuster automatiquement les lignes avec des options spécifiques
            worksheet.AutoFitRows(new AutoFitterOptions
            {
                AutoFitMergedCellsType = AutoFitMergedCellsType.EachLine,
                AutoFitWrappedTextType = AutoFitWrappedTextType.Paragraph,
                MaxRowHeight = 100,  // Set reasonable max height
                OnlyAuto = true
            });

            // Enregistrez le classeur
            workbook.Save("AutoFitRowsDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [AutoFitterOptions](../../autofitteroptions/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## AutoFitRows(int, int) {#autofitrows_3}

Ajuste automatiquement la hauteur de la ligne dans une plage.

```csharp
public void AutoFitRows(int startRow, int endRow)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| startRow | Int32 | Indice de ligne de départ. |
| endRow | Int32 | Indice de ligne de fin. |

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodAutoFitRowsWithInt32Int32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            Cells cells = sheet.Cells;

            // Remplir les cellules avec des données d'exemple et des styles
            for (int i = 0; i <= 8; i++)
            {
                Cell cell = cells[i, i];
                cell.Value = "Sample text for row " + i;
                
                if (i % 2 == 0)
                {
                    Style style = cell.GetStyle();
                    style.SetBorder(BorderType.BottomBorder, CellBorderType.Thin, System.Drawing.Color.Black);
                    cell.SetStyle(style);
                }
            }

            // Ajuster automatiquement les lignes de l'index 0 à 8
            sheet.AutoFitRows(0, 8);

            // Afficher les hauteurs de ligne résultantes
            for (int i = 0; i <= 8; i++)
            {
                Console.WriteLine($"Row {i} height: {cells.GetRowHeightPixel(i)} pixels");
            }
        }
    }
}
```

### Voir aussi

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## AutoFitRows(int, int, AutoFitterOptions) {#autofitrows_4}

Ajuste automatiquement la hauteur de la ligne dans une plage.

```csharp
public void AutoFitRows(int startRow, int endRow, AutoFitterOptions options)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| startRow | Int32 | Indice de ligne de départ. |
| endRow | Int32 | Indice de ligne de fin. |
| options | AutoFitterOptions | Les options de l'ajusteur automatique. |

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodAutoFitRowsWithInt32Int32AutoFitterOptionsDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajoutez des données d'exemple aux cellules
            worksheet.Cells["A1"].PutValue("This is a test string for auto-fit row height demonstration");
            worksheet.Cells["A2"].PutValue("Another line\nwith multiple lines\nof text");
            
            // Créer des options d'ajustement automatique
            AutoFitterOptions options = new AutoFitterOptions();
            options.OnlyAuto = true;
            
            // Ajuster les lignes 0 à 1 avec des options
            worksheet.AutoFitRows(0, 1, options);
            
            // Enregistrez le classeur
            workbook.Save("AutoFitRowsDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [AutoFitterOptions](../../autofitteroptions/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## AutoFitRows() {#autofitrows}

Ajuste automatiquement toutes les lignes de cette feuille de calcul.

```csharp
public void AutoFitRows()
```

### Exemples

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodAutoFitRowsDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajoutez des données d'exemple aux cellules
            worksheet.Cells["A1"].PutValue("This is a test string for AutoFitRows demonstration");
            worksheet.Cells["A2"].PutValue("Another line of text\nwith line break to show row height adjustment");
            worksheet.Cells["B1"].PutValue("Column B content");
            
            // Ajuster automatiquement les lignes
            worksheet.AutoFitRows();
            
            // Ajuster automatiquement les colonnes pour une meilleure visibilité
            worksheet.AutoFitColumns();
            
            // Enregistrez le classeur
            string outputPath = Path.Combine(Environment.GetFolderPath(Environment.SpecialFolder.Desktop), "AutoFitRowsDemo.xlsx");
            workbook.Save(outputPath, SaveFormat.Xlsx);
            
            Console.WriteLine("Worksheet with AutoFitRows saved to: " + outputPath);
        }
    }
}
```

### Voir aussi

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## AutoFitRows(bool) {#autofitrows_2}

Ajuste automatiquement toutes les lignes de cette feuille de calcul.

```csharp
public void AutoFitRows(bool onlyAuto)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| onlyAuto | Boolean | True, ajuste automatiquement la hauteur de ligne lorsque la hauteur de ligne n'est pas personnalisée. |

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodAutoFitRowsWithBooleanDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajouter du texte d'exemple aux cellules pour démontrer l'ajustement automatique des lignes
            worksheet.Cells["A1"].PutValue("This is a sample text that will demonstrate AutoFitRows functionality");
            worksheet.Cells["A2"].PutValue("Another line of text\nwith line breaks\nto show multi-line row adjustment");
            
            // Ajuster automatiquement les lignes en tenant compte de la fusion automatique
            worksheet.AutoFitRows(true);
            
            // Enregistrez le classeur
            workbook.Save("AutoFitRowsDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


