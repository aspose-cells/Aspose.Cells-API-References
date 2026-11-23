---
title: "WorkbookDesigner.SetJsonDataSource"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode WorkbookDesigner. Définit la valeur de chaîne JSON comme source de données des marqueurs intelligents"
type: docs
url: /fr/net/aspose.cells/workbookdesigner/setjsondatasource/
---
## WorkbookDesigner.SetJsonDataSource method

Définir la valeur de chaîne JSON comme source de données des smart markers.

```csharp
public void SetJsonDataSource(string name, string json)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| name | String | Le nom du tableau. Si la valeur du JSON représente un objet, elle peut être nulle. |
| json | String | La valeur de la chaîne Json. |

### Exemples

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookDesignerMethodSetJsonDataSourceWithStringStringDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajoutez un marqueur d'exemple dans la cellule A1
            worksheet.Cells["A1"].PutValue("&=$DataSource.Name");
            
            // Créer un concepteur de classeur
            WorkbookDesigner designer = new WorkbookDesigner();
            designer.Workbook = workbook;
            
            // Exemple de données JSON
            string jsonData = "{\"Name\":\"John Doe\",\"Age\":30,\"City\":\"New York\"}";
            
            // Définissez la source de données JSON
            designer.SetJsonDataSource("DataSource", jsonData);
            
            // Traitez les marqueurs
            designer.Process();
            
            // Enregistrez le classeur
            workbook.Save("output.xlsx");
        }
    }
}
```

### Voir aussi

* class [WorkbookDesigner](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


