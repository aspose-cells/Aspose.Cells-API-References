---
title: "Klasse DataModel"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.DataModels.DataModel class. Stellt das Datenmodell dar"
type: docs
url: /de/net/aspose.cells.datamodels/datamodel/
---
## DataModel class

Stellt das Datenmodell dar.

```csharp
public class DataModel
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [Relationships](../../aspose.cells.datamodels/datamodel/relationships/) { get; } | Liefert alle Beziehungen der Tabellen im Datenmodell. |
| [Tables](../../aspose.cells.datamodels/datamodel/tables/) { get; } | Ermittelt alle Tabellen im Datenmodell. |

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Holen Sie das DataModel aus der Arbeitsmappe, anstatt eine neue Instanz zu erstellen
            DataModel dataModel = workbook.DataModel;

            // Demonstrieren Sie den Zugriff auf Tabellen und Beziehungen (schreibgeschützte Eigenschaften)
            Console.WriteLine("Number of tables in DataModel: " + dataModel.Tables.Count);
            Console.WriteLine("Number of relationships in DataModel: " + dataModel.Relationships.Count);

            // Hinweis: Da Tabellen und Beziehungen schreibgeschützte Sammlungen sind,
            // können wir nur auf vorhandene Elemente zugreifen, sie jedoch nicht direkt ändern

            // Speichern Sie die Arbeitsmappe (DataModel wird typischerweise intern von Aspose.Cells verwendet)
            workbook.Save("DataModelDemo.xlsx");
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells.DataModels](../../aspose.cells.datamodels/)
* assembly [Aspose.Cells](../../)


