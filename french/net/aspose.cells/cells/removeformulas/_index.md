---
title: "Cells.RemoveFormulas"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Cells. Supprime toutes les formules et les remplace par la valeur de la formule"
type: docs
url: /fr/net/aspose.cells/cells/removeformulas/
---
## Cells.RemoveFormulas method

Supprime toutes les formules et les remplace par la valeur de la formule.

```csharp
public void RemoveFormulas()
```

### Exemples

```csharp
using System;
using System.Data;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodRemoveFormulasDemo
    {
        public static void Run()
        {
            // Créer un jeu de données d'exemple
            DataSet ds = new DataSet();

            // Créer et remplir la table Master
            DataTable dtMaster = new DataTable("Master");
            dtMaster.Columns.Add("ACCOUNT", typeof(string));
            dtMaster.Columns.Add("ACCOUNT_CREATEDBY_NAME", typeof(string));
            dtMaster.Rows.Add("Test_Account", "Test_user");
            ds.Tables.Add(dtMaster);

            // Créer et remplir la table OppLineItems
            DataTable lineItems = new DataTable("OppLineItems");
            lineItems.Columns.Add("Id", typeof(int));
            lineItems.Columns.Add("Name", typeof(string));
            lineItems.Columns.Add("SALESPRICE", typeof(int));
            lineItems.Rows.Add(1, "lineItem1", 10);
            lineItems.Rows.Add(2, "lineItem2", 20);
            ds.Tables.Add(lineItems);

            // Créer un nouveau classeur
            Workbook wkb = new Workbook();
            
            // Utiliser WorkbookDesigner pour lier les données
            WorkbookDesigner designer = new WorkbookDesigner { Workbook = wkb };
            designer.SetDataSource(ds);
            designer.Process(false);

            // Ajouter une formule pour démontrer la suppression
            wkb.Worksheets[0].Cells["A10"].Formula = "=SUM(C2:C3)";
            
            // Calculer les formules d'abord
            wkb.CalculateFormula();

            // Supprimer toutes les formules de la feuille de calcul
            wkb.Worksheets[0].Cells.RemoveFormulas();

            // Enregistrez le classeur
            wkb.Save("output.xlsx");
            
            Console.WriteLine("Formulas removed and workbook saved successfully.");
        }
    }
}
```

### Voir aussi

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


