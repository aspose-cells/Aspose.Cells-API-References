---
title: "WorkbookDesigner.WorkbookDesigner"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Constructeur WorkbookDesigner. Initialise une nouvelle instance de la classe WorkbookDesigner"
type: docs
url: /fr/net/aspose.cells/workbookdesigner/workbookdesigner/
---
## WorkbookDesigner() {#constructor}

Initialise une nouvelle instance de la classe [`WorkbookDesigner`](../).

```csharp
public WorkbookDesigner()
```

### Exemples

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
            // Créez un nouveau WorkbookDesigner en utilisant le constructeur
            WorkbookDesigner designer = new WorkbookDesigner();
            
            // Créez une source de données d'exemple
            List<Level> levels = new List<Level>();
            levels.Add(new Level("r1", "c1"));
            levels.Add(new Level("r2", "c2"));
            levels.Add(new Level("r3", "c3"));

            // Créez un nouveau classeur et définissez-le comme classeur du concepteur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Définissez les marqueurs dans la feuille de calcul
            worksheet.Cells["A1"].PutValue("&Level.Name");
            worksheet.Cells["B1"].PutValue("&Level.Value");

            // Attribuez le classeur au concepteur
            designer.Workbook = workbook;

            // Définir la source de données et traiter
            designer.SetDataSource("Level", levels);
            designer.Process();

            // Enregistrer le résultat
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

### Voir aussi

* class [WorkbookDesigner](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## WorkbookDesigner(Workbook) {#constructor_1}

Initialise une nouvelle instance de la classe [`WorkbookDesigner`](../).

```csharp
public WorkbookDesigner(Workbook workbook)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| classeur | Classeur | Le fichier de classeur modèle. |

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookDesignerMethodCtorWithWorkbookDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Définissez des données d'exemple dans les cellules
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["A2"].PutValue("&=$ds.object.object1.name");
            
            // Créer une source de données JSON
            string jsonData = "{\"object\": {\"object1\": {\"name\": \"John Doe\"}}}";
            
            // Initialisez WorkbookDesigner avec le classeur
            WorkbookDesigner designer = new WorkbookDesigner(workbook);
            
            // Définissez la source de données JSON
            designer.SetJsonDataSource("ds", jsonData);
            
            // Traiter le concepteur
            designer.Process();
            
            // Afficher le résultat
            Console.WriteLine("Processed value: " + worksheet.Cells["A2"].StringValue);
        }
    }
}
```

### Voir aussi

* class [Workbook](../../workbook/)
* class [WorkbookDesigner](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


