---
title: "FormatCondition.GetFormula1"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode FormatCondition. Obtient la valeur ou l'expression associée à cette condition de formatage"
type: docs
url: /fr/net/aspose.cells/formatcondition/getformula1/
---
## GetFormula1(bool, bool) {#getformula1}

Obtient la valeur ou l'expression associée à cette condition de format.

```csharp
public string GetFormula1(bool isR1C1, bool isLocal)
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

    public class FormatConditionMethodGetFormula1WithBooleanBooleanDemo
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
            FormatConditionCollection fcc = worksheet.ConditionalFormattings[index];
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.EndRow = 2;
            area.StartColumn = 0;
            area.EndColumn = 0;
            fcc.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "10", "30");

            // Obtenir la première condition de formatage
            FormatCondition fc = fcc[0];

            try
            {
                // Appeler GetFormula1 avec des paramètres (Boolean, Boolean)
                string formula = fc.GetFormula1(false, false);
                
                Console.WriteLine("Formula1: " + formula);
                Console.WriteLine("Method executed successfully with parameters (Boolean, Boolean)");
                
                // Afficher l'effet en montrant la plage de format conditionnel
                Console.WriteLine($"Conditional format applied to range: A1:A3");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetFormula1 method: {ex.Message}");
            }
            
            // Enregistrer le résultat
            workbook.Save("FormatConditionMethodGetFormula1WithBooleanBooleanDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [FormatCondition](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetFormula1(bool, bool, int, int) {#getformula1_1}

Obtient la valeur ou l'expression de la mise en forme conditionnelle de la cellule.

```csharp
public string GetFormula1(bool isR1C1, bool isLocal, int row, int column)
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
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FormatConditionMethodGetFormula1WithBooleanBooleanInt32Int32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter une condition de formatage
            int formatIndex = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcc = worksheet.ConditionalFormattings[formatIndex];
            fcc.AddArea(CellArea.CreateCellArea(0, 0, 1, 0));
            int conditionIndex = fcc.AddCondition(FormatConditionType.Expression, OperatorType.None, "=IF(MOD(A1,2)=0,TRUE,FALSE)", null);

            // Obtenir la formule avec différents paramètres
            FormatCondition condition = fcc[conditionIndex];
            string formula1 = condition.GetFormula1(false, false, 0, 0);
            string formula2 = condition.GetFormula1(false, false, 1, 0);

            Console.WriteLine("Formula for row 0: " + formula1);
            Console.WriteLine("Formula for row 1: " + formula2);
        }
    }
}
```

### Voir aussi

* class [FormatCondition](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetFormula1(int, int) {#getformula1_2}

Obtient la formule de la mise en forme conditionnelle de la cellule.

```csharp
public string GetFormula1(int row, int column)
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

    public class FormatConditionMethodGetFormula1WithInt32Int32Demo
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

            // Ajouter une mise en forme conditionnelle
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcc = worksheet.ConditionalFormattings[index];
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.StartColumn = 0;
            area.EndRow = 2;
            area.EndColumn = 0;
            fcc.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "10", "30");

            // Obtenir la première condition de formatage
            FormatCondition fc = fcc[0];

            try
            {
                // Appeler GetFormula1 avec des paramètres de ligne et de colonne spécifiques
                string formula = fc.GetFormula1(0, 0);
                
                Console.WriteLine("Formula1 for cell (0,0): " + formula);
                Console.WriteLine("Method executed successfully with parameters (Int32, Int32)");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetFormula1 method: {ex.Message}");
            }
            
            // Enregistrer le résultat
            workbook.Save("FormatConditionMethodGetFormula1WithInt32Int32Demo.xlsx");
        }
    }
}
```

### Voir aussi

* class [FormatCondition](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


