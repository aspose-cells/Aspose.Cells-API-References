---
title: "WorkbookDesigner.UpdateEmptyStringAsNull"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété WorkbookDesigner. Si TRUE, Null sera inséré si la valeur est"
type: docs
url: /fr/net/aspose.cells/workbookdesigner/updateemptystringasnull/
---
## WorkbookDesigner.UpdateEmptyStringAsNull property

Si VRAI, Null sera inséré si la valeur est "";

```csharp
public bool UpdateEmptyStringAsNull { get; set; }
```

### Exemples

```csharp
using System;
using System.Data;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookDesignerPropertyUpdateEmptyStringAsNullDemo
    {
        public static void Run()
        {
            // Créer un DataSet d'exemple avec des chaînes vides
            DataSet ds = new DataSet();
            DataTable dt = new DataTable("Products");
            dt.Columns.Add("Name");
            dt.Columns.Add("Price");
            dt.Rows.Add("Laptop", "");
            dt.Rows.Add("", "999.99");
            ds.Tables.Add(dt);

            // Créer un classeur avec des marqueurs de concepteur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("&=$Products.Name");
            worksheet.Cells["B1"].PutValue("&=$Products.Price");

            // Initialiser WorkbookDesigner et définir les propriétés
            WorkbookDesigner designer = new WorkbookDesigner();
            designer.Workbook = workbook;
            designer.UpdateEmptyStringAsNull = true; // This is the key property being demonstrated
            
            // Définir la source de données et traiter
            designer.SetDataSource(ds.Tables["Products"]);
            designer.Process();

            // Vérifier les résultats
            Console.WriteLine("A1 value: " + worksheet.Cells["A1"].StringValue); // Should show "Laptop"
            Console.WriteLine("B1 value: " + worksheet.Cells["B1"].StringValue); // Should show empty (null)
        }
    }
}
```

### Voir aussi

* class [WorkbookDesigner](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


