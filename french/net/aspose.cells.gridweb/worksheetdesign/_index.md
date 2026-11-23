---
title: "Classe WorksheetDesign"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Aspose.Cells.GridWeb.WorksheetDesign classe. Hérité de WebWorksheet. Utilisé uniquement en temps de conception."
type: docs
url: /fr/net/aspose.cells.gridweb/worksheetdesign/
---
## WorksheetDesign class

Hérité de WebWorksheet. Utilisé uniquement en mode conception.

```csharp
public class WorksheetDesign : WebWorksheet
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [WorksheetDesign](worksheetdesign/#constructor)() | Constructeur par défaut. |
| [WorksheetDesign](worksheetdesign/#constructor_1)(MainWeb, GridWorksheet) | le constructeur avec MainWeb et GridWorksheet |

## Propriétés

| Nom | Description |
| --- | --- |
| [BindColumns](../../aspose.cells.gridweb.data/webworksheet/bindcolumns/) { get; } | Collection de colonnes de liaison.(Hérité de [`WebWorksheet`](../../aspose.cells.gridweb.data/webworksheet/).) |
| [BindingSource](../../aspose.cells.gridweb.data/webworksheet/bindingsource/) { get; } | L'objet source de données réellement lié à l'exécution. C'est un objet DataView lorsque la propriété DataSource est un objet DataSet, DataTable ou DataView.(Hérité de [`WebWorksheet`](../../aspose.cells.gridweb.data/webworksheet/).) |
| [BindStartColumn](../../aspose.cells.gridweb.data/webworksheet/bindstartcolumn/) { get; set; } | En mode liaison de données, BindStartRow et BindStartColumn indiquent la position de la grille à lier à la source de données.(Hérité de [`WebWorksheet`](../../aspose.cells.gridweb.data/webworksheet/).) |
| [BindStartRow](../../aspose.cells.gridweb.data/webworksheet/bindstartrow/) { get; set; } | En mode liaison de données, BindStartRow et BindStartColumn indiquent la position de la grille à lier à la source de données.(Hérité de [`WebWorksheet`](../../aspose.cells.gridweb.data/webworksheet/).) |
| [CellImages](../../aspose.cells.gridweb.data/webworksheet/cellimages/) { get; } | (Hérité de [`WebWorksheet`](../../aspose.cells.gridweb.data/webworksheet/).) |
| [Cells](../../aspose.cells.gridweb.data/webworksheet/cells/) { get; } | Obtient le [`WebCells`](../../aspose.cells.gridweb.data/webcells/).(Hérité de [`WebWorksheet`](../../aspose.cells.gridweb.data/webworksheet/).) |
| [Comments](../../aspose.cells.gridweb.data/webworksheet/comments/) { get; } | (Hérité de [`WebWorksheet`](../../aspose.cells.gridweb.data/webworksheet/).) |
| [CurrentBindRows](../../aspose.cells.gridweb.data/webworksheet/currentbindrows/) { get; set; } | Obtient le nombre de lignes liées en mode liaison de données.(Hérité de [`WebWorksheet`](../../aspose.cells.gridweb.data/webworksheet/).) |
| [DataMember](../../aspose.cells.gridweb.data/webworksheet/datamember/) { get; set; } | Obtient ou définit le DataMember de la source de données multi-membres. Généralement, il représente un objet DataTable d'un DataSet.(Hérité de [`WebWorksheet`](../../aspose.cells.gridweb.data/webworksheet/).) |
| [DataSource](../../aspose.cells.gridweb.data/webworksheet/datasource/) { get; set; } | Obtient ou définit la DataSource. Généralement, c'est un objet DataSet.(Hérité de [`WebWorksheet`](../../aspose.cells.gridweb.data/webworksheet/).) |
| [EnableCreateBindColumnHeader](../../aspose.cells.gridweb.data/webworksheet/enablecreatebindcolumnheader/) { get; set; } | En mode liaison de données, indique s'il faut créer les légendes d'en-tête de colonne liées dans la feuille.(Hérité de [`WebWorksheet`](../../aspose.cells.gridweb.data/webworksheet/).) |
| [Hyperlinks](../../aspose.cells.gridweb.data/webworksheet/hyperlinks/) { get; } | Obtient la collection HyperlinkCollection.(Hérité de [`WebWorksheet`](../../aspose.cells.gridweb.data/webworksheet/).) |
| [Index](../../aspose.cells.gridweb.data/webworksheet/index/) { get; } | Obtient l'index de lui-même parmi les feuilles de calcul.(Hérité de [`WebWorksheet`](../../aspose.cells.gridweb.data/webworksheet/).) |
| [IsProtected](../../aspose.cells.gridweb.data/webworksheet/isprotected/) { get; set; } | Obtient ou définit si la feuille de calcul est protégée. Lorsqu'une feuille de calcul est protégée, toutes les cellules ne peuvent pas être modifiées sauf la cellule dont la propriété IsLocked est false.(Hérité de [`WebWorksheet`](../../aspose.cells.gridweb.data/webworksheet/).) |
| [Name](../../aspose.cells.gridweb.data/webworksheet/name/) { get; set; } | Obtient ou définit le nom de la feuille.(Hérité de [`WebWorksheet`](../../aspose.cells.gridweb.data/webworksheet/).) |
| [RowFilter](../../aspose.cells.gridweb.data/webworksheet/rowfilter/) { get; } | (Hérité de [`WebWorksheet`](../../aspose.cells.gridweb.data/webworksheet/).) |
| [Validations](../../aspose.cells.gridweb.data/webworksheet/validations/) { get; } | Obtient la collection des paramètres de validation des données dans la feuille de calcul.(Hérité de [`WebWorksheet`](../../aspose.cells.gridweb.data/webworksheet/).) |
| override [Visible](../../aspose.cells.gridweb.data/webworksheet/visible/) { get; set; } | Indique si le nom de cette feuille est affiché dans les onglets de feuilles du contrôle.(Hérité de [`WebWorksheet`](../../aspose.cells.gridweb.data/webworksheet/).) |

## Méthodes

| Nom | Description |
| --- | --- |
| [AutoFitColumn](../../aspose.cells.gridweb.data/webworksheet/autofitcolumn/)(int) | Ajuste automatiquement la largeur de la colonne.(Hérité de [`WebWorksheet`](../../aspose.cells.gridweb.data/webworksheet/).) |
| [AutoFitColumn](../../aspose.cells.gridweb.data/webworksheet/autofitcolumn/)(int, int, int) | Ajuste automatiquement la largeur de la colonne. Cette méthode ajuste automatiquement une colonne en fonction du contenu d'une plage de cellules dans la colonne, de startRow à endRow. AutoFitColumn est une fonction imprécise.(Hérité de [`WebWorksheet`](../../aspose.cells.gridweb.data/webworksheet/).) |
| [CancelNewBindRow](../../aspose.cells.gridweb.data/webworksheet/cancelnewbindrow/)() | Annule et supprime la nouvelle ligne liée ajoutée.(Hérité de [`WebWorksheet`](../../aspose.cells.gridweb.data/webworksheet/).) |
| [CommitNewBindRow](../../aspose.cells.gridweb.data/webworksheet/commitnewbindrow/)() | Valide la nouvelle ligne liée ajoutée et l'ajoute à la source de données.(Hérité de [`WebWorksheet`](../../aspose.cells.gridweb.data/webworksheet/).) |
| [Copy](../../aspose.cells.gridweb.data/webworksheet/copy/)(WebWorksheet) | Copie à partir d'un autre objet de feuille de calcul.(Hérité de [`WebWorksheet`](../../aspose.cells.gridweb.data/webworksheet/).) |
| [CreateAutoGenratedColumns](../../aspose.cells.gridweb.data/webworksheet/createautogenratedcolumns/)() | Après avoir défini une source de données pour la feuille de calcul, appelez cette méthode pour générer automatiquement les colonnes liées.(Hérité de [`WebWorksheet`](../../aspose.cells.gridweb.data/webworksheet/).) |
| [CreateNewBindRow](../../aspose.cells.gridweb.data/webworksheet/createnewbindrow/)() | Crée une nouvelle ligne liée et la lie à la source de données.(Hérité de [`WebWorksheet`](../../aspose.cells.gridweb.data/webworksheet/).) |
| [CreateSubtotal](../../aspose.cells.gridweb.data/webworksheet/createsubtotal/)(int, int, int, SubtotalFunction, int[], string, GridTableItemStyle, GridTableItemStyle, NumberType, string) | Crée un sous-total dans la feuille.(Hérité de [`WebWorksheet`](../../aspose.cells.gridweb.data/webworksheet/).) |
| override [DataBind](../../aspose.cells.gridweb.data/webworksheet/databind/)() | Lie la feuille à la source de données.(Hérité de [`WebWorksheet`](../../aspose.cells.gridweb.data/webworksheet/).) |
| [DeleteBindRow](../../aspose.cells.gridweb.data/webworksheet/deletebindrow/)(int) | Supprime une ligne liée.(Hérité de [`WebWorksheet`](../../aspose.cells.gridweb.data/webworksheet/).) |
| [FreezePanes](../../aspose.cells.gridweb.data/webworksheet/freezepanes/)(int, int, int, int) | Gèle les volets à la cellule spécifiée dans la feuille de calcul.(Hérité de [`WebWorksheet`](../../aspose.cells.gridweb.data/webworksheet/).) |
| [GroupRows](../../aspose.cells.gridweb.data/webworksheet/grouprows/)(int, int) | Regroupe les lignes.(Hérité de [`WebWorksheet`](../../aspose.cells.gridweb.data/webworksheet/).) |
| [GroupRows](../../aspose.cells.gridweb.data/webworksheet/grouprows/)(int, int, bool) | Regroupe les lignes.(Hérité de [`WebWorksheet`](../../aspose.cells.gridweb.data/webworksheet/).) |
| [SetAllCellsEditable](../../aspose.cells.gridweb.data/webworksheet/setallcellseditable/)() | Rend toutes les cellules modifiables.cet attribut est étendu(Hérité de [`WebWorksheet`](../../aspose.cells.gridweb.data/webworksheet/).) |
| [SetAllCellsReadonly](../../aspose.cells.gridweb.data/webworksheet/setallcellsreadonly/)() | Rend toutes les cellules en lecture seule.cet attribut est étendu, notez que cet attribut ne peut pas être conservé dans la cellule réelle, si vous voulez garder la protection veuillez utiliser setProtect(Hérité de [`WebWorksheet`](../../aspose.cells.gridweb.data/webworksheet/).) |
| [SetEditableRange](../../aspose.cells.gridweb.data/webworksheet/seteditablerange/)(int, int, int, int) | Rend une plage de cellules modifiable. http://docs.aspose.com:8082/docs/display/cellsnet/Protecting+Cells Rendre toutes les cellules en lecture seule en appelant la méthode SetAllCellsReadonly. puis appeler cette méthode pour spécifier la plage de cellules qui doit être modifiable(Hérité de [`WebWorksheet`](../../aspose.cells.gridweb.data/webworksheet/).) |
| [SetReadonlyRange](../../aspose.cells.gridweb.data/webworksheet/setreadonlyrange/)(int, int, int, int) | Rend une plage de cellules en lecture seule. http://docs.aspose.com:8082/docs/display/cellsnet/Protecting+Cells D'abord rendre toutes les cellules modifiables en appelant la méthode SetAllCellsEditable. puis appeler cette méthode pour spécifier la plage de cellules qui doit être en lecture seule(Hérité de [`WebWorksheet`](../../aspose.cells.gridweb.data/webworksheet/).) |
| [UnfreezePanes](../../aspose.cells.gridweb.data/webworksheet/unfreezepanes/)() | Dégele les volets dans la feuille de calcul.(Hérité de [`WebWorksheet`](../../aspose.cells.gridweb.data/webworksheet/).) |
| [UngroupRows](../../aspose.cells.gridweb.data/webworksheet/ungrouprows/)(int, int) | Dégroupe les lignes.(Hérité de [`WebWorksheet`](../../aspose.cells.gridweb.data/webworksheet/).) |
| [UpdateBindCellValue](../../aspose.cells.gridweb.data/webworksheet/updatebindcellvalue/)(GridCell) | Met à jour la valeur de la propriété de l'enregistrement de la source de données liée en fonction de la valeur de la cellule.(Hérité de [`WebWorksheet`](../../aspose.cells.gridweb.data/webworksheet/).) |

### Voir aussi

* class [WebWorksheet](../../aspose.cells.gridweb.data/webworksheet/)
* namespace [Aspose.Cells.GridWeb](../../aspose.cells.gridweb/)
* assembly [Aspose.Cells.GridWeb](../../)


