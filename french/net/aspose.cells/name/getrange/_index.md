---
title: "Name.GetRange"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Name. Obtient la plage si ce nom fait référence à une plage"
type: docs
url: /fr/net/aspose.cells/name/getrange/
---
## GetRange() {#getrange}

Obtient la plage si ce nom fait référence à une plage.

```csharp
public Range GetRange()
```

### Valeur de retour

La plage.

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class NameMethodGetRangeDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajoutez des données d'exemple aux cellules
            worksheet.Cells["A1"].PutValue("Item");
            worksheet.Cells["B1"].PutValue("Quantity");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["B3"].PutValue(15);
            
            // Créer une plage nommée
            int index = workbook.Worksheets.Names.Add("MyRange");
            workbook.Worksheets.Names[index].RefersTo = "=Sheet1!A1:B3";
            Name namedRange = workbook.Worksheets.Names[index];
            
            // Démontrer la méthode GetRange
            Aspose.Cells.Range range = namedRange.GetRange();
            Console.WriteLine("Named Range Address: " + range.Address);
            Console.WriteLine("Worksheet Name: " + range.Worksheet.Name);
            
            // Modifier la plage
            foreach (Cell cell in range)
            {
                if (cell.Row == 0)
                {
                    cell.PutValue(cell.StringValue.ToUpper());
                }
            }
            
            // Enregistrez le classeur
            workbook.Save("NamedRangeDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Range](../../range/)
* class [Name](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetRange(bool) {#getrange_1}

Obtient la plage si ce nom fait référence à une plage

```csharp
public Range GetRange(bool recalculate)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| recalculer | Boolean | si le recalcul doit être effectué si ce nom a déjà été calculé avant cet appel. |

### Valeur de retour

La plage.

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class NameMethodGetRangeWithBooleanDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            Cells cells = sheet.Cells;

            // Remplissez des données d'exemple
            for (int i = 0; i < 4; i++)
            {
                cells[i, 1].PutValue(i); // Column B values: 0,1,2,3
            }

            // Créer une plage nommée avec formule
            int nameIndex = wb.Worksheets.Names.Add("testname");
            Name name = wb.Worksheets.Names[nameIndex];
            name.RefersTo = "IFERROR(Sheet1!$B$2:$B$4,-1)";

            // Utiliser la plage nommée dans les formules
            cells["C1"].Formula = "=testname";
            cells["D1"].Formula = "SUM(testname)";

            // Calculer les formules
            wb.CalculateFormula();

            // Obtenir la plage en utilisant GetRange(true)
            Aspose.Cells.Range namedRange = name.GetRange(true);
            Console.WriteLine($"Named range: FirstRow={namedRange.FirstRow}, FirstColumn={namedRange.FirstColumn}, " +
                $"RowCount={namedRange.RowCount}, ColumnCount={namedRange.ColumnCount}");

            // Créer un graphique en utilisant la plage nommée
            int chartIndex = sheet.Charts.Add(ChartType.Column, 10, 1, 20, 5);
            Chart chart = sheet.Charts[chartIndex];
            chart.NSeries.Add("testname", true);
            Console.WriteLine($"Chart data points count: {chart.NSeries[0].CountOfDataValues}");
        }
    }
}
```

### Voir aussi

* class [Range](../../range/)
* class [Name](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetRange(int, int, int) {#getrange_2}

Obtient la plage si ce nom fait référence à une plage. Si la référence de ce nom n’est pas absolue, la plage peut différer selon la cellule.

```csharp
public Range GetRange(int sheetIndex, int row, int column)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| sheetIndex | Int32 | L'index de feuille correspondant. |
| ligne | Int32 | L'index de ligne correspondant. |
| column | Int32 | L'index de colonne correspondant |

### Valeur de retour

La plage.

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class NameMethodGetRangeWithInt32Int32Int32Demo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajoutez des données d'exemple
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Fruits");
            worksheet.Cells["A3"].PutValue("Vegetables");
            worksheet.Cells["A4"].PutValue("Dairy");
            
            // Créer une plage nommée en utilisant la signature de méthode correcte
            int index = workbook.Worksheets.Names.Add("SubCat");
            workbook.Worksheets.Names["SubCat"].RefersTo = "=" + worksheet.Name + "!A2:A4";
            
            // Obtenir la plage en utilisant GetRange avec les paramètres ligne, colonne et nombre de lignes
            Aspose.Cells.Range range = workbook.Worksheets.Names["SubCat"].GetRange(0, 0, 3);
            
            // Afficher la référence de la plage
            Console.WriteLine("Range refers to: " + range.RefersTo);
        }
    }
}
```

### Voir aussi

* class [Range](../../range/)
* class [Name](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


