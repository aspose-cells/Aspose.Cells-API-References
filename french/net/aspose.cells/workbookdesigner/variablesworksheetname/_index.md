---
title: "WorkbookDesigner.VariablesWorksheetName"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété WorkbookDesigner. Obtient et définit le nom de la feuille de calcul qui contient le marqueur intelligent de variables"
type: docs
url: /fr/net/aspose.cells/workbookdesigner/variablesworksheetname/
---
## WorkbookDesigner.VariablesWorksheetName property

Obtient et définit le nom de la feuille de calcul qui contient les variables smart marker.

```csharp
public string VariablesWorksheetName { get; set; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class WorkbookDesignerPropertyVariablesWorksheetNameDemo
    {
        public static void Run()
        {
            try
            {
                // Créer un nouveau classeur
                Workbook workbook = new Workbook();

                // Ajoutez une feuille de calcul nommée "Variables" pour démontrer la propriété
                Worksheet variablesSheet = workbook.Worksheets.Add("Variables");
                variablesSheet.Cells["A1"].PutValue("Variable1");
                variablesSheet.Cells["B1"].PutValue("Value1");

                // Créer une instance de WorkbookDesigner
                WorkbookDesigner designer = new WorkbookDesigner(workbook);

                // Affichez la valeur actuelle de VariablesWorksheetName
                Console.WriteLine("Initial VariablesWorksheetName: " + designer.VariablesWorksheetName);

                // Définissez une nouvelle valeur pour VariablesWorksheetName
                designer.VariablesWorksheetName = "Variables";
                Console.WriteLine("Updated VariablesWorksheetName: " + designer.VariablesWorksheetName);

                // Ajoutez une autre feuille de calcul avec des marqueurs intelligents
                Worksheet templateSheet = workbook.Worksheets.Add("Template");
                templateSheet.Cells["A1"].PutValue("&=$Variable1");

                // Traitez les marqueurs intelligents
                designer.Process();

                // Enregistrez le classeur
                workbook.Save("VariablesWorksheetNameDemo.xlsx");
                Console.WriteLine("Workbook saved successfully with VariablesWorksheetName set.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Voir aussi

* class [WorkbookDesigner](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


