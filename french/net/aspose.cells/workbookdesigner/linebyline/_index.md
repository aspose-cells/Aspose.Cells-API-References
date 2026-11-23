---
title: "WorkbookDesigner.LineByLine"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété WorkbookDesigner. Indique si le traitement du smart marker se fait ligne par ligne"
type: docs
url: /fr/net/aspose.cells/workbookdesigner/linebyline/
---
## WorkbookDesigner.LineByLine property

Indique si le traitement du smart marker se fait ligne par ligne.

```csharp
[Obsolete("Use range smart markers instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool LineByLine { get; set; }
```

### Remarques

La valeur par défaut est true. Si False, le fichier de modèle doit contenir une plage nommée "_CellsSmartMarkers".

NOTE : Cette classe est maintenant obsolète. À la place, veuillez utiliser les smart markers de plage. Cette propriété sera supprimée 12 mois plus tard à partir de juillet 2025. Aspose s'excuse pour tout désagrément que vous avez pu rencontrer.

### Exemples

```csharp
using System;
using System.Collections.Generic;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookDesignerPropertyLineByLineDemo
    {
        public static void Run()
        {
            // Créer un classeur d'exemple avec des smart markers
            Workbook wb = new Workbook();
            Worksheet ws = wb.Worksheets[0];
            
            // Configurer les smart markers dans la feuille de calcul
            ws.Cells["A1"].PutValue("&RootData.Name");
            ws.Cells["A2"].PutValue("&RootData.Age");
            ws.Cells["A3"].PutValue("&RootData.Department");
            
            // Créer des données d'exemple
            var employee = new EmployeeData
            {
                Name = "John Doe",
                Age = 35,
                Department = "Sales"
            };
            
            List<EmployeeData> employees = new List<EmployeeData> { employee };

            // Traiter avec LineByLine défini sur false
            WorkbookDesigner designer = new WorkbookDesigner
            {
                Workbook = wb,
                LineByLine = false // This is the key property being demonstrated
            };
            
            designer.SetDataSource("RootData", employees);
            designer.Process();

            // Enregistrer le résultat
            wb.Save("output.xlsx");
            
            Console.WriteLine("Workbook processed with LineByLine=false. Output saved to output.xlsx");
        }
    }

    // Classe de données simple pour la démonstration
    public class EmployeeData
    {
        public string Name { get; set; }
        public int Age { get; set; }
        public string Department { get; set; }
    }
}
```

### Voir aussi

* class [WorkbookDesigner](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


