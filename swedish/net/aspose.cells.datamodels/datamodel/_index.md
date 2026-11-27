---
title: "Klass DataModel"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.DataModels.DataModel-klass. Representerar datamodellen"
type: docs
url: /sv/net/aspose.cells.datamodels/datamodel/
---
## DataModel class

Representerar datamodellen.

```csharp
public class DataModel
```

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [Relationships](../../aspose.cells.datamodels/datamodel/relationships/) { get; } | Hämtar alla relationer för tabellerna i datamodellen. |
| [Tables](../../aspose.cells.datamodels/datamodel/tables/) { get; } | Hämtar alla tabeller i datamodellen. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.DataModels;
    using System;

    public class DataModelsClassDataModelDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Hämta DataModel från arbetsboken istället för att skapa en ny instans
            DataModel dataModel = workbook.DataModel;

            // Demonstrera åtkomst till tabeller och relationer (skrivskyddade egenskaper)
            Console.WriteLine("Number of tables in DataModel: " + dataModel.Tables.Count);
            Console.WriteLine("Number of relationships in DataModel: " + dataModel.Relationships.Count);

            // Obs: Eftersom Tabeller och Relationer är skrivskyddade samlingar,
            // kan vi bara komma åt befintliga objekt men inte ändra dem direkt

            // Spara arbetsboken (DataModel används vanligtvis internt av Aspose.Cells)
            workbook.Save("DataModelDemo.xlsx");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells.DataModels](../../aspose.cells.datamodels/)
* assembly [Aspose.Cells](../../)


