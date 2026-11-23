---
title: "Cells.MinDataRow"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Cells. Indice de ligne minimum de la cellule qui contient des données"
type: docs
url: /fr/net/aspose.cells/cells/mindatarow/
---
## Cells.MinDataRow property

Indice de ligne minimal de la cellule contenant des données.

```csharp
public int MinDataRow { get; }
```

### Remarques

Renvoie -1 s'il n'y a aucune cellule contenant des données. Cette propriété doit itérer et vérifier les cellules et les lignes dynamiquement, ce qui consomme du temps et ne doit pas être invoquée de façon répétée, par exemple en l'utilisant directement comme condition dans une boucle.

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsPropertyMinDataRowDemo
    {
        public static void Run()
        {
            // Créer un classeur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Remplissez quelques données
            sheet.Cells[0, 0].Value = "Header1";
            sheet.Cells[0, 1].Value = "Header2";
            sheet.Cells[1, 0].Value = "Data1";
            sheet.Cells[1, 1].Value = "Data2";
            sheet.Cells[2, 0].Value = "Data3";
            sheet.Cells[2, 1].Value = "Data4";

            // Démontrer l'utilisation de MinDataRow
            Console.WriteLine("Minimum data row index: " + sheet.Cells.MinDataRow);
            Console.WriteLine("Maximum data row index: " + sheet.Cells.MaxDataRow);

            // Enregistrez le classeur
            workbook.Save("MinDataRowExample.xlsx");
        }
    }
}
```

### Voir aussi

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


