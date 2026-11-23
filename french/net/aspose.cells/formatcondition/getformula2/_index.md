---
title: "FormatCondition.GetFormula2"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode FormatCondition. Obtient la valeur ou l'expression associée à cette condition de formatage"
type: docs
url: /fr/net/aspose.cells/formatcondition/getformula2/
---
## GetFormula2(bool, bool) {#getformula2}

Obtient la valeur ou l'expression associée à cette condition de format.

```csharp
public string GetFormula2(bool isR1C1, bool isLocal)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| isR1C1 | Boolean | Indique si la formule doit être formatée en R1C1. |
| isLocal | Boolean | Indique si la formule doit être formatée selon la locale. |

### Valeur de retour

La valeur ou l'expression associée à cette condition de format.

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class FormatConditionMethodGetFormula2WithBooleanBooleanDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajoutez des données d'exemple
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue(30);

            // Ajouter une condition de formatage
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = worksheet.ConditionalFormattings[index];
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.EndRow = 2;
            area.StartColumn = 0;
            area.EndColumn = 0;
            int conditionIndex = fcs.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "10", "30");
            FormatCondition fc = fcs[conditionIndex];
            
            // Définir Formula2
            fc.Formula2 = "30";

            try
            {
                // Appeler GetFormula2 avec des paramètres (Boolean, Boolean)
                string formula2 = fc.GetFormula2(false, false);
                
                // Afficher le résultat
                Console.WriteLine("Formula2: " + formula2);
                Console.WriteLine("Method executed successfully with parameters (Boolean, Boolean)");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetFormula2 method: {ex.Message}");
            }
            
            // Enregistrer le résultat
            workbook.Save("FormatConditionMethodGetFormula2WithBooleanBooleanDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [FormatCondition](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetFormula2(bool, bool, int, int) {#getformula2_1}

Obtient la valeur ou l'expression de la mise en forme conditionnelle de la cellule.

```csharp
public string GetFormula2(bool isR1C1, bool isLocal, int row, int column)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| isR1C1 | Boolean | Indique si la formule doit être formatée en R1C1. |
| isLocal | Boolean | Indique si la formule doit être formatée selon la locale. |
| ligne | Int32 | L'index de ligne. |
| column | Int32 | L'index de colonne. |

### Valeur de retour

La valeur ou l'expression associée au formatage conditionnel de la cellule.

### Remarques

La cellule donnée doit être contenue dans ce formatage conditionnel, sinon null sera retourné.

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class FormatConditionMethodGetFormula2WithBooleanBooleanInt32Int32Demo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajoutez des données d'exemple
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue(30);

            // Ajouter un format conditionnel
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = worksheet.ConditionalFormattings[index];
            int conditionIndex = fcs.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "=A1", "=A3");
            FormatCondition fc = fcs[conditionIndex];

            try
            {
                // Appeler GetFormula2 avec des paramètres spécifiques (isR1C1, isLocal, row, column)
                string formula = fc.GetFormula2(false, false, 0, 0);
                
                Console.WriteLine("Formula2 retrieved successfully: " + formula);
                Console.WriteLine("Method executed successfully with parameters (Boolean, Boolean, Int32, Int32)");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetFormula2 method: {ex.Message}");
            }
            
            // Enregistrer le résultat
            workbook.Save("FormatConditionMethodGetFormula2WithBooleanBooleanInt32Int32Demo.xlsx");
        }
    }
}
```

### Voir aussi

* class [FormatCondition](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetFormula2(int, int) {#getformula2_2}

Obtient la formule de la mise en forme conditionnelle de la cellule.

```csharp
public string GetFormula2(int row, int column)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| ligne | Int32 | L'index de ligne. |
| column | Int32 | L'index de colonne. |

### Valeur de retour

La formule.

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class FormatConditionMethodGetFormula2WithInt32Int32Demo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajoutez des données d'exemple
            worksheet.Cells["A1"].PutValue(5);
            worksheet.Cells["A2"].PutValue(15);
            worksheet.Cells["A3"].PutValue(25);
            worksheet.Cells["B1"].PutValue(10);
            worksheet.Cells["B2"].PutValue(20);
            worksheet.Cells["B3"].PutValue(30);

            // Ajouter une mise en forme conditionnelle
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcc = worksheet.ConditionalFormattings[index];
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.StartColumn = 0;
            area.EndRow = 2;
            area.EndColumn = 1;
            fcc.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "A1", "B3");

            // Obtenir la première condition de formatage
            FormatCondition fc = fcc[0];

            try
            {
                // Appeler GetFormula2 avec des paramètres spécifiques de ligne et de colonne
                string formula = fc.GetFormula2(1, 0); // Row 1, Column 0 (A2)
                
                Console.WriteLine("Formula2 for cell (1,0): " + formula);
                Console.WriteLine("Method executed successfully with parameters (Int32, Int32)");

                // Appliquer un style pour visualiser le formatage conditionnel
                Style style = workbook.CreateStyle();
                style.Font.Color = System.Drawing.Color.Red;
                fc.Style = style;
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetFormula2 method: {ex.Message}");
            }
            
            // Enregistrer le résultat
            workbook.Save("FormatConditionMethodGetFormula2WithInt32Int32Demo.xlsx");
        }
    }
}
```

### Voir aussi

* class [FormatCondition](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


