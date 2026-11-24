---
title: "Klasse CellsDataTableFactory"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.CellsDataTableFactory Klasse. Dienstprogramm zum Erstellen von ICellsDataTable aus benutzerdefinierten Objekten für die Benutzerfreundlichkeit"
type: docs
url: /de/net/aspose.cells/cellsdatatablefactory/
---
## CellsDataTableFactory class

Hilfsprogramm zum Erstellen von ICellsDataTable aus benutzerdefinierten Objekten für die Bequemlichkeit des Benutzers.

```csharp
public class CellsDataTableFactory
```

## Methoden

| Name | Beschreibung |
| --- | --- |
| [GetInstance](../../aspose.cells/cellsdatatablefactory/getinstance/#getinstance)(double[]) |  |
| [GetInstance](../../aspose.cells/cellsdatatablefactory/getinstance/#getinstance_6)(ICollection) | Erstellt ICellsDataTable aus der angegebenen Sammlung. |
| [GetInstance](../../aspose.cells/cellsdatatablefactory/getinstance/#getinstance_3)(int[]) |  |
| [GetInstance](../../aspose.cells/cellsdatatablefactory/getinstance/#getinstance_8)(object[]) |  |
| [GetInstance](../../aspose.cells/cellsdatatablefactory/getinstance/#getinstance_1)(double[], bool) | Erstellt ICellsDataTable aus der angegebenen Sequenz von Double-Werten. |
| [GetInstance](../../aspose.cells/cellsdatatablefactory/getinstance/#getinstance_2)(double[], string[]) | Erstellt ICellsDataTable aus der angegebenen Sequenz von Double-Werten. |
| [GetInstance](../../aspose.cells/cellsdatatablefactory/getinstance/#getinstance_7)(ICollection, bool) | Erstellt ICellsDataTable aus der angegebenen Sammlung. |
| [GetInstance](../../aspose.cells/cellsdatatablefactory/getinstance/#getinstance_4)(int[], bool) | Erstellt ICellsDataTable aus der angegebenen Sequenz von Integer-Werten. |
| [GetInstance](../../aspose.cells/cellsdatatablefactory/getinstance/#getinstance_5)(int[], string[]) | Erstellt ICellsDataTable aus der angegebenen Sequenz von Integer-Werten. |
| [GetInstance](../../aspose.cells/cellsdatatablefactory/getinstance/#getinstance_9)(object[], bool) | Erstellt ICellsDataTable aus der angegebenen Sequenz von Objekten. |
| [GetInstance](../../aspose.cells/cellsdatatablefactory/getinstance/#getinstance_10)(object[], string[]) | Erstellt ICellsDataTable aus der angegebenen Sequenz von Objekten. |
| [GetInstance](../../aspose.cells/cellsdatatablefactory/getinstance/#getinstance_11)(object[][], bool, string[]) | Erstellt ein ICellsDataTable aus einer angegebenen Sequenz von Objekten. |

### Beispiele

```csharp
using Aspose.Cells;
using System;
using System.Collections.Generic;

namespace AsposeCellsExamples
{
    public class CellsDataTableFactoryDemo
    {
        public static void RunDemo()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Fügen Sie einige Beispieldaten hinzu
            List<CustomData> dataList = new List<CustomData>
            {
                new CustomData { Id = 1, Name = "John Doe", Age = 30 },
                new CustomData { Id = 2, Name = "Jane Smith", Age = 25 },
                new CustomData { Id = 3, Name = "Sam Brown", Age = 35 }
            };

            // Hole die CellsDataTableFactory-Instanz aus der Arbeitsmappe
            CellsDataTableFactory factory = workbook.CellsDataTableFactory;

            // Erstelle eine ICellsDataTable-Instanz aus der benutzerdefinierten Datenliste
            ICellsDataTable dataTable = factory.GetInstance(dataList);

            // Importiere die Datentabelle in das Arbeitsblatt, beginnend bei Zelle A1
            sheet.Cells.ImportData(dataTable, 0, 0, new ImportTableOptions());

            // Speichere die Arbeitsmappe
            workbook.Save("CellsDataTableFactoryDemo.xlsx");
            workbook.Save("CellsDataTableFactoryDemo.pdf");
        }
    }

    // Benutzerdefinierte Datenklasse
    public class CustomData
    {
        public int Id { get; set; }
        public string Name { get; set; }
        public int Age { get; set; }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


