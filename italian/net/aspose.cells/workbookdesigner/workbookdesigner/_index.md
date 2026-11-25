---
title: "WorkbookDesigner.WorkbookDesigner"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Costruttore di WorkbookDesigner. Inizializza una nuova istanza della classe WorkbookDesigner"
type: docs
url: /it/net/aspose.cells/workbookdesigner/workbookdesigner/
---
## WorkbookDesigner() {#constructor}

Inizializza una nuova istanza della classe [`WorkbookDesigner`](../).

```csharp
public WorkbookDesigner()
```

### Esempi

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
            // Crea un nuovo WorkbookDesigner usando il costruttore
            WorkbookDesigner designer = new WorkbookDesigner();
            
            // Crea una fonte di dati di esempio
            List<Level> levels = new List<Level>();
            levels.Add(new Level("r1", "c1"));
            levels.Add(new Level("r2", "c2"));
            levels.Add(new Level("r3", "c3"));

            // Crea un nuovo workbook e impostalo come workbook del designer
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Imposta i marcatori nel foglio di lavoro
            worksheet.Cells["A1"].PutValue("&Level.Name");
            worksheet.Cells["B1"].PutValue("&Level.Value");

            // Imposta il workbook al designer
            designer.Workbook = workbook;

            // Imposta la fonte dati ed elabora
            designer.SetDataSource("Level", levels);
            designer.Process();

            // Salva il risultato
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

### Vedi anche

* class [WorkbookDesigner](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## WorkbookDesigner(Workbook) {#constructor_1}

Inizializza una nuova istanza della classe [`WorkbookDesigner`](../).

```csharp
public WorkbookDesigner(Workbook workbook)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| cartella di lavoro | Cartella di lavoro | Il file workbook modello. |

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookDesignerMethodCtorWithWorkbookDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Imposta dati di esempio nelle celle
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["A2"].PutValue("&=$ds.object.object1.name");
            
            // Crea origine dati JSON
            string jsonData = "{\"object\": {\"object1\": {\"name\": \"John Doe\"}}}";
            
            // Inizializza WorkbookDesigner con il workbook
            WorkbookDesigner designer = new WorkbookDesigner(workbook);
            
            // Imposta la fonte di dati JSON
            designer.SetJsonDataSource("ds", jsonData);
            
            // Elabora il designer
            designer.Process();
            
            // Restituisci il risultato
            Console.WriteLine("Processed value: " + worksheet.Cells["A2"].StringValue);
        }
    }
}
```

### Vedi anche

* class [Workbook](../../workbook/)
* class [WorkbookDesigner](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


