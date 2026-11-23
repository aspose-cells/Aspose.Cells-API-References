---
title: "Class GridWorksheet"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Aspose.Cells.GridWeb.Data.GridWorksheet class. encapsule l'objet qui représente une seule feuille de calcul"
type: docs
url: /fr/net/aspose.cells.gridweb.data/gridworksheet/
---
## GridWorksheet class

Encapsule l'objet qui représente une seule feuille de calcul.

```csharp
public class GridWorksheet : Control, ISerializable
```

## Propriétés

| Nom | Description |
| --- | --- |
| [ActiveCell](../../aspose.cells.gridweb.data/gridworksheet/activecell/) { get; set; } | Obtient ou définit la cellule active dans la feuille de calcul. |
| [BackgroundImage](../../aspose.cells.gridweb.data/gridworksheet/backgroundimage/) { get; set; } | Obtient et définit l'image d'arrière-plan de la feuille de calcul. |
| [BindColumns](../../aspose.cells.gridweb.data/gridworksheet/bindcolumns/) { get; } | Lier la collection de colonnes. |
| [BindingSource](../../aspose.cells.gridweb.data/gridworksheet/bindingsource/) { get; } | L'objet source de données réellement lié à l'exécution. Il s'agit d'un objet DataView lorsque la propriété DataSource est un objet DataSet, DataTable ou DataView. |
| [BindStartColumn](../../aspose.cells.gridweb.data/gridworksheet/bindstartcolumn/) { get; set; } | En mode liaison de données, BindStartRow et BindStartColumn indiquent la position de la grille à lier à la source de données. |
| [BindStartRow](../../aspose.cells.gridweb.data/gridworksheet/bindstartrow/) { get; set; } | En mode liaison de données, BindStartRow et BindStartColumn indiquent la position de la grille à lier à la source de données. |
| [Cells](../../aspose.cells.gridweb.data/gridworksheet/cells/) { get; } | Obtient la [`GridCell`](../gridcell/) collection. |
| [CodeName](../../aspose.cells.gridweb.data/gridworksheet/codename/) { get; } | Représente le nom de code de la feuille de calcul. |
| [Comments](../../aspose.cells.gridweb.data/gridworksheet/comments/) { get; } | Obtient la collection [`GridComment`](../gridcomment/). |
| [CurrentBindRows](../../aspose.cells.gridweb.data/gridworksheet/currentbindrows/) { get; set; } | Obtient le nombre de lignes de liaison en mode liaison de données. |
| [DataMember](../../aspose.cells.gridweb.data/gridworksheet/datamember/) { get; set; } | Obtient ou définit le DataMember à partir du DataSource multi-membres. En général, il représente un objet DataTable d'un DataSet. |
| [DataSource](../../aspose.cells.gridweb.data/gridworksheet/datasource/) { get; set; } | Obtient ou définit le DataSource. En général, c'est un objet DataSet. |
| [DisplayRightToLeft](../../aspose.cells.gridweb.data/gridworksheet/displayrighttoleft/) { get; set; } | Indique si la feuille de calcul spécifiée est affichée de droite à gauche au lieu de gauche à droite. La valeur par défaut est false. |
| [DisplayZeros](../../aspose.cells.gridweb.data/gridworksheet/displayzeros/) { get; set; } | Vrai si les valeurs zéro sont affichées. |
| [EnableCreateBindColumnHeader](../../aspose.cells.gridweb.data/gridworksheet/enablecreatebindcolumnheader/) { get; set; } | En mode liaison de données, indique s'il faut créer les légendes d'en-tête de colonne liées dans la feuille. |
| [FirstVisibleColumn](../../aspose.cells.gridweb.data/gridworksheet/firstvisiblecolumn/) { get; set; } | Représente l'index de la première colonne visible. |
| [FirstVisibleRow](../../aspose.cells.gridweb.data/gridworksheet/firstvisiblerow/) { get; set; } | Représente l'index de la première ligne visible. |
| [GridActiveCell](../../aspose.cells.gridweb.data/gridworksheet/gridactivecell/) { get; set; } | Obtient ou définit la cellule active dans la feuille de calcul. |
| [Hyperlinks](../../aspose.cells.gridweb.data/gridworksheet/hyperlinks/) { get; } | Obtient la collection [`GridHyperlinkCollection`](../gridhyperlinkcollection/). |
| [Index](../../aspose.cells.gridweb.data/gridworksheet/index/) { get; } | Obtient l'index de la feuille dans la collection de feuilles de calcul. |
| [IsGridlinesVisible](../../aspose.cells.gridweb.data/gridworksheet/isgridlinesvisible/) { get; set; } | Obtient ou définit une valeur indiquant si les lignes de grille sont visibles. La valeur par défaut est true. |
| [IsSummaryRowBelow](../../aspose.cells.gridweb.data/gridworksheet/issummaryrowbelow/) { get; set; } | Indique si la ligne de synthèse sera positionnée sous les lignes de détail dans le plan. |
| [Name](../../aspose.cells.gridweb.data/gridworksheet/name/) { get; set; } | Obtient ou définit le nom de la feuille de calcul. |
| [OutlineShown](../../aspose.cells.gridweb.data/gridworksheet/outlineshown/) { get; set; } | Indique si le contour doit être affiché. |
| [Pictures](../../aspose.cells.gridweb.data/gridworksheet/pictures/) { get; } | Obtient une collection [`Pictures`](./pictures/). |
| [PivotTables](../../aspose.cells.gridweb.data/gridworksheet/pivottables/) { get; } | Obtient les pivotTables dans la feuille de calcul. |
| [Selected](../../aspose.cells.gridweb.data/gridworksheet/selected/) { get; set; } | Indique si cette feuille de calcul est sélectionnée lorsque le classeur est ouvert. |
| [Shapes](../../aspose.cells.gridweb.data/gridworksheet/shapes/) { get; } | Obtient une collection [`Pictures`](./pictures/). |
| [StandardHeight](../../aspose.cells.gridweb.data/gridworksheet/standardheight/) { get; set; } | Obtient ou définit la hauteur de ligne par défaut dans cette feuille de calcul, en points. |
| [StandardHeightPixels](../../aspose.cells.gridweb.data/gridworksheet/standardheightpixels/) { get; set; } | Obtient ou définit la hauteur de ligne par défaut dans cette feuille de calcul, en pixels. |
| [TabColor](../../aspose.cells.gridweb.data/gridworksheet/tabcolor/) { get; set; } | Représente la couleur de l'onglet de la feuille de calcul. |
| [Validations](../../aspose.cells.gridweb.data/gridworksheet/validations/) { get; } | Obtient la collection des paramètres de validation des données dans la feuille de calcul. |
| override [Visible](../../aspose.cells.gridweb.data/gridworksheet/visible/) { get; set; } | Indique si le nom de cette feuille est affiché dans les onglets de feuille du contrôle. |
| [Workbook](../../aspose.cells.gridweb.data/gridworksheet/workbook/) { get; } | Obtient l'objet [`GridWorkbook`](../gridworkbook/) de la collection de feuilles de calcul. |
| [Zoom](../../aspose.cells.gridweb.data/gridworksheet/zoom/) { get; set; } | Représente le facteur d'échelle en pourcentage. Il doit être compris entre 10 et 400. |

