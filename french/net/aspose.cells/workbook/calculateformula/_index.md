---
title: "Workbook.CalculateFormula"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Workbook. Calcule le résultat des formules"
type: docs
url: /fr/net/aspose.cells/workbook/calculateformula/
---
## CalculateFormula() {#calculateformula}

Calcule le résultat des formules.

```csharp
public void CalculateFormula()
```

### Remarques

Pour toutes les formules prises en charge, veuillez consulter la liste à https://docs.aspose.com/display/cellsnet/Supported+Formula+Functions

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodCalculateFormulaDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            
            // Définir des valeurs et des formules
            cells["A1"].PutValue(5);
            cells["B1"].Formula = "=A1*2";
            cells["C1"].Formula = "=B1+10";
            
            // Calculer les formules
            workbook.CalculateFormula();
            
            // Afficher les résultats
            Console.WriteLine("A1 value: " + cells["A1"].IntValue);
            Console.WriteLine("B1 formula result: " + cells["B1"].IntValue);
            Console.WriteLine("C1 formula result: " + cells["C1"].IntValue);
        }
    }
}
```

### Voir aussi

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## CalculateFormula(bool) {#calculateformula_2}

Calcule le résultat des formules.

```csharp
public void CalculateFormula(bool ignoreError)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| ignoreError | Boolean | Indique s'il faut masquer l'erreur lors du calcul des formules. L'erreur peut être une fonction non prise en charge, des liens externes, etc. |

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodCalculateFormulaWithBooleanDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook wb = new Workbook();
            
            // Accéder à la première feuille de calcul et à ses cellules
            Worksheet worksheet = wb.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Placer des valeurs dans la première ligne (A1:E1)
            for (int i = 0; i < 5; i++)
            {
                cells[0, i].PutValue(i + 1); // Values 1-5
            }

            // Placer des valeurs dans la deuxième ligne (A2:E2)
            for (int i = 0; i < 5; i++)
            {
                cells[1, i].PutValue((i + 1) * 10); // Values 10,20,30,40,50
            }

            // Définir une formule HLOOKUP partagée dans la quatrième ligne (A4:E4)
            cells[3, 0].SetSharedFormula("=HLOOKUP(A1,$A$1:$E$2,2,FALSE)", 1, 5);

            // Calculer les formules sans calcul récursif
            wb.CalculateFormula(false);

            // Affichez les résultats
            Console.WriteLine("Formula calculation results:");
            for (int i = 0; i < 5; i++)
            {
                Console.WriteLine($"Cell {((char)('A' + i))}4 value: {cells[3, i].StringValue}");
            }
        }
    }
}
```

### Voir aussi

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## CalculateFormula(CalculationOptions) {#calculateformula_1}

Calcul des formules dans ce classeur.

```csharp
public void CalculateFormula(CalculationOptions options)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| options | CalculationOptions | Options de calcul |

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodCalculateFormulaWithCalculationOptionsDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            
            // Créer un tableau et définir les noms de colonnes
            sheet.Cells["A1"].PutValue("A");
            sheet.Cells["B1"].PutValue("B");
            sheet.Cells["A2"].PutValue(1);
            sheet.Cells["B2"].PutValue(2);
            
            // Définir les formules et calculer
            Cells cells = sheet.Cells;
            cells["C1"].PutValue("InvalidColumn");
            cells["D1"].Formula = "=INDIRECT(\"A\"&ROW())";
            cells["E1"].Formula = "=IFERROR(INDIRECT(\"B\"&ROW()),\"OK\")";
            
            // Calculer les formules avec des options
            wb.CalculateFormula(new CalculationOptions());
            
            // Afficher les résultats
            Console.WriteLine("D1 result: " + cells["D1"].StringValue);
            Console.WriteLine("E1 result: " + cells["E1"].StringValue);
        }
    }
}
```

### Voir aussi

* class [CalculationOptions](../../calculationoptions/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


