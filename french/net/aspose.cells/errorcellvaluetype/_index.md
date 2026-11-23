---
title: "Énumération ErrorCellValueType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Énumération Aspose.Cells.ErrorCellValueType. Représente une valeur de cellule contenant une erreur"
type: docs
url: /fr/net/aspose.cells/errorcellvaluetype/
---
## ErrorCellValueType enumeration

Représente une valeur de cellule contenant une erreur.

```csharp
public enum ErrorCellValueType
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| Value | `1` | Représente la valeur d'une cellule contenant une erreur #VALUE!. |
| Ref | `3` | Représente la valeur d'une cellule contenant une erreur #REF!. |
| Name | `4` | Représente la valeur d'une cellule contenant une erreur #NAME?. |
| NA | `6` | Représente la valeur d'une cellule contenant une erreur #N/A. |
| Blocked | `10` | Représente la valeur d'une cellule contenant une erreur #BLOCKED!. |
| Busy | `14` | Représente la valeur d'une cellule contenant une erreur #BUSY!. |
| Calc | `13` | Représente la valeur d'une cellule contenant une erreur #CALC!. |
| Connect | `9` | Représente la valeur d'une cellule contenant une erreur #CONNECT!. |
| Field | `12` | Représente la valeur d'une cellule contenant une erreur #FIELD!. |
| Spill | `8` | Représente la valeur d'une cellule contenant une erreur #SPILL!. |
| Unknown | `11` | Représente la valeur d'une cellule contenant une erreur #UNKNOWN!. |
| TimeOut | `19` | Représente la valeur d'une cellule contenant une erreur #TIMEOUT!. |
| External | `18` | Représente la valeur d'une cellule contenant une erreur #EXTERNAL!. |

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassErrorCellValueTypeDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Définissez une formule qui entraînera une erreur de débordement
            worksheet.Cells["A1"].Formula = "=UNIQUE({1,2,3;1,2,3})";
            
            try
            {
                // Calculez des formules pour déclencher l'erreur
                workbook.CalculateFormula();
            }
            catch (Exception)
            {
                // Erreur de débordement attendue
            }
            
            // Obtenez la valeur enrichie de la cellule.
            CellRichValue richValue = worksheet.Cells["A1"].GetRichValue();
            
            // Vérifiez le type d'erreur
            if (richValue.ErrorValue == ErrorCellValueType.Spill)
            {
                Console.WriteLine("Cell contains a spill error as expected");
            }
            
            // Enregistrez le classeur
            workbook.Save("ErrorCellValueTypeDemo.xlsx");
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


