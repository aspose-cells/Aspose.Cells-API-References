---
title: "Interface ISmartMarkerCallBack"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Interface Aspose.Cells.ISmartMarkerCallBack. Représente l'interface de rappel du traitement du smartmarker"
type: docs
url: /fr/net/aspose.cells/ismartmarkercallback/
---
## ISmartMarkerCallBack interface

Représente l'interface de rappel du traitement du smartmarker.

```csharp
public interface ISmartMarkerCallBack
```

## Méthodes

| Nom | Description |
| --- | --- |
| [Process](../../aspose.cells/ismartmarkercallback/process/)(int, int, int, string, string) | Rappel pour le traitement d'un smart marker. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ISmartMarkerCallBackDemo : ISmartMarkerCallBack
    {
        // Implémentation de la méthode Process de l'interface ISmartMarkerCallBack
        public void Process(int sheetIndex, int rowIndex, int colIndex, string tableName, string columnName)
        {
            // Exemple d'implémentation de la méthode Process
            Console.WriteLine($"Processing sheetIndex: {sheetIndex}, rowIndex: {rowIndex}, colIndex: {colIndex}, tableName: {tableName}, columnName: {columnName}");
        }

        public static void ISmartMarkerCallBackExample()
        {
            // Créez une nouvelle instance de WorkbookDesigner
            WorkbookDesigner designer = new WorkbookDesigner();
            // Ouvrez un fichier modèle (qui contient des smart markers)
            designer.Workbook = new Workbook("ISmartMarkerCallBackExample_original.xlsx");

            // Définissez l'interface de rappel
            designer.CallBack = new ISmartMarkerCallBackDemo();

            // Initialisez vos données à partir de la source de données
            // À titre de démonstration, nous utiliserons une DataTable simple
            System.Data.DataTable dataTable = new System.Data.DataTable("Table1");
            dataTable.Columns.Add("Column1", typeof(string));
            dataTable.Rows.Add("Value1");
            dataTable.Rows.Add("Value2");

            // Définissez la DataTable comme source de données
            designer.SetDataSource(dataTable);

            // Traitez les smart markers pour remplir les données dans les feuilles de calcul
            designer.Process(true);

            // Enregistrez le fichier Excel
            designer.Workbook.Save("ISmartMarkerCallBackExample.xlsx");
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


