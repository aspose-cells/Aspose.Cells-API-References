---
title: GridDesktop
second_title: Référence de l'API Aspose.Cells pour .NET
description: Aspose GridDesktop class Représente un objet racine pour créer un contrôle GridDesktop. Pour utiliser ce contrôle faites-le simplement glisser de votre boîte à outils vers un formulaire ou un contrôle utilisateur.
type: docs
weight: 840
url: /fr/net/aspose.cells.griddesktop/griddesktop/
---
## GridDesktop class

Aspose GridDesktop class Représente un objet racine pour créer un contrôle GridDesktop. Pour utiliser ce contrôle, faites-le simplement glisser de votre boîte à outils vers un formulaire ou un contrôle utilisateur.

```csharp
public class GridDesktop : UserControl
```

## Constructeurs

| Nom | La description |
| --- | --- |
| [GridDesktop](griddesktop)() | Aspose GridDesktop class |

## Propriétés

| Nom | La description |
| --- | --- |
| [ActiveSheetIndex](../../aspose.cells.griddesktop/griddesktop/activesheetindex) { get; set; } | Obtient ou définit l'index de feuille sélectionné. |
| [ActiveSheetNameFont](../../aspose.cells.griddesktop/griddesktop/activesheetnamefont) { get; set; } | Obtient ou définit la feuille active affichant la police de la barre de feuille. |
| [AlwasysRecalculateAllFormulas](../../aspose.cells.griddesktop/griddesktop/alwasysrecalculateallformulas) { get; set; } | Obtient ou définit une valeur indiquant si nous devons exécuter toutes les formules, comme lorsque nous exécutons toutes les formules, lors de la mise à jour d'une valeur de cellule, et cela affecte les autres, et d'autres affectent les autres, de plus en plus, car les cellules entières doivent être recalculées , tout comme l'effet papillon, il a besoin de beaucoup d'opérations de pile, il obtiendra des performances très faibles, comme dans CELLSNET-41921, ce problème contient le fichier même qui peut montrer ce scénario nous ferions mieux d'exécuter toutes les formules, , comme lors de l'exécution de toutes les formules, nous pouvons avoir une optimisation. |
| [BorderStyle](../../aspose.cells.griddesktop/griddesktop/borderstyle) { get; set; } | Indique le style de bordure du contrôle. |
| [ColumnHeaderVisible](../../aspose.cells.griddesktop/griddesktop/columnheadervisible) { get; set; } | Obtient ou définit une valeur indiquant si l'en-tête de colonne est visible. |
| [CommentDisplayingFont](../../aspose.cells.griddesktop/griddesktop/commentdisplayingfont) { get; set; } | Obtient ou définit la police d'affichage par défaut du texte de commentaire. |
| [ContextMenuManager](../../aspose.cells.griddesktop/griddesktop/contextmenumanager) { get; } | Obtient l'instance ContextMenuManager. |
| [DefaultCellFont](../../aspose.cells.griddesktop/griddesktop/defaultcellfont) { get; set; } | Obtient ou définit la police par défaut de la cellule |
| [DefaultCellFontColor](../../aspose.cells.griddesktop/griddesktop/defaultcellfontcolor) { get; set; } | Obtient ou définit la couleur de police par défaut de la cellule. |
| [EnableClipboardCopyPaste](../../aspose.cells.griddesktop/griddesktop/enableclipboardcopypaste) { get; set; } | Indique s'il faut copier/coller en fonction du presse-papiers, afin qu'il puisse copier/coller avec MS-EXCEL. Il copie/colle uniquement la valeur de la cellule, il ne copie aucun autre paramètre de la cellule comme le format, le style de bordure, etc. La valeur par défaut est false. |
| [EnableCopyWithExtension](../../aspose.cells.griddesktop/griddesktop/enablecopywithextension) { get; set; } | Obtient ou définit une valeur indiquant si l'opération de copie étendra le nombre de lignes ou de colonnes. |
| [EnableCopyWithLockedOption](../../aspose.cells.griddesktop/griddesktop/enablecopywithlockedoption) { get; set; } | Obtient ou définit une valeur indiquant si l'opération de copie copiera la valeur d'attribut CellLocked du style d'une cellule. |
| [EnableUndo](../../aspose.cells.griddesktop/griddesktop/enableundo) { get; set; } | Obtient ou définit une valeur indiquant si la fonction Annuler est activée. La valeur par défaut est false. |
| [GridMemorySetting](../../aspose.cells.griddesktop/griddesktop/gridmemorysetting) { get; set; } | Obtient ou définit l'option de mémoire. |
| [IsHorizontalScrollBarVisible](../../aspose.cells.griddesktop/griddesktop/ishorizontalscrollbarvisible) { get; set; } | Définit la statue visible pour la barre de défilement horizontale. |
| [IsVerticalScrollBarVisible](../../aspose.cells.griddesktop/griddesktop/isverticalscrollbarvisible) { get; set; } | Définit la statue visible pour la barre de défilement verticale. |
| [Names](../../aspose.cells.griddesktop/griddesktop/names) { get; } | Obtient la collection de tous les objets Name dans la feuille de calcul. |
| [PageRows](../../aspose.cells.griddesktop/griddesktop/pagerows) { get; set; } | définit ou obtient la taille de ligne pour la pagination. le maximum de PageRows pris en charge est de 100 000, le nombre maximum de numéros de page pris en charge est de 5 000. |
| [PasteType](../../aspose.cells.griddesktop/griddesktop/pastetype) { get; set; } | Indique quel type de collage lors de l'action de collage ， uniquement disponible lorsque EnableClipboardCopyPaste est faux . |
| [R1C1](../../aspose.cells.griddesktop/griddesktop/r1c1) { get; set; } | Obtient ou définit une valeur indiquant si le contrôle utilise le style de référence R1C1. |
| [RecalculateFormulas](../../aspose.cells.griddesktop/griddesktop/recalculateformulas) { get; set; } | Obtient ou définit une valeur indiquant s'il faut recalculer la formule de toutes les cellules lorsque la valeur d'une cellule a changé. La valeur par défaut est true. |
| [RowHeaderVisible](../../aspose.cells.griddesktop/griddesktop/rowheadervisible) { get; set; } | Obtient ou définit une valeur indiquant si l'en-tête de ligne est visible. |
| [SheetNameFont](../../aspose.cells.griddesktop/griddesktop/sheetnamefont) { get; set; } | Obtient ou définit la police d'affichage par défaut de la barre de feuille. |
| [SheetsBarVisible](../../aspose.cells.griddesktop/griddesktop/sheetsbarvisible) { get; set; } | Obtient ou définit une valeur indiquant si la barre de feuille est visible. |
| [SheetTabWidth](../../aspose.cells.griddesktop/griddesktop/sheettabwidth) { get; set; } | Définit/Obtient la largeur de l'onglet de la feuille. |
| [ShowContextMenu](../../aspose.cells.griddesktop/griddesktop/showcontextmenu) { get; set; } | Obtient ou définit une valeur indiquant si le contrôle peut afficher le menu contextuel. |
| [ShowStatus](../../aspose.cells.griddesktop/griddesktop/showstatus) { get; set; } | Obtient ou définit une valeur indiquant s'il faut afficher l'état de calcul La valeur par défaut est true. |
| [UndoManager](../../aspose.cells.griddesktop/griddesktop/undomanager) { get; } | Obtient l'instance UndoManager. |
| [Worksheets](../../aspose.cells.griddesktop/griddesktop/worksheets) { get; } | obtient les feuilles de travail. |

