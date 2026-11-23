---
title: "WorkbookDesigner.Process"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "WorkbookDesigner méthode. Traite les marqueurs intelligents et remplit les valeurs de la source de données"
type: docs
url: /fr/net/aspose.cells/workbookdesigner/process/
---
## Process(Range, bool) {#process_1}

Traite les smart markers et remplit les valeurs de la source de données.

```csharp
[Obsolete("Use Range smart markers instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public void Process(Range range, bool isPreserved)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| plage | Plage | La plage à traiter |
| isPreserved | Boolean | Vrai si le marqueur intelligent non reconnu est préservé. |

### Remarques

NOTE: Cette classe est maintenant obsolète. À la place, veuillez utiliser les marqueurs intelligents de plage. Cette propriété sera supprimée 12 mois plus tard depuis juillet 2025. Aspose s'excuse pour tout inconvénient que vous avez pu rencontrer.

### Exemples

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookDesignerMethodProcessWithRangeBooleanDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook wb = new Workbook();
            
            // Accéder à la première feuille de calcul
            Worksheet sheet = wb.Worksheets[0];
            
            // Créez des données d'exemple dans les cellules
            sheet.Cells["A1"].PutValue("Name");
            sheet.Cells["B1"].PutValue("Value");
            sheet.Cells["A2"].PutValue("&=$Name");
            sheet.Cells["B2"].PutValue("&=$Value");
            
            // Créer un concepteur de classeur
            WorkbookDesigner designer = new WorkbookDesigner();
            designer.Workbook = wb;
            
            // Créer une source de données JSON
            string jsonData = "{'Name':'Test Product','Value':100.50}";
            designer.SetJsonDataSource("Data", jsonData);
            
            // Traiter une plage spécifique avec des marqueurs intelligents
            Aspose.Cells.Range range = sheet.Cells.CreateRange("A2:B2");
            range.Name = "_CellsSmartMarkers";
            
            // Traiter la plage (true = ne traiter que cette plage)
            designer.Process(range, true);
            
            // Enregistrer le résultat
            wb.Save("output.xlsx");
        }
    }
}
```

### Voir aussi

* class [Range](../../range/)
* class [WorkbookDesigner](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Process() {#process}

Traite les smart markers et remplit les valeurs de la source de données.

```csharp
public void Process()
```

### Exemples

```csharp
using System;
using System.Collections;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookDesignerMethodProcessDemo
    {
        public static void Run()
        {
            // Créer un classeur à partir d'un fichier modèle
            Workbook workbook = new Workbook("example.xlsx");
            WorkbookDesigner designer = new WorkbookDesigner(workbook);

            // Préparer la source de données
            ArrayList persons = new ArrayList();
            
            Person person1 = new Person("John Doe", 30);
            person1.FOTO = File.ReadAllBytes("1.jpg");
            persons.Add(person1);

            Person person2 = new Person("Jane Smith", 28);
            person2.FOTO = File.ReadAllBytes("1.jpg");
            persons.Add(person2);

            // Définir la source de données et traiter
            designer.SetDataSource("Datos", persons);
            designer.Process();

            // Enregistrer le résultat
            workbook.Save("output.xlsx");
        }
    }

    public class Person
    {
        public string Name { get; set; }
        public int Age { get; set; }
        public byte[] FOTO { get; set; }

        public Person(string name, int age)
        {
            Name = name;
            Age = age;
        }
    }
}
```

### Voir aussi

* class [WorkbookDesigner](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Process(bool) {#process_2}

Traite les smart markers et remplit les valeurs de la source de données.

```csharp
public void Process(bool isPreserved)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| isPreserved | Boolean | Vrai si le marqueur intelligent non reconnu est préservé. |

### Exemples

```csharp
using System;
using System.Collections.Generic;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookDesignerMethodProcessWithBooleanDemo
    {
        public static void Run()
        {
            // Initialiser le classeur et charger le modèle
            Workbook workbook = new Workbook("example.xlsx");
            
            // Créer des données d'exemple directement au lieu de les charger depuis JSON
            ABC_1_Data data = new ABC_1_Data
            {
                Directors = new List<Director>
                {
                    new Director { DRFNAME2 = "DRFNAME2" }
                }
            };

            // Configurer les marqueurs intelligents
            workbook.Worksheets[0].Cells.CreateRange("A13:K19").Name = "_CellsSmartMarkers";

            // Préparer les sources de données
            List<ABC_1_Data> listData = new List<ABC_1_Data> { data };

            // Traiter le concepteur de classeur
            WorkbookDesigner designer = new WorkbookDesigner
            {
                Workbook = workbook,
                LineByLine = false
            };
            
            designer.SetDataSource("RootData", listData);
            designer.SetDataSource("Directors", data.Directors);
            
            // Traiter avec un paramètre booléen
            designer.Process(true);
            
            // Enregistrer le résultat
            workbook.Save("output.xlsx");
        }
    }

    // Classes de données d'exemple
    public class ABC_1_Data
    {
        public List<Director> Directors { get; set; }
    }

    public class Director
    {
        public string DRFNAME2 { get; set; }
    }
}
```

### Voir aussi

* class [WorkbookDesigner](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Process(int, bool) {#process_3}

Traite les smart markers et remplit les valeurs de la source de données.

```csharp
public void Process(int sheetIndex, bool isPreserved)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| sheetIndex | Int32 | Index de la feuille de calcul. |
| isPreserved | Boolean | Vrai si le marqueur intelligent non reconnu est préservé. |

### Remarques

Cette méthode fonctionne au niveau de la feuille de calcul.

### Exemples

```csharp
using System;
using System.Data;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookDesignerMethodProcessWithInt32BooleanDemo
    {
        public static void Run()
        {
            // Créer un classeur à partir du fichier source
            Workbook workbook = new Workbook("example.xlsx");
            
            // Exporter les données de la feuille de calcul vers le DataTable
            Worksheet worksheet = workbook.Worksheets["Data"];
            DataTable dataTable = worksheet.Cells.ExportDataTable(
                0, 0, 
                worksheet.Cells.MaxDataRow, 
                worksheet.Cells.MaxDataColumn + 1, 
                new ExportTableOptions { 
                    CheckMixedValueType = true, 
                    ExportColumnName = true 
                });
            dataTable.TableName = "Table";

            // Créer le concepteur de classeur et définir la source de données
            WorkbookDesigner designer = new WorkbookDesigner();
            designer.Workbook = workbook;
            designer.SetDataSource(dataTable);

            // Traiter le concepteur avec les paramètres (Int32, Boolean)
            designer.Process(0, true);

            // Enregistrer le résultat
            workbook.Save("output.xlsx");
        }
    }
}
```

### Voir aussi

* class [WorkbookDesigner](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


