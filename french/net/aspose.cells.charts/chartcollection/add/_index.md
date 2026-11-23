---
title: "ChartCollection.Add"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode ChartCollection. Ajoute un graphique à la collection"
type: docs
url: /fr/net/aspose.cells.charts/chartcollection/add/
---
## Add(ChartType, int, int, int, int) {#add}

Ajoute un graphique à la collection.

```csharp
public int Add(ChartType type, int topRow, int leftColumn, int bottomRow, int rightColumn)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| type | ChartType | Type de graphique |
| topRow | Int32 | Indice de la ligne supérieure gauche. |
| leftColumn | Int32 | Indice de la colonne supérieure gauche. |
| bottomRow | Int32 | Index de la ligne du coin inférieur droit |
| rightColumn | Int32 | Index de la colonne du coin inférieur droit |

### Valeur de retour

[`Chart`](../../chart/) object index.

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartCollectionMethodAddWithChartTypeInt32Int32Int32Int32Demo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Ajouter des données d'exemple pour le graphique
            sheet.Cells["A1"].PutValue("Category");
            sheet.Cells["B1"].PutValue("Value");
            for (int i = 1; i <= 10; i++)
            {
                sheet.Cells["A" + (i + 1)].PutValue("Cat " + i);
                sheet.Cells["B" + (i + 1)].PutValue(i * 10);
            }

            // Ajouter un graphique en utilisant les paramètres spécifiés
            int chartIndex = sheet.Charts.Add(ChartType.Column, 5, 2, 25, 11);
            Chart chart = sheet.Charts[chartIndex];

            // Définir la source de données du graphique
            chart.NSeries.Add("=Sheet1!$A$1:$B$11", true);

            // Enregistrez le classeur
            workbook.Save("output.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Voir aussi

* enum [ChartType](../../charttype/)
* class [ChartCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)

---

## Add(ChartType, string, int, int, int, int) {#add_2}

Ajoute un graphique à la collection.

```csharp
[Obsolete("Use ChartCollection.Add(ChartType, string, bool ,int , int, int, int ) instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int Add(ChartType type, string dataRange, int topRow, int leftColumn, int rightRow, 
    int bottomColumn)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| type | ChartType | Type de graphique |
| dataRange | String | Spécifie la plage de données du graphique |
| topRow | Int32 | Indice de la ligne supérieure gauche. |
| leftColumn | Int32 | Indice de la colonne supérieure gauche. |
| rightRow | Int32 | Index de la ligne du coin inférieur droit |
| bottomColumn | Int32 | Index de la colonne du coin inférieur droit |

### Valeur de retour

[`Chart`](../../chart/) object index.

### Remarques

NOTE : Ce membre est maintenant obsolète. À la place, veuillez utiliser la propriété `Add`. Cette propriété sera supprimée 12 mois plus tard à compter de mai 2022. Aspose s'excuse pour tout désagrément que vous avez pu rencontrer.

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartCollectionMethodAddWithChartTypeStringInt32Int32Int32Demo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter des données d'exemple pour le graphique
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            try
            {
                // Appelez la méthode Add avec les paramètres (ChartType, String, Int32, Int32, Int32, Int32)
                int chartIndex = worksheet.Charts.Add(
                    ChartType.Column,          // Chart type
                    "A1:B4",                  // Data range
                    0,                        // Top row position
                    3,                        // Left column position
                    15,                       // Bottom row position
                    8                         // Right column position
                );

                Console.WriteLine("Chart added successfully at index: " + chartIndex);
                
                // Accéder au graphique nouvellement créé
                Chart chart = worksheet.Charts[chartIndex];
                chart.Title.Text = "Sample Column Chart";
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Add method: {ex.Message}");
            }
            
            // Enregistrer le résultat
            workbook.Save("ChartCollectionMethodAddDemo.xlsx");
        }
    }
}
```

### Voir aussi

* enum [ChartType](../../charttype/)
* class [ChartCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)

---

## Add(byte[], string, bool, int, int, int, int) {#add_3}

Ajoute un graphique avec un modèle prédéfini.

```csharp
public int Add(byte[] data, string dataRange, bool isVertical, int topRow, int leftColumn, 
    int rightRow, int bottomColumn)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| données | Byte[] | Les données du fichier de modèle de graphique (.crtx). |
| dataRange | String | Spécifie la plage de données du graphique |
| isVertical | Boolean | Spécifie s'il faut tracer la série à partir d'une plage de valeurs de cellules par ligne ou par colonne. |
| topRow | Int32 | Indice de la ligne supérieure gauche. |
| leftColumn | Int32 | Indice de la colonne supérieure gauche. |
| rightRow | Int32 | Index de la ligne du coin inférieur droit |
| bottomColumn | Int32 | Index de la colonne du coin inférieur droit |

### Valeur de retour

[`Chart`](../../chart/) object index.

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartCollectionMethodAddWithByteArrayStringBooleanInt32Int32Int32Int32Demo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter des données d'exemple à la feuille de calcul
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Créer un tableau d'octets représentant les données du graphique (exemple simplifié)
            byte[] chartData = new byte[] { 0x01, 0x02, 0x03 };

            try
            {
                // Appeler la méthode Add avec des paramètres spécifiques
                int chartIndex = worksheet.Charts.Add(
                    chartData,          // Byte[] data
                    "A1:B4",            // String dataRange
                    true,               // Boolean isVertical
                    0,                  // Int32 topRow
                    0,                  // Int32 leftColumn
                    15,                 // Int32 rightRow
                    8                   // Int32 bottomColumn
                );

                Console.WriteLine($"Chart added successfully at index: {chartIndex}");

                // Accéder au graphique ajouté
                Chart chart = worksheet.Charts[chartIndex];
                chart.Type = ChartType.Column;

                // Enregistrer le résultat
                workbook.Save("ChartCollectionMethodAddDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Add method: {ex.Message}");
            }
        }
    }
}
```

### Voir aussi

* class [ChartCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)

---

## Add(ChartType, string, bool, int, int, int, int) {#add_1}

Ajoute un graphique à la collection.

```csharp
public int Add(ChartType type, string dataRange, bool isVertical, int topRow, int leftColumn, 
    int rightRow, int bottomColumn)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| type | ChartType | Type de graphique |
| dataRange | String | Spécifie la plage de données du graphique |
| isVertical | Boolean | Spécifie s'il faut tracer la série à partir d'une plage de valeurs de cellules par ligne ou par colonne. |
| topRow | Int32 | Indice de la ligne supérieure gauche. |
| leftColumn | Int32 | Indice de la colonne supérieure gauche. |
| rightRow | Int32 | Index de la ligne du coin inférieur droit |
| bottomColumn | Int32 | Index de la colonne du coin inférieur droit |

### Valeur de retour

[`Chart`](../../chart/) object index.

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartCollectionMethodAddWithChartTypeStringBooleanInt32IntDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajoutez des données d'exemple
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Series1");
            worksheet.Cells["C1"].PutValue("Series2");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["C2"].PutValue(20);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(30);
            worksheet.Cells["C3"].PutValue(40);

            // Ajouter un graphique avec les paramètres spécifiés
            int chartIndex = worksheet.Charts.Add(ChartType.Column, "A1:C3", true, 4, 4, 14, 10);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            workbook.Save("output.xlsx");
        }
    }
}
```

### Voir aussi

* enum [ChartType](../../charttype/)
* class [ChartCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


