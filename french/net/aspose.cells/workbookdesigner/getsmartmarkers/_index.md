---
title: "WorkbookDesigner.GetSmartMarkers"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode WorkbookDesigner. Retourne une collection de smart markers dans une feuille de calcul"
type: docs
url: /fr/net/aspose.cells/workbookdesigner/getsmartmarkers/
---
## WorkbookDesigner.GetSmartMarkers method

Renvoie une collection de smart markers dans une feuille de calcul.

```csharp
public string[] GetSmartMarkers()
```

### Valeur de retour

Une collection de smart markers

### Remarques

Un tableau de chaînes est créé à chaque appel. Le tableau est trié et les valeurs dupliquées sont supprimées.

### Exemples

```csharp
using System;
using System.Data;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookDesignerMethodGetSmartMarkersDemo
    {
        public static void Run()
        {
            // Créer un fichier de modèle d'exemple en mémoire
            Workbook templateWorkbook = new Workbook();
            Cells cells = templateWorkbook.Worksheets[0].Cells;
            
            // Ajouter des smart markers au modèle
            cells["A1"].PutValue("&=COLORS_TIMES.COLORS");
            cells["B1"].PutValue("&=COLORS_TIMES.TIMES");
            
            // Enregistrer le modèle dans le flux mémoire
            MemoryStream templateStream = new MemoryStream();
            templateWorkbook.Save(templateStream, SaveFormat.Xlsx);
            
            // Initialiser WorkbookDesigner avec le modèle
            WorkbookDesigner designer = new WorkbookDesigner();
            designer.Workbook = new Workbook(templateStream);
            
            // Obtenir et afficher les marqueurs intelligents
            string[] smartMarkers = designer.GetSmartMarkers();
            Console.WriteLine("Found smart markers:");
            foreach (string marker in smartMarkers)
            {
                Console.WriteLine(marker);
            }
            
            // Préparer la source de données
            DataTable data = new DataTable("COLORS_TIMES");
            data.Columns.Add("COLORS", typeof(string));
            data.Columns.Add("TIMES", typeof(DateTime));
            data.Rows.Add("red", DateTime.Now.AddDays(-1));
            data.Rows.Add("yellow", DateTime.Now);
            data.Rows.Add("green", DateTime.Now.AddDays(1));
            
            // Définir la source de données et traiter
            designer.SetDataSource(data);
            designer.Process();
            
            // Enregistrer le résultat
            designer.Workbook.Save("output.xlsx");
        }
    }
}
```

### Voir aussi

* class [WorkbookDesigner](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