## Méthodes

| Nom | Description |
| --- | --- |
| [AddAutoFilter](../../aspose.cells.gridweb.data/gridworksheet/addautofilter/)(int, int, int) | Définit la plage à laquelle le AutoFilter spécifié s'applique. |
| [AddCustomFilter](../../aspose.cells.gridweb.data/gridworksheet/addcustomfilter/)(int, string) | Ajoute un filtre personnalisé pour la ligne spécifiée. |
| [AutoFitColumn](../../aspose.cells.gridweb.data/gridworksheet/autofitcolumn/#autofitcolumn)(int) | Ajuste automatiquement la largeur de la colonne. |
| [AutoFitColumn](../../aspose.cells.gridweb.data/gridworksheet/autofitcolumn/#autofitcolumn_1)(int, int, int) | Ajuste automatiquement la largeur de la colonne. |
| [AutoFitColumns](../../aspose.cells.gridweb.data/gridworksheet/autofitcolumns/)() |  |
| [AutoFitRow](../../aspose.cells.gridweb.data/gridworksheet/autofitrow/#autofitrow)(int) | Ajuste automatiquement la hauteur de la ligne. |
| [AutoFitRow](../../aspose.cells.gridweb.data/gridworksheet/autofitrow/#autofitrow_1)(int, int, int) | Ajuste automatiquement la hauteur de la ligne. |
| [AutoFitRow](../../aspose.cells.gridweb.data/gridworksheet/autofitrow/#autofitrow_2)(int, int, int, int) | Ajuste automatiquement la hauteur de la ligne dans une plage rectangulaire. |
| [AutoFitRows](../../aspose.cells.gridweb.data/gridworksheet/autofitrows/#autofitrows)() | Ajuste automatiquement toutes les lignes de cette feuille de calcul. |
| [AutoFitRows](../../aspose.cells.gridweb.data/gridworksheet/autofitrows/#autofitrows_1)(bool) | Ajuste automatiquement toutes les lignes de cette feuille de calcul. |
| [AutoFitRows](../../aspose.cells.gridweb.data/gridworksheet/autofitrows/#autofitrows_2)(int, int) | Ajuste automatiquement la hauteur de la ligne dans une plage. |
| [CalculateFormula](../../aspose.cells.gridweb.data/gridworksheet/calculateformula/)(string) | Calcule une formule. |
| [CancelNewBindRow](../../aspose.cells.gridweb.data/gridworksheet/cancelnewbindrow/)() | Annule et supprime la nouvelle ligne liée ajoutée. |
| [ClearComments](../../aspose.cells.gridweb.data/gridworksheet/clearcomments/)() | Efface tous les commentaires dans la feuille de calcul du concepteur. |
| [CommitNewBindRow](../../aspose.cells.gridweb.data/gridworksheet/commitnewbindrow/)() | Valide la nouvelle ligne liée ajoutée et l'ajoute au datasource. |
| [Copy](../../aspose.cells.gridweb.data/gridworksheet/copy/)(GridWorksheet) | Copie le contenu et les formats d'une autre feuille de calcul. |
| [CreateAutoGenratedColumns](../../aspose.cells.gridweb.data/gridworksheet/createautogenratedcolumns/)() | Après avoir défini un datasource pour la feuille de calcul, appelez cette méthode pour générer automatiquement les colonnes liées. |
| [CreateNewBindRow](../../aspose.cells.gridweb.data/gridworksheet/createnewbindrow/)() | Crée une nouvelle ligne liée et la lie au datasource. |
| [CreateSubtotal](../../aspose.cells.gridweb.data/gridworksheet/createsubtotal/#createsubtotal)(int, int, int, SubtotalFunction, int[]) | Crée un sous-total dans la feuille. |
| [CreateSubtotal](../../aspose.cells.gridweb.data/gridworksheet/createsubtotal/#createsubtotal_1)(int, int, int, SubtotalFunction, int[], string, GridTableItemStyle, GridTableItemStyle, NumberType, string) | Crée un sous-total dans la feuille. |
| override [DataBind](../../aspose.cells.gridweb.data/gridworksheet/databind/)() | Lie la feuille au DataSource. |
| [DataSourceControlUpdate](../../aspose.cells.gridweb.data/gridworksheet/datasourcecontrolupdate/)(AccessDataSource) | Lie la feuille au DataSource. |
| [DeleteBindRow](../../aspose.cells.gridweb.data/gridworksheet/deletebindrow/)(int) | Supprime une ligne liée. |
| [FilterString](../../aspose.cells.gridweb.data/gridworksheet/filterstring/)(int, string) | Définit le filtre pour la colonne. Notez que nous devons appeler AddAutoFilter avant d'appeler filterString. La chaîne de critères de filtre. Notez que nous utilisons la virgule-&gt;"," comme caractère de séparation, donc la valeur de cellule que vous souhaitez filtrer ne doit pas contenir de virgule. filterString(10,"123,456") signifie que la colonne 10 doit contenir 123 ou 456, filterString(10,"123") signifie que la colonne 10 doit contenir 123. L'index de colonne est séparé par des virgules, par ex. 123,456,789 ou abc |
| [FreezePanes](../../aspose.cells.gridweb.data/gridworksheet/freezepanes/#freezepanes_1)(string, int, int) | Gèle les volets à la cellule spécifiée dans la feuille de calcul. |
| [FreezePanes](../../aspose.cells.gridweb.data/gridworksheet/freezepanes/#freezepanes)(int, int, int, int) | Gèle les volets à la cellule spécifiée dans la feuille de calcul. |
| [GetColumnCaption](../../aspose.cells.gridweb.data/gridworksheet/getcolumncaption/)(int) | Obtient la légende de la colonne. Si la légende n'est pas définie, renvoie une chaîne vide. |
| [GetColumnHeaderToolTip](../../aspose.cells.gridweb.data/gridworksheet/getcolumnheadertooltip/)(int) | Obtient le texte de l'infobulle de l'en-tête de colonne. |
| [GetColumnReadonly](../../aspose.cells.gridweb.data/gridworksheet/getcolumnreadonly/)(int) | Obtient si une colonne est en lecture seule. il s'agit d'une méthode étendue de GridWeb spécifiquement, elle ne sera pas conservée ni prise en compte dans le fichier Excel réel. |
| [GetFreezedPanes](../../aspose.cells.gridweb.data/gridworksheet/getfreezedpanes/)(out int, out int, out int, out int) | Obtient les volets figés. |
| [GetIsReadonly](../../aspose.cells.gridweb.data/gridworksheet/getisreadonly/)(int, int) | Obtient si la cellule est en lecture seule. il s'agit d'un attribut étendu de GridWeb, il ne sera pas conservé dans le fichier Excel réel. |
| [GetRowCaption](../../aspose.cells.gridweb.data/gridworksheet/getrowcaption/)(int) | Obtient la légende de la ligne. Si la légende n'est pas définie, renvoie une chaîne vide. |
| [GetRowHeaderToolTip](../../aspose.cells.gridweb.data/gridworksheet/getrowheadertooltip/)(int) | Obtient le texte de l'infobulle de l'en-tête de ligne. |
| [GetRowReadonly](../../aspose.cells.gridweb.data/gridworksheet/getrowreadonly/)(int) | Obtient si une ligne est en lecture seule. Cette méthode étendue de GridWeb spécifiquement ne sera pas conservée et n'affectera pas le fichier Excel réel. |
| [GroupRows](../../aspose.cells.gridweb.data/gridworksheet/grouprows/)(int, int, bool) | Regroupe les lignes. |
| [IsProtected](../../aspose.cells.gridweb.data/gridworksheet/isprotected/)() | Indique si la feuille de calcul est protégée. |
| [MoveTo](../../aspose.cells.gridweb.data/gridworksheet/moveto/)(int) | Déplace la feuille vers un autre emplacement dans la feuille de calcul. |
| [RefreshFilter](../../aspose.cells.gridweb.data/gridworksheet/refreshfilter/)() | Actualise les filtres automatiques pour masquer ou afficher les lignes. |
| [RemoveAutoFilter](../../aspose.cells.gridweb.data/gridworksheet/removeautofilter/)() | Supprime le filtre automatique de la feuille de calcul. |
| [RemoveSubtotal](../../aspose.cells.gridweb.data/gridworksheet/removesubtotal/)() | Supprime le sous-total créé par la méthode CreateSubtotal dans la feuille. |
| [ResetFilter](../../aspose.cells.gridweb.data/gridworksheet/resetfilter/)(int) | Le décalage entier du champ sur lequel vous souhaitez appliquer, basé sur la première colonne de filtre (à partir de la gauche de la liste ; le champ le plus à gauche est le champ 0). |
| [SetAllCellsEditable](../../aspose.cells.gridweb.data/gridworksheet/setallcellseditable/)() | Rend toutes les cellules modifiables. Ceci est un attribut étendu. |
| [SetAllCellsReadonly](../../aspose.cells.gridweb.data/gridworksheet/setallcellsreadonly/)() | Rend toutes les cellules en lecture seule. Ceci est un attribut étendu, notez que cet attribut ne peut pas être conservé dans la cellule réelle ; si vous souhaitez conserver la protection, veuillez utiliser setProtect. |
| [SetColumnCaption](../../aspose.cells.gridweb.data/gridworksheet/setcolumncaption/)(int, string) | Définit la légende pour la colonne. Veuillez noter que c'est un attribut d'extension et qu'il ne peut pas être conservé dans le fichier Excel. |
| [SetColumnHeaderToolTip](../../aspose.cells.gridweb.data/gridworksheet/setcolumnheadertooltip/)(int, string) | Définit le texte de l'infobulle de l'en-tête de colonne. |
| [SetColumnReadonly](../../aspose.cells.gridweb.data/gridworksheet/setcolumnreadonly/)(int, bool) | Définit une colonne en lecture seule afin que l'utilisateur ne puisse pas la supprimer côté client. Cette méthode étendue de GridWeb spécifiquement ne sera pas conservée et n'affectera pas le fichier Excel réel. |
| [SetEditableRange](../../aspose.cells.gridweb.data/gridworksheet/seteditablerange/)(int, int, int, int) | Rend une plage de cellules modifiable. http://docs.aspose.com:8082/docs/display/cellsnet/Protecting+Cells Rendez toutes les cellules en lecture seule en appelant la méthode SetAllCellsReadonly. Ensuite, appelez cette méthode pour spécifier la plage de cellules qui doit être modifiable. |
| [SetIsReadonly](../../aspose.cells.gridweb.data/gridworksheet/setisreadonly/)(int, int, bool) | Définit si la cellule est en lecture seule. Ceci est un attribut étendu de GridWeb, il ne sera pas conservé dans le fichier Excel réel. |
| [SetProtect](../../aspose.cells.gridweb.data/gridworksheet/setprotect/)() | Protège la feuille de calcul. |
| [SetReadonlyRange](../../aspose.cells.gridweb.data/gridworksheet/setreadonlyrange/)(int, int, int, int) | Rend une plage de cellules en lecture seule. http://docs.aspose.com:8082/docs/display/cellsnet/Protecting+Cells Commencez par rendre toutes les cellules modifiables en appelant la méthode SetAllCellsEditable. Ensuite, appelez cette méthode pour spécifier la plage de cellules qui doit être en lecture seule. |
| [SetRowCaption](../../aspose.cells.gridweb.data/gridworksheet/setrowcaption/)(int, string) | Définit la légende pour la ligne. |
| [SetRowHeaderToolTip](../../aspose.cells.gridweb.data/gridworksheet/setrowheadertooltip/)(int, string) | Définit le texte de l'infobulle de l'en-tête de ligne. |
| [SetRowReadonly](../../aspose.cells.gridweb.data/gridworksheet/setrowreadonly/)(int, bool) | Définit une ligne en lecture seule afin que l'utilisateur ne puisse pas la supprimer côté client. Cette méthode étendue de GridWeb spécifiquement ne sera pas conservée et n'affectera pas le fichier Excel réel. |
| [UnFreezePanes](../../aspose.cells.gridweb.data/gridworksheet/unfreezepanes/)() | Défige les volets dans la feuille de calcul. |
| [UnGroupRows](../../aspose.cells.gridweb.data/gridworksheet/ungrouprows/)(int, int) | Dégroupe les lignes. |
| [UnProtect](../../aspose.cells.gridweb.data/gridworksheet/unprotect/)() | Supprime la protection de la feuille de calcul. |

## Événements

| Nom | Description |
| --- | --- |
| event [InitializeNewBindRow](../../aspose.cells.gridweb.data/gridworksheet/initializenewbindrow/) | Se produit lorsque la feuille de calcul a créé une nouvelle ligne liée et doit l'initialiser. |

### Voir aussi

* namespace [Aspose.Cells.GridWeb.Data](../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../)


