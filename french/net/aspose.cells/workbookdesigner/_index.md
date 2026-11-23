---
title: "Classe WorkbookDesigner"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.WorkbookDesigner. Encapsule l'objet qui représente une feuille de calcul de conception"
type: docs
url: /fr/net/aspose.cells/workbookdesigner/
---
## WorkbookDesigner class

Encapsule l'objet qui représente une feuille de calcul de conception.

```csharp
public class WorkbookDesigner
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [WorkbookDesigner](workbookdesigner/#constructor)() | Initialise une nouvelle instance de la classe `WorkbookDesigner`. |
| [WorkbookDesigner](workbookdesigner/#constructor_1)(Workbook) | Initialise une nouvelle instance de la classe `WorkbookDesigner`. |

## Propriétés

| Nom | Description |
| --- | --- |
| [CalculateFormula](../../aspose.cells/workbookdesigner/calculateformula/) { get; set; } | Indique si les formules doivent être calculées. |
| [CallBack](../../aspose.cells/workbookdesigner/callback/) { get; set; } | Obtient et définit l'interface de rappel du traitement du smartmarker. |
| [ContainsVariables](../../aspose.cells/workbookdesigner/containsvariables/) { get; set; } | (**Obsolete.**) Indique si la première feuille de calcul contient des variables personnalisées. |
| [EnableHeaderFooterMarkers](../../aspose.cells/workbookdesigner/enableheaderfootermarkers/) { get; set; } | Indique si l'en-tête/pied de page contient des smart markers et doit être traité conjointement. |
| [LineByLine](../../aspose.cells/workbookdesigner/linebyline/) { get; set; } | (**Obsolete.**) Indique si le traitement du smart marker se fait ligne par ligne. |
| [RepeatFormulasWithSubtotal](../../aspose.cells/workbookdesigner/repeatformulaswithsubtotal/) { get; set; } | Indique si les formules sont répétées avec une ligne de sous-total. |
| [SortDataSource](../../aspose.cells/workbookdesigner/sortdatasource/) { get; set; } | Indique si la source de données est triée. |
| [UpdateEmptyStringAsNull](../../aspose.cells/workbookdesigner/updateemptystringasnull/) { get; set; } | Si VRAI, Null sera inséré si la valeur est ""; |
| [UpdateReference](../../aspose.cells/workbookdesigner/updatereference/) { get; set; } | Indique si les références dans d'autres feuilles de calcul seront mises à jour. |
| [VariablesWorksheetName](../../aspose.cells/workbookdesigner/variablesworksheetname/) { get; set; } | Obtient et définit le nom de la feuille de calcul qui contient les variables smart marker. |
| [Workbook](../../aspose.cells/workbookdesigner/workbook/) { get; set; } | Obtient et définit l'objet [`Workbook`](./workbook/). |

## Méthodes

| Nom | Description |
| --- | --- |
| [ClearDataSource](../../aspose.cells/workbookdesigner/cleardatasource/)() | Efface toutes les sources de données. |
| [GetSmartMarkers](../../aspose.cells/workbookdesigner/getsmartmarkers/)() | Renvoie une collection de smart markers dans une feuille de calcul. |
| [Process](../../aspose.cells/workbookdesigner/process/#process)() | Traite les smart markers et remplit les valeurs de la source de données. |
| [Process](../../aspose.cells/workbookdesigner/process/#process_2)(bool) | Traite les smart markers et remplit les valeurs de la source de données. |
| [Process](../../aspose.cells/workbookdesigner/process/#process_3)(int, bool) | Traite les smart markers et remplit les valeurs de la source de données. |
| [Process](../../aspose.cells/workbookdesigner/process/#process_1)(Range, bool) | (**Obsolete.**) Traite les smart markers et remplit les valeurs de la source de données. |
| [SetDataSource](../../aspose.cells/workbookdesigner/setdatasource/#setdatasource)(DataSet) | Définit la source de données d'un objet DataSet. |
| [SetDataSource](../../aspose.cells/workbookdesigner/setdatasource/#setdatasource_1)(DataTable) | Définit la source de données d'un objet DataTable. |
| [SetDataSource](../../aspose.cells/workbookdesigner/setdatasource/#setdatasource_2)(DataView) | Définit la source de données d'un objet DataView. |
| [SetDataSource](../../aspose.cells/workbookdesigner/setdatasource/#setdatasource_3)(OleDbConnection) | Définit la source de données d'un objet OleDbConnection. |
| [SetDataSource](../../aspose.cells/workbookdesigner/setdatasource/#setdatasource_4)(SqlConnection) | Définit la source de données d'un objet SqlConnection. |
| [SetDataSource](../../aspose.cells/workbookdesigner/setdatasource/#setdatasource_6)(string, DataView) | Définit la source de données d'un objet DataView et l'associe à un nom de source de données. |
| [SetDataSource](../../aspose.cells/workbookdesigner/setdatasource/#setdatasource_5)(string, ICellsDataTable) | Définit la source de données d'un objet [`ICellsDataTable`](../icellsdatatable/). |
| [SetDataSource](../../aspose.cells/workbookdesigner/setdatasource/#setdatasource_8)(string, object) | Définit la liaison de données à une variable. |
| [SetDataSource](../../aspose.cells/workbookdesigner/setdatasource/#setdatasource_7)(string, IDataReader, int) | Définit la source de données d'un objet IDataReader. |
| [SetJsonDataSource](../../aspose.cells/workbookdesigner/setjsondatasource/)(string, string) | Définir la valeur de chaîne JSON comme source de données des smart markers. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Data;

    public class WorkbookDesignerDemo
    {
        public static void WorkbookDesignerExample()
        {
            // Créer l'objet WorkbookDesigner
            WorkbookDesigner wd = new WorkbookDesigner();

            // Ouvrir le fichier modèle (qui contient des smart markers)
            wd.Workbook = new Workbook("SmartMarker_Designer_original.xlsx");

            // Initialisez vos données à partir de la source de données
            DataSet ds = new DataSet();
            // Ajouter des données au dataset (c'est juste un exemple, remplacez par la source de données réelle)
            DataTable dt = new DataTable("Table1");
            dt.Columns.Add("Column1");
            dt.Columns.Add("Column2");
            dt.Rows.Add("Value1", "Value2");
            dt.Rows.Add("Value11", "Value22");
            ds.Tables.Add(dt);

            // Définir le dataset comme source de données
            wd.SetDataSource(ds);

            // Traitez les smart markers pour remplir les données dans les feuilles de calcul
            wd.Process(true);

            // Enregistrez le fichier Excel
            wd.Workbook.Save("WorkbookDesignerExample.xlsx");

            // Démonstration d'autres propriétés
            wd.RepeatFormulasWithSubtotal = true;
            wd.UpdateEmptyStringAsNull = true;
            wd.UpdateReference = true;
            wd.CalculateFormula = true;
            wd.LineByLine = true;

            // Effacer la source de données
            wd.ClearDataSource();

            // Définir la source de données en utilisant différentes méthodes
            wd.SetDataSource("dataSourceName", dt);
            wd.SetDataSource(dt);
            wd.SetDataSource(ds);
            wd.SetDataSource("dataSourceName", new DataView(dt));
            wd.SetDataSource(new DataView(dt));
            wd.SetDataSource("name", new DataTableReader(dt), dt.Rows.Count);
            wd.SetJsonDataSource("variable", "{\"key\":\"value\"}");
            wd.SetDataSource("variable", new object());

            // Traiter à nouveau les smart markers
            wd.Process();
            wd.Process(true);
            wd.Process(0, true);

            // Enregistrer à nouveau le fichier Excel
            wd.Workbook.Save("WorkbookDesignerExample_SmartMarker_Designer_Processed.xlsx");

            return;
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


