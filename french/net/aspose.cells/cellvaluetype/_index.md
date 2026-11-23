---
title: "Enum CellValueType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Enum Aspose.Cells.CellValueType. Spécifie un type de valeur de cellule"
type: docs
url: /fr/net/aspose.cells/cellvaluetype/
---
## CellValueType enumeration

Spécifie un type de valeur de cellule.

```csharp
public enum CellValueType
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| IsUnknown | `0` | Le type de valeur de la cellule est inconnu. |
| IsNull | `1` | Cellule vide. La valeur correspondante doit être null. |
| IsNumeric | `2` | La valeur de la cellule est numérique. La valeur correspondante doit être int ou double. |
| IsDateTime | `4` | La valeur de la cellule est une date/heure. La valeur correspondante doit être DateTime. |
| IsString | `8` | La valeur de la cellule est une chaîne. La valeur correspondante doit être string. |
| IsBool | `16` | La valeur de la cellule est booléenne. La valeur correspondante doit être bool. |
| IsError | `32` | La cellule contient une valeur d'erreur. La valeur correspondante doit être une chaîne d'erreur. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellValueTypeDemo
    {
        public static void CellValueTypeExample()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter des données d'exemple à la feuille de calcul
            worksheet.Cells["A1"].PutValue(123); // Numeric value
            worksheet.Cells["A2"].PutValue("Hello World"); // String value
            worksheet.Cells["A3"].PutValue(DateTime.Now); // DateTime value
            worksheet.Cells["A4"].PutValue(true); // Boolean value
            worksheet.Cells["A5"].PutValue(null); // Null value

            // Vérifier et afficher les types de valeur des cellules
            DisplayCellValueType(worksheet.Cells["A1"]);
            DisplayCellValueType(worksheet.Cells["A2"]);
            DisplayCellValueType(worksheet.Cells["A3"]);
            DisplayCellValueType(worksheet.Cells["A4"]);
            DisplayCellValueType(worksheet.Cells["A5"]);

            // Enregistrez le classeur
            workbook.Save("CellValueTypeExample.xlsx");
            workbook.Save("CellValueTypeExample.pdf");
        }

        private static void DisplayCellValueType(Cell cell)
        {
            Console.WriteLine($"Cell {cell.Name} has value: {cell.Value} and type: {cell.Type}");

            switch (cell.Type)
            {
                case CellValueType.IsNumeric:
                    Console.WriteLine("The cell contains a numeric value.");
                    break;
                case CellValueType.IsString:
                    Console.WriteLine("The cell contains a string value.");
                    break;
                case CellValueType.IsDateTime:
                    Console.WriteLine("The cell contains a DateTime value.");
                    break;
                case CellValueType.IsBool:
                    Console.WriteLine("The cell contains a boolean value.");
                    break;
                case CellValueType.IsNull:
                    Console.WriteLine("The cell is blank.");
                    break;
                case CellValueType.IsError:
                    Console.WriteLine("The cell contains an error value.");
                    break;
                default:
                    Console.WriteLine("The cell value type is unknown.");
                    break;
            }
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


