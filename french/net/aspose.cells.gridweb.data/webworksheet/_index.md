---
title: "Classe WebWorksheet"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Aspose.Cells.GridWeb.Data.WebWorksheet class. Représente une feuille de calcul web"
type: docs
url: /fr/net/aspose.cells.gridweb.data/webworksheet/
---
## WebWorksheet class

Représente une feuille de calcul web.

```csharp
[Obsolete("This class is obsolete; use  GridWorksheet instead")]
public class WebWorksheet : Control, ISerializable
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [WebWorksheet](webworksheet/#constructor)() | le constructeur de la WebWorksheet. |
| [WebWorksheet](webworksheet/#constructor_1)(MainWeb, GridWorksheet) | le constructeur de la WebWorksheet. |

## Propriétés

| Nom | Description |
| --- | --- |
| [BindColumns](../../aspose.cells.gridweb.data/webworksheet/bindcolumns/) { get; } | Lier la collection de colonnes. |
| [BindingSource](../../aspose.cells.gridweb.data/webworksheet/bindingsource/) { get; } | L'objet source de données réellement lié à l'exécution. Il s'agit d'un objet DataView lorsque la propriété DataSource est un objet DataSet, DataTable ou DataView. |
| [BindStartColumn](../../aspose.cells.gridweb.data/webworksheet/bindstartcolumn/) { get; set; } | En mode liaison de données, BindStartRow et BindStartColumn indiquent la position de la grille à lier à la source de données. |
| [BindStartRow](../../aspose.cells.gridweb.data/webworksheet/bindstartrow/) { get; set; } | En mode liaison de données, BindStartRow et BindStartColumn indiquent la position de la grille à lier à la source de données. |
| [CellImages](../../aspose.cells.gridweb.data/webworksheet/cellimages/) { get; } |  |
| [Cells](../../aspose.cells.gridweb.data/webworksheet/cells/) { get; } | Obtient le [`WebCells`](../webcells/). |
| [Comments](../../aspose.cells.gridweb.data/webworksheet/comments/) { get; } |  |
| [CurrentBindRows](../../aspose.cells.gridweb.data/webworksheet/currentbindrows/) { get; set; } | Obtient le nombre de lignes de liaison en mode liaison de données. |
| [DataMember](../../aspose.cells.gridweb.data/webworksheet/datamember/) { get; set; } | Obtient ou définit le DataMember à partir du DataSource multi-membres. En général, il représente un objet DataTable d'un DataSet. |
| [DataSource](../../aspose.cells.gridweb.data/webworksheet/datasource/) { get; set; } | Obtient ou définit le DataSource. En général, c'est un objet DataSet. |
| [EnableCreateBindColumnHeader](../../aspose.cells.gridweb.data/webworksheet/enablecreatebindcolumnheader/) { get; set; } | En mode liaison de données, indique s'il faut créer les légendes d'en-tête de colonne liées dans la feuille. |
| [Hyperlinks](../../aspose.cells.gridweb.data/webworksheet/hyperlinks/) { get; } | Obtient la collection HyperlinkCollection. |
| [Index](../../aspose.cells.gridweb.data/webworksheet/index/) { get; } | Obtient l'index de lui-même parmi les feuilles de calcul. |
| [IsProtected](../../aspose.cells.gridweb.data/webworksheet/isprotected/) { get; set; } | Obtient ou définit si la feuille de calcul est protégée. Lorsqu'une feuille de calcul est protégée, toutes les cellules ne peuvent pas être modifiées sauf la cellule dont la propriété IsLocked est false. |
| [Name](../../aspose.cells.gridweb.data/webworksheet/name/) { get; set; } | Obtient ou définit le nom de la feuille. |
| [RowFilter](../../aspose.cells.gridweb.data/webworksheet/rowfilter/) { get; } |  |
| [Validations](../../aspose.cells.gridweb.data/webworksheet/validations/) { get; } | Obtient la collection des paramètres de validation des données dans la feuille de calcul. |
| override [Visible](../../aspose.cells.gridweb.data/webworksheet/visible/) { get; set; } | Indique si le nom de cette feuille est affiché dans les onglets de feuille du contrôle. |

## Méthodes

| Nom | Description |
| --- | --- |
| [AutoFitColumn](../../aspose.cells.gridweb.data/webworksheet/autofitcolumn/#autofitcolumn)(int) | Ajuste automatiquement la largeur de la colonne. |
| [AutoFitColumn](../../aspose.cells.gridweb.data/webworksheet/autofitcolumn/#autofitcolumn_1)(int, int, int) | Ajuste automatiquement la largeur de la colonne. Cette méthode ajuste automatiquement une colonne en fonction du contenu d'une plage de cellules de la colonne de startRow à endRow. AutoFitColumn est une fonction imprécise. |
| [CancelNewBindRow](../../aspose.cells.gridweb.data/webworksheet/cancelnewbindrow/)() | Annule et supprime la nouvelle ligne liée ajoutée. |
| [CommitNewBindRow](../../aspose.cells.gridweb.data/webworksheet/commitnewbindrow/)() | Valide la nouvelle ligne liée ajoutée et l'ajoute au datasource. |
| [Copy](../../aspose.cells.gridweb.data/webworksheet/copy/)(WebWorksheet) | Copie à partir d'un autre objet feuille de calcul. |
| [CreateAutoGenratedColumns](../../aspose.cells.gridweb.data/webworksheet/createautogenratedcolumns/)() | Après avoir défini un datasource pour la feuille de calcul, appelez cette méthode pour générer automatiquement les colonnes liées. |
| [CreateNewBindRow](../../aspose.cells.gridweb.data/webworksheet/createnewbindrow/)() | Crée une nouvelle ligne liée et la lie au datasource. |
| [CreateSubtotal](../../aspose.cells.gridweb.data/webworksheet/createsubtotal/)(int, int, int, SubtotalFunction, int[], string, GridTableItemStyle, GridTableItemStyle, NumberType, string) | Crée un sous-total dans la feuille. |
| override [DataBind](../../aspose.cells.gridweb.data/webworksheet/databind/)() | Lie la feuille au DataSource. |
| [DeleteBindRow](../../aspose.cells.gridweb.data/webworksheet/deletebindrow/)(int) | Supprime une ligne liée. |
| [FreezePanes](../../aspose.cells.gridweb.data/webworksheet/freezepanes/)(int, int, int, int) | Gèle les volets à la cellule spécifiée dans la feuille de calcul. |
| [GroupRows](../../aspose.cells.gridweb.data/webworksheet/grouprows/#grouprows)(int, int) | Regroupe les lignes. |
| [GroupRows](../../aspose.cells.gridweb.data/webworksheet/grouprows/#grouprows_1)(int, int, bool) | Regroupe les lignes. |
| [SetAllCellsEditable](../../aspose.cells.gridweb.data/webworksheet/setallcellseditable/)() | Rend toutes les cellules modifiables. Ceci est un attribut étendu. |
| [SetAllCellsReadonly](../../aspose.cells.gridweb.data/webworksheet/setallcellsreadonly/)() | Rend toutes les cellules en lecture seule. Ceci est un attribut étendu, notez que cet attribut ne peut pas être conservé dans la cellule réelle ; si vous souhaitez conserver la protection, veuillez utiliser setProtect. |
| [SetEditableRange](../../aspose.cells.gridweb.data/webworksheet/seteditablerange/)(int, int, int, int) | Rend une plage de cellules modifiable. http://docs.aspose.com:8082/docs/display/cellsnet/Protecting+Cells Rendez toutes les cellules en lecture seule en appelant la méthode SetAllCellsReadonly. Ensuite, appelez cette méthode pour spécifier la plage de cellules qui doit être modifiable. |
| [SetReadonlyRange](../../aspose.cells.gridweb.data/webworksheet/setreadonlyrange/)(int, int, int, int) | Rend une plage de cellules en lecture seule. http://docs.aspose.com:8082/docs/display/cellsnet/Protecting+Cells Commencez par rendre toutes les cellules modifiables en appelant la méthode SetAllCellsEditable. Ensuite, appelez cette méthode pour spécifier la plage de cellules qui doit être en lecture seule. |
| [UnfreezePanes](../../aspose.cells.gridweb.data/webworksheet/unfreezepanes/)() | Défige les volets dans la feuille de calcul. |
| [UngroupRows](../../aspose.cells.gridweb.data/webworksheet/ungrouprows/)(int, int) | Dégroupe les lignes. |
| [UpdateBindCellValue](../../aspose.cells.gridweb.data/webworksheet/updatebindcellvalue/)(GridCell) | Met à jour la valeur de la propriété de l'enregistrement de la source de données liée selon la valeur de la cellule. |

### Remarques

NOTE : Cette classe est maintenant obsolète. Veuillez utiliser GridWorksheet à la place. Cette classe sera supprimée après 6 mois à compter d'août 2014. Aspose s'excuse pour tout inconvénient que vous auriez pu rencontrer.

### Exemples

```csharp

 [C#]
 ...
 using System.Web.UI.WebControls;
 ...
 ...

 WebWorksheets Worksheets = GridWeb1.WebWorksheets;
	WebCells cells = Worksheets[0].Cells;

	//Définit la hauteur de ligne par défaut
	cells.StandardHeight = new Unit(16, UnitType.Point);
	//Définit la hauteur de ligne
	cells.SetRowHeight(2, new Unit(20, UnitType.Point));

	//Définit la largeur de colonne par défaut
	cells.StandardWidth = new Unit(50, UnitType.Point);
	//Définit la largeur de colonne
	cells.SetColumnWidth(3, new Unit(80, UnitType.Point));

	//Fusionner des cellules
	cells.Merge(5, 4, 2, 2);

	//Importer des données
	DataSet1 ds1 = new DataSet1();

	for (int i =0; i<16; i++)
	{
		DataSet1.Table1Row row = ds1.Table1.NewTable1Row();
		row["c1"] = "hello1";
		row["c2"] = i;
		row["c3"] = "data";
		ds1.Table1.AddTable1Row(row);
	}

	GridWeb1.WebWorksheets.ImportDataView(ds1.Table1.DefaultView, null, null);

 //Importer depuis un fichier Excel
 Worksheets.ImportExcelFile("c:\\file1.xls");

 [Visual Basic]
	Imports System.Web.UI.WebControls
	...
	...

	Dim Worksheets As WebWorksheets =  GridWeb1.WebWorksheets
	Dim cells As WebCells =  Worksheets(0).Cells

	'Sets default row height
	cells.StandardHeight = New Unit(16, UnitType.Point)
	'Sets row height
	cells.SetRowHeight(2,New Unit(20,UnitType.Point))

	'Sets default colum width
	cells.StandardWidth = New Unit(50, UnitType.Point)
	'Sets column width
	cells.SetColumnWidth(3,New Unit(80,UnitType.Point))

	'Merge cells
	cells.Merge(5, 4, 2, 2)

	'Import data
	Dim ds1 As DataSet1 =  New DataSet1()

	Dim i As Integer
	For  i = 0 To 15
		Dim row As DataSet1.Table1Row =  ds1.Table1.NewTable1Row()
		row("c1") = "hello1"
		row("c2") = i
		row("c3") = "data"
		ds1.Table1.AddTable1Row(row)
	Next

	GridWeb1.WebWorksheets.ImportDataView(ds1.Table1.DefaultView, Nothing, Nothing)

	'Import from excel file
	Worksheets.ImportExcelFile("c:\\file1.xls")
```

### Voir aussi

* namespace [Aspose.Cells.GridWeb.Data](../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../)


