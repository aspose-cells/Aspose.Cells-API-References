---
title: "WorkbookDesigner.WorkbookDesigner"
second_title: "Aspose.Cells för .NET API‑referens"
description: "WorkbookDesigner-konstruktor. Initierar en ny instans av WorkbookDesigner-klassen"
type: docs
url: /sv/net/aspose.cells/workbookdesigner/workbookdesigner/
---
## WorkbookDesigner() {#constructor}

Initierar en ny instans av [`WorkbookDesigner`](../)-klassen.

```csharp
public WorkbookDesigner()
```

### Exempel

```csharp
using System;
using System.Collections.Generic;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookDesignerMethodCtorDemo
    {
        public static void Run()
        {
            // Skapa en ny WorkbookDesigner med hjälp av konstruktorn
            WorkbookDesigner designer = new WorkbookDesigner();
            
            // Skapa en exempel-datakälla
            List<Level> levels = new List<Level>();
            levels.Add(new Level("r1", "c1"));
            levels.Add(new Level("r2", "c2"));
            levels.Add(new Level("r3", "c3"));

            // Skapa en ny arbetsbok och sätt den som designerns arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ange markörer i kalkylbladet
            worksheet.Cells["A1"].PutValue("&Level.Name");
            worksheet.Cells["B1"].PutValue("&Level.Value");

            // Ange arbetsboken till designern
            designer.Workbook = workbook;

            // Ange datakälla och bearbeta
            designer.SetDataSource("Level", levels);
            designer.Process();

            // Spara resultatet
            workbook.Save("output.xlsx", SaveFormat.Xlsx);
        }
    }

    public class Level
    {
        public string Name { get; set; }
        public string Value { get; set; }

        public Level(string name, string value)
        {
            Name = name;
            Value = value;
        }
    }
}
```

### Se även

* class [WorkbookDesigner](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## WorkbookDesigner(Workbook) {#constructor_1}

Initierar en ny instans av [`WorkbookDesigner`](../)-klassen.

```csharp
public WorkbookDesigner(Workbook workbook)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| arbetsbok | Arbetsbok | Mallarbetsboksfilen. |

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookDesignerMethodCtorWithWorkbookDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Åtkomst till det första kalkylbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ange exempeldata i celler
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["A2"].PutValue("&=$ds.object.object1.name");
            
            // Skapa JSON-datakälla
            string jsonData = "{\"object\": {\"object1\": {\"name\": \"John Doe\"}}}";
            
            // Initiera WorkbookDesigner med arbetsboken
            WorkbookDesigner designer = new WorkbookDesigner(workbook);
            
            // Ange JSON-datakälla
            designer.SetJsonDataSource("ds", jsonData);
            
            // Bearbeta designern
            designer.Process();
            
            // Skriv ut resultatet
            Console.WriteLine("Processed value: " + worksheet.Cells["A2"].StringValue);
        }
    }
}
```

### Se även

* class [Workbook](../../workbook/)
* class [WorkbookDesigner](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


