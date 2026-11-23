---
title: "LightCellsDataHandler.ProcessRow"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode LightCellsDataHandler. Commence à traiter une ligne"
type: docs
url: /fr/net/aspose.cells/lightcellsdatahandler/processrow/
---
## LightCellsDataHandler.ProcessRow method

Commence à traiter une ligne.

```csharp
public bool ProcessRow(Row row)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| ligne | Row | Objet Row qui est actuellement traité. |

### Valeur de retour

indique si les cellules de cette ligne doivent être traitées. false pour ignorer toutes les cellules de cette ligne.

### Remarques

Elle sera appelée après que les propriétés de la ligne telles que la hauteur, le style, ...etc. aient été lues. Cependant, les cellules de cette ligne n'ont pas encore été lues.

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class LightCellsDataHandlerMethodProcessRowWithRowDemo
    {
        public static void Run()
        {
            try
            {
                // Créer un nouveau classeur
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];

                // Ajoutez des données d'exemple
                worksheet.Cells["A1"].Value = "Test Data";
                worksheet.Cells["A2"].Value = 100;
                worksheet.Cells["B2"].Value = 200;

                // Créer un gestionnaire personnalisé
                var handler = new CustomRowHandler();

                // Traiter la première ligne
                Row firstRow = worksheet.Cells.Rows[0];
                bool result = handler.ProcessRow(firstRow);

                Console.WriteLine($"ProcessRow returned: {result}");
                Console.WriteLine($"Row height after processing: {firstRow.Height}");

                workbook.Save("ProcessRowDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error in ProcessRow demo: {ex.Message}");
            }
        }

        private class CustomRowHandler : LightCellsDataHandler
        {
            public bool ProcessRow(Row row)
            {
                // Démontrer l'accès aux propriétés de la ligne
                Console.WriteLine($"Processing row index: {row.Index}");
                Console.WriteLine($"Row is hidden: {row.IsHidden}");
                Console.WriteLine($"Row is blank: {row.IsBlank}");

                // Modifier la hauteur de la ligne si ce n'est pas la ligne d'en-tête
                if (row.Index > 0)
                {
                    row.Height = 25.0;
                }

                return true;
            }

            public bool StartSheet(Worksheet sheet) => true;
            public bool StartRow(int rowIndex) => true;
            public bool StartCell(int columnIndex) => true;
            public bool ProcessCell(Cell cell) => true;
        }
    }
}
```

### Voir aussi

* class [Row](../../row/)
* interface [LightCellsDataHandler](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


