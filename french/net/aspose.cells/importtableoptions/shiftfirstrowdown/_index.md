---
title: "ImportTableOptions.ShiftFirstRowDown"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ImportTableOptions. Indique si le décalage de la première ligne vers le bas est effectué lors de l'insertion de lignes"
type: docs
url: /fr/net/aspose.cells/importtableoptions/shiftfirstrowdown/
---
## ImportTableOptions.ShiftFirstRowDown property

Indique si la première ligne doit être décalée vers le bas lors de l'insertion de lignes.

```csharp
public bool ShiftFirstRowDown { get; set; }
```

### Exemples

```csharp
using System;
using System.Data;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ImportTableOptionsPropertyShiftFirstRowDownDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;

            // Créer un DataTable d’exemple
            DataTable table = new DataTable();
            table.Columns.Add("Column1");
            table.Columns.Add("Column2");
            table.Rows.Add("Header1", "Header2");
            table.Rows.Add("Data1", "Data2");
            table.Rows.Add("Data3", "Data4");

            // Importer avec ShiftFirstRowDown = false (comportement par défaut)
            var options1 = new ImportTableOptions
            {
                IsFieldNameShown = false,
                ShiftFirstRowDown = false
            };
            cells.ImportData(table, 0, 0, options1);
            Console.WriteLine("With ShiftFirstRowDown=false, first row starts at A1: " + cells[0, 0].StringValue);

            // Effacer la feuille de calcul et importer avec ShiftFirstRowDown = true
            workbook.Worksheets[0].Cells.Clear();
            var options2 = new ImportTableOptions
            {
                IsFieldNameShown = false,
                ShiftFirstRowDown = true
            };
            cells.ImportData(table, 0, 0, options2);
            Console.WriteLine("With ShiftFirstRowDown=true, first row is shifted down to A2: " + cells[1, 0].StringValue);

            // Enregistrez le classeur
            workbook.Save("ShiftFirstRowDownDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [ImportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