## Méthodes

| Nom | La description |
| --- | --- |
| [Clear](../../aspose.cells.griddesktop/griddesktop/clear)() | Efface le contrôle GridDesktop. |
| [Copy](../../aspose.cells.griddesktop/griddesktop/copy)() | Copie le contenu de la cellule ciblée dans le presse-papiers. |
| [Cut](../../aspose.cells.griddesktop/griddesktop/cut)() | Coupe le contenu de la cellule ciblée dans le presse-papiers. |
| [DoSplit](../../aspose.cells.griddesktop/griddesktop/dosplit)() | Définit la vue fractionnée. |
| [EndFormatPainter](../../aspose.cells.griddesktop/griddesktop/endformatpainter)() | Notifie à GridDesktop de mettre fin à FormatPainter. |
| [ExportExcelFile](../../aspose.cells.griddesktop/griddesktop/exportexcelfile#exportexcelfile)(Stream) | Exporte vers un flux de fichier Excel, y compris le flux d'E/S de disque ou le flux de mémoire. |
| [ExportExcelFile](../../aspose.cells.griddesktop/griddesktop/exportexcelfile#exportexcelfile_2)(string) | Exporte vers un fichier Excel. |
| [ExportExcelFile](../../aspose.cells.griddesktop/griddesktop/exportexcelfile#exportexcelfile_1)(Stream, FileFormatType) | Exporte vers un flux de fichier Excel, y compris le flux d'E/S de disque ou le flux de mémoire. |
| [ExportExcelFile](../../aspose.cells.griddesktop/griddesktop/exportexcelfile#exportexcelfile_3)(string, FileFormatType) | Exporte vers un fichier Excel. |
| [GetActiveWorksheet](../../aspose.cells.griddesktop/griddesktop/getactiveworksheet)() | Obtient la feuille de calcul active actuelle. |
| [getHScrollBar](../../aspose.cells.griddesktop/griddesktop/gethscrollbar)() | retourner la barre de défilement horizontale |
| [getVScrollBar](../../aspose.cells.griddesktop/griddesktop/getvscrollbar)() | retour barre de défilement vertical |
| [ImportExcelFile](../../aspose.cells.griddesktop/griddesktop/importexcelfile#importexcelfile)(Stream) | Importations à partir d'un flux de fichiers Excel, y compris le flux de fichiers de disque ou le flux de mémoire. |
| [ImportExcelFile](../../aspose.cells.griddesktop/griddesktop/importexcelfile#importexcelfile_3)(string) | Importe à partir d'un fichier Excel. |
| [ImportExcelFile](../../aspose.cells.griddesktop/griddesktop/importexcelfile#importexcelfile_1)(Stream, bool) | Importations à partir d'un flux de fichiers Excel, y compris le flux de fichiers de disque ou le flux de mémoire. |
| [ImportExcelFile](../../aspose.cells.griddesktop/griddesktop/importexcelfile#importexcelfile_4)(string, bool) | Importe à partir d'un fichier Excel. |
| [ImportExcelFile](../../aspose.cells.griddesktop/griddesktop/importexcelfile#importexcelfile_5)(string, int) | Importe une feuille de calcul à partir d'un fichier Excel. |
| [ImportExcelFile](../../aspose.cells.griddesktop/griddesktop/importexcelfile#importexcelfile_2)(Stream, string, string, bool, bool) | Importe à partir d'un fichier Excel. |
| [ImportExcelFile](../../aspose.cells.griddesktop/griddesktop/importexcelfile#importexcelfile_6)(string, string, string, bool, bool) | Importe à partir d'un fichier Excel. |
| [OpenFindReplaceDialog](../../aspose.cells.griddesktop/griddesktop/openfindreplacedialog)(bool) | Ouvre la boîte de dialogue FindReplace pour rechercher ou remplacer des cellules. |
| [Paste](../../aspose.cells.griddesktop/griddesktop/paste)() | Colle le contenu du presse-papiers dans la cellule ciblée. |
| [RefreshControl](../../aspose.cells.griddesktop/griddesktop/refreshcontrol)() | Actualiser le contrôle GridDesktop. |
| [RunAllFormulas](../../aspose.cells.griddesktop/griddesktop/runallformulas)() | Exécute la formule de toutes les cellules. |
| [SetAllScrollBarsVisible](../../aspose.cells.griddesktop/griddesktop/setallscrollbarsvisible)() | Définit toutes les barres de défilement visibles. |
| [ShowStyleDialog](../../aspose.cells.griddesktop/griddesktop/showstyledialog)() | Ouvre une boîte de dialogue de style, pour définir le style des cellules, la police, les couleurs, etc. |
| [StartFormatPainter](../../aspose.cells.griddesktop/griddesktop/startformatpainter)(bool) | Notifie à GridDesktop de démarrer FormatPainter. |
| [UnDoSplit](../../aspose.cells.griddesktop/griddesktop/undosplit)() | Désactiver la vue fractionnée. |
| static [GetVersion](../../aspose.cells.griddesktop/griddesktop/getversion)() | Obtenez la version finale. |

## Des champs

| Nom | La description |
| --- | --- |
| [LoadDataFilter](../../aspose.cells.griddesktop/griddesktop/loaddatafilter) | les options pour filtrer les données lors du chargement du classeur à partir du modèle. |
| [ShowImportMessage](../../aspose.cells.griddesktop/griddesktop/showimportmessage) | s'il faut afficher la boîte de message en cas d'échec de l'importation du fichier, la valeur par défaut est true |

## Événements

| Nom | La description |
| --- | --- |
| event [AfterDeleteColumns](../../aspose.cells.griddesktop/griddesktop/afterdeletecolumns) | Se produit après la suppression de la colonne. |
| event [AfterDeleteRows](../../aspose.cells.griddesktop/griddesktop/afterdeleterows) | Se produit après la suppression de la ligne. |
| event [AfterInsertColumns](../../aspose.cells.griddesktop/griddesktop/afterinsertcolumns) | Se produit après l'insertion d'une nouvelle colonne. |
| event [AfterInsertRows](../../aspose.cells.griddesktop/griddesktop/afterinsertrows) | Se produit après l'insertion d'une nouvelle ligne. |
| event [BeforeCalculate](../../aspose.cells.griddesktop/griddesktop/beforecalculate) | Se produit avant de calculer la formule dans le classeur. |
| event [BeforeLoadFile](../../aspose.cells.griddesktop/griddesktop/beforeloadfile) | Se produit avant le chargement du classeur à partir du fichier. |
| event [CellButtonClick](../../aspose.cells.griddesktop/griddesktop/cellbuttonclick) | Se produit lorsque le bouton de la cellule est cliqué. |
| event [CellCheckedChanged](../../aspose.cells.griddesktop/griddesktop/cellcheckedchanged) | Se produit lorsque la case à cocher de cellule Propriété cochée est modifiée. |
| event [CellClick](../../aspose.cells.griddesktop/griddesktop/cellclick) | Se produit lorsque la cellule de grille est cliquée. |
| event [CellComboBoxCopy](../../aspose.cells.griddesktop/griddesktop/cellcomboboxcopy) | Se produit lorsqu'une ComboBox de cellule de grille est copiée. |
| event [CellDataChanged](../../aspose.cells.griddesktop/griddesktop/celldatachanged) | Se produit lorsque la propriété de données de cellule de grille est modifiée. |
| event [CellDoubleClick](../../aspose.cells.griddesktop/griddesktop/celldoubleclick) | Se produit lorsque la cellule de grille est double-cliquée. |
| event [CellFormatChanged](../../aspose.cells.griddesktop/griddesktop/cellformatchanged) | Se produit lorsque le format de cellule est modifié via la boîte de dialogue Format de cellule. |
| event [CellKeyPressed](../../aspose.cells.griddesktop/griddesktop/cellkeypressed) | Se produit lorsqu'une touche est enfoncée alors qu'une cellule a le focus. |
| event [CellSelectedIndexChanged](../../aspose.cells.griddesktop/griddesktop/cellselectedindexchanged) | Se produit lorsque la propriété SelectedIndex de la liste déroulante des cellules a changé. |
| event [CellTextBoxChanging](../../aspose.cells.griddesktop/griddesktop/celltextboxchanging) | Se produit lors de la saisie de caractères dans une cellule de la grille. |
| event [CellValidationFailed](../../aspose.cells.griddesktop/griddesktop/cellvalidationfailed) | Se produit lorsque la validation d'une cellule de la grille a échoué. |
| event [ColumnHeaderClick](../../aspose.cells.griddesktop/griddesktop/columnheaderclick) | Se produit lorsque l'en-tête de colonne a cliqué. |
| event [ColumnHeaderDoubleClick](../../aspose.cells.griddesktop/griddesktop/columnheaderdoubleclick) | Se produit lorsque l'en-tête de colonne a double-cliqué. |
| event [CommentDataChanged](../../aspose.cells.griddesktop/griddesktop/commentdatachanged) | Se produit lorsque les données de commentaire ont changé. |
| event [FailLoadFile](../../aspose.cells.griddesktop/griddesktop/failloadfile) |  |
| event [FinishCalculate](../../aspose.cells.griddesktop/griddesktop/finishcalculate) | Se produit après le calcul de la formule dans le classeur. |
| event [FinishLoadFile](../../aspose.cells.griddesktop/griddesktop/finishloadfile) | Se produit lorsque le classeur est chargé. |
| event [FocusedCellChanged](../../aspose.cells.griddesktop/griddesktop/focusedcellchanged) | Se produit lorsque la cellule ciblée est modifiée. |
| event [RowColumnHiddenChanged](../../aspose.cells.griddesktop/griddesktop/rowcolumnhiddenchanged) | Se produit lorsque l'état de masquage des lignes/colonnes a changé. |
| event [RowFilteredEvent](../../aspose.cells.griddesktop/griddesktop/rowfilteredevent) | Se produit après la sélection de l'élément de filtre de ligne. |
| event [RowHeaderClick](../../aspose.cells.griddesktop/griddesktop/rowheaderclick) | Se produit lorsque l'en-tête de ligne a cliqué. |
| event [RowHeaderDoubleClick](../../aspose.cells.griddesktop/griddesktop/rowheaderdoubleclick) | Se produit lorsque l'en-tête de ligne a double-cliqué. |
| event [SelectedCellRangeChanged](../../aspose.cells.griddesktop/griddesktop/selectedcellrangechanged) | Se produit lorsque la plage de cellules sélectionnée est modifiée. |
| event [SelectedSheetIndexChanged](../../aspose.cells.griddesktop/griddesktop/selectedsheetindexchanged) | Se produit lorsque la propriété SelectedSheetIndex est modifiée. |
| event [ShapeClick](../../aspose.cells.griddesktop/griddesktop/shapeclick) | Se produit lorsque la forme est cliqué. |

### Remarques

Veuillez vous référer au document .NET SDK pour plus d'informations sur System.Windows.Forms.UserControl.

### Exemples

```csharp
[C#]
gridDesktop1.Worksheets[0].Cells[0, 0].Value = "2";
gridDesktop1.Worksheets[0].Cells[1, 0].Value = "3";
gridDesktop1.Worksheets[0].Cells[2, 1].Value = "=a1*a2";
gridDesktop1.RunAllFormulas();
gridDesktop1.Invalidate();

[Visual Basic]
gridDesktop1.Worksheets(0).Cells(0, 0).Value = "2"
gridDesktop1.Worksheets(0).Cells(1, 0).Value = "3"
gridDesktop1.Worksheets(0).Cells(2, 1).Value = "=a1*a2"
gridDesktop1.RunAllFormulas()
gridDesktop1.Invalidate()

```

### Voir également

* espace de noms [Aspose.Cells.GridDesktop](../../aspose.cells.griddesktop)
* Assemblée [Aspose.Cells.GridDesktop](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.GridDesktop.dll -->
