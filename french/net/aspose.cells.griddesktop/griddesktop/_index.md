---
title: "Classe GridDesktop"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.GridDesktop.GridDesktop. La classe Aspose GridDesktop représente un objet racine pour créer un contrôle GridDesktop. Pour utiliser ce contrôle, il suffit de le faire glisser depuis votre boîte à outils vers un formulaire ou un contrôle utilisateur"
type: docs
url: /fr/net/aspose.cells.griddesktop/griddesktop/
---
## GridDesktop class

La classe Aspose GridDesktop représente un objet racine pour créer un contrôle GridDesktop. Pour utiliser ce contrôle, il suffit de le faire glisser depuis votre boîte à outils vers un formulaire ou un contrôle utilisateur.

```csharp
public class GridDesktop : UserControl
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [GridDesktop](griddesktop/)() | Classe Aspose GridDesktop |

## Propriétés

| Nom | Description |
| --- | --- |
| [ActiveSheetIndex](../../aspose.cells.griddesktop/griddesktop/activesheetindex/) { get; set; } | Obtient ou définit l'index de la feuille sélectionnée. |
| [ActiveSheetNameFont](../../aspose.cells.griddesktop/griddesktop/activesheetnamefont/) { get; set; } | Obtient ou définit la police d'affichage de la barre de feuille de la feuille active. |
| [AlwasysRecalculateAllFormulas](../../aspose.cells.griddesktop/griddesktop/alwasysrecalculateallformulas/) { get; set; } | Obtient ou définit une valeur indiquant si nous devons exécuter toutes les formules, comme lorsque nous exécutons toutes les formules, lorsqu'une valeur de cellule est mise à jour et qu'elle affecte d'autres cellules, qui à leur tour affectent d'autres cellules, etc., entraînant le recalcul de toutes les cellules, à l'instar de l'effet papillon. Cela nécessite de nombreuses opérations de pile, ce qui entraîne de très faibles performances, comme dans CELLSNET-41921. Ce problème contient le fichier qui illustre ce scénario ; il vaut mieux simplement exécuter toutes les formules, car lorsque toutes les formules sont exécutées nous pouvons avoir certaines optimisations. |
| [BorderStyle](../../aspose.cells.griddesktop/griddesktop/borderstyle/) { get; set; } | Indique le style de bordure du contrôle. |
| [ColumnHeaderVisible](../../aspose.cells.griddesktop/griddesktop/columnheadervisible/) { get; set; } | Obtient ou définit une valeur indiquant si l'en-tête de colonne est visible. |
| [CommentDisplayingFont](../../aspose.cells.griddesktop/griddesktop/commentdisplayingfont/) { get; set; } | Obtient ou définit la police d'affichage par défaut du texte des commentaires. |
| [ContextMenuManager](../../aspose.cells.griddesktop/griddesktop/contextmenumanager/) { get; } | Obtient l'instance de ContextMenuManager. |
| [DefaultCellFont](../../aspose.cells.griddesktop/griddesktop/defaultcellfont/) { get; set; } | Obtient ou définit la police par défaut de la cellule |
| [DefaultCellFontColor](../../aspose.cells.griddesktop/griddesktop/defaultcellfontcolor/) { get; set; } | Obtient ou définit la couleur de police par défaut de la cellule. |
| [EnableClipboardCopyPaste](../../aspose.cells.griddesktop/griddesktop/enableclipboardcopypaste/) { get; set; } | Indique s'il faut copier/coller en se basant sur le presse‑papier, afin de pouvoir copier/coller avec MS‑EXCEL. Cela ne copie/colle que la valeur de la cellule ; cela ne copie aucun autre paramètre de la cellule comme le format, le style de bordure, etc. La valeur par défaut est false. |
| [EnableCopyWithExtension](../../aspose.cells.griddesktop/griddesktop/enablecopywithextension/) { get; set; } | Obtient ou définit une valeur indiquant si l'opération de copie étendra le nombre de lignes ou de colonnes. |
| [EnableCopyWithLockedOption](../../aspose.cells.griddesktop/griddesktop/enablecopywithlockedoption/) { get; set; } | Obtient ou définit une valeur indiquant si l'opération de copie copiera la valeur de l'attribut CellLocked du style d'une cellule. |
| [EnableUndo](../../aspose.cells.griddesktop/griddesktop/enableundo/) { get; set; } | Obtient ou définit une valeur indiquant si la fonction Undo est activée. La valeur par défaut est false. |
| [GridMemorySetting](../../aspose.cells.griddesktop/griddesktop/gridmemorysetting/) { get; set; } | Obtient ou définit l'option de mémoire, la valeur par défaut est GridMemorySetting.Normal |
| [IsHorizontalScrollBarVisible](../../aspose.cells.griddesktop/griddesktop/ishorizontalscrollbarvisible/) { get; set; } | Définit l'état de visibilité pour la barre de défilement horizontale. |
| [IsVerticalScrollBarVisible](../../aspose.cells.griddesktop/griddesktop/isverticalscrollbarvisible/) { get; set; } | Définit l'état de visibilité pour la barre de défilement verticale. |
| [Names](../../aspose.cells.griddesktop/griddesktop/names/) { get; } | Obtient la collection de tous les objets Name dans le classeur. |
| [PageRows](../../aspose.cells.griddesktop/griddesktop/pagerows/) { get; set; } | Définit ou obtient la taille de ligne pour la pagination. Le maximum de PageRows pris en charge est 100000, le nombre maximal de pages pris en charge est 5000. |
| [PasteType](../../aspose.cells.griddesktop/griddesktop/pastetype/) { get; set; } | Indique le type de collage à utiliser lors de l'action de collage, disponible uniquement lorsque EnableClipboardCopyPaste est false. La valeur par défaut est GridPasteType.Default ; |
| [R1C1](../../aspose.cells.griddesktop/griddesktop/r1c1/) { get; set; } | Obtient ou définit une valeur indiquant si le contrôle utilise le style de référence R1C1. |
| [RecalculateFormulas](../../aspose.cells.griddesktop/griddesktop/recalculateformulas/) { get; set; } | Obtient ou définit une valeur indiquant s'il faut recalculer toutes les formules des cellules lorsqu'une valeur de cellule change. La valeur par défaut est true. |
| [RowHeaderVisible](../../aspose.cells.griddesktop/griddesktop/rowheadervisible/) { get; set; } | Obtient ou définit une valeur indiquant si l'en-tête de ligne est visible. |
| [SheetNameFont](../../aspose.cells.griddesktop/griddesktop/sheetnamefont/) { get; set; } | Obtient ou définit la police d'affichage par défaut de la barre de feuilles. |
| [SheetsBarVisible](../../aspose.cells.griddesktop/griddesktop/sheetsbarvisible/) { get; set; } | Obtient ou définit une valeur indiquant si la barre de feuilles est visible. |
| [SheetTabWidth](../../aspose.cells.griddesktop/griddesktop/sheettabwidth/) { get; set; } | Définit / obtient la largeur de l'onglet de feuille. |
| [ShowContextMenu](../../aspose.cells.griddesktop/griddesktop/showcontextmenu/) { get; set; } | Obtient ou définit une valeur indiquant si le contrôle peut afficher le menu contextuel. |
| [ShowFormulaWarning](../../aspose.cells.griddesktop/griddesktop/showformulawarning/) { get; set; } | Définit / obtient si le message d'erreur ou d'avertissement doit être affiché pour la valeur de formule de cellule définie, la valeur par défaut est true. |
| [ShowNumberStoredAsTextSymbol](../../aspose.cells.griddesktop/griddesktop/shownumberstoredastextsymbol/) { get; set; } | Définit / obtient si le symbole triangle doit être affiché pour la cellule contenant une chaîne numérique mais stockée au format texte. |
| [ShowStatus](../../aspose.cells.griddesktop/griddesktop/showstatus/) { get; set; } | Obtient ou définit une valeur indiquant s'il faut afficher l'état de calcul. La valeur par défaut est true. |
| [UndoManager](../../aspose.cells.griddesktop/griddesktop/undomanager/) { get; } | Obtient l'instance UndoManager. |
| [Worksheets](../../aspose.cells.griddesktop/griddesktop/worksheets/) { get; } | Obtient les feuilles de calcul. |

## Méthodes

| Nom | Description |
| --- | --- |
| [Clear](../../aspose.cells.griddesktop/griddesktop/clear/)() | Efface le contrôle GridDesktop. |
| [Copy](../../aspose.cells.griddesktop/griddesktop/copy/)() | Copie le contenu de la cellule focalisée dans le presse‑papier. |
| [Cut](../../aspose.cells.griddesktop/griddesktop/cut/)() | Coupe le contenu de la cellule focalisée dans le presse‑papier. |
| [DoSplit](../../aspose.cells.griddesktop/griddesktop/dosplit/)() | Définit la vue fractionnée. |
| [EndFormatPainter](../../aspose.cells.griddesktop/griddesktop/endformatpainter/)() | Notifie GridDesktop de terminer le FormatPainter. |
| [ExportExcelFile](../../aspose.cells.griddesktop/griddesktop/exportexcelfile/#exportexcelfile)(Stream) | Exporte vers un flux de fichier Excel, incluant le flux d'E/S disque ou le flux mémoire. |
| [ExportExcelFile](../../aspose.cells.griddesktop/griddesktop/exportexcelfile/#exportexcelfile_2)(string) | Exporte vers un fichier Excel. |
| [ExportExcelFile](../../aspose.cells.griddesktop/griddesktop/exportexcelfile/#exportexcelfile_1)(Stream, FileFormatType) | Exporte vers un flux de fichier Excel, incluant le flux d'E/S disque ou le flux mémoire. |
| [ExportExcelFile](../../aspose.cells.griddesktop/griddesktop/exportexcelfile/#exportexcelfile_3)(string, FileFormatType) | Exporte vers un fichier Excel. |
| [ExportPdfFile](../../aspose.cells.griddesktop/griddesktop/exportpdffile/#exportpdffile)(Stream, GridPdfSaveOptions) | Exporte vers un flux de fichier PDF, incluant le flux d'E/S disque ou le flux mémoire. |
| [ExportPdfFile](../../aspose.cells.griddesktop/griddesktop/exportpdffile/#exportpdffile_1)(string, GridPdfSaveOptions) | Exporte vers un flux de fichier PDF, incluant le flux d'E/S disque ou le flux mémoire. |
| [GetActiveWorksheet](../../aspose.cells.griddesktop/griddesktop/getactiveworksheet/)() | Obtient la feuille de calcul active actuelle. |
| [getHScrollBar](../../aspose.cells.griddesktop/griddesktop/gethscrollbar/)() | renvoie la barre de défilement horizontale |
| [getVScrollBar](../../aspose.cells.griddesktop/griddesktop/getvscrollbar/)() | renvoie la barre de défilement verticale |
| [ImportExcelFile](../../aspose.cells.griddesktop/griddesktop/importexcelfile/#importexcelfile)(Stream) | Importe depuis un flux de fichier Excel, y compris un flux de fichier disque ou un flux mémoire. |
| [ImportExcelFile](../../aspose.cells.griddesktop/griddesktop/importexcelfile/#importexcelfile_3)(string) | Importe depuis un fichier Excel. |
| [ImportExcelFile](../../aspose.cells.griddesktop/griddesktop/importexcelfile/#importexcelfile_1)(Stream, bool) | Importe depuis un flux de fichier Excel, y compris un flux de fichier disque ou un flux mémoire. |
| [ImportExcelFile](../../aspose.cells.griddesktop/griddesktop/importexcelfile/#importexcelfile_4)(string, bool) | Importe depuis un fichier Excel. |
| [ImportExcelFile](../../aspose.cells.griddesktop/griddesktop/importexcelfile/#importexcelfile_5)(string, int) | Importe une feuille de calcul depuis un fichier Excel. |
| [ImportExcelFile](../../aspose.cells.griddesktop/griddesktop/importexcelfile/#importexcelfile_2)(Stream, string, string, bool, bool) | Importe depuis un fichier Excel. |
| [ImportExcelFile](../../aspose.cells.griddesktop/griddesktop/importexcelfile/#importexcelfile_6)(string, string, string, bool, bool) | Importe depuis un fichier Excel. |
| [Invalidate](../../aspose.cells.griddesktop/griddesktop/invalidate/#invalidate)() | Remplacer l'invalidation. |
| [OpenFindReplaceDialog](../../aspose.cells.griddesktop/griddesktop/openfindreplacedialog/)(bool) | Ouvre la boîte de dialogue RechercherRemplacer pour trouver ou remplacer des cellules. |
| [Paste](../../aspose.cells.griddesktop/griddesktop/paste/)() | Colle le contenu du presse-papiers dans la cellule ciblée. |
| [RefreshControl](../../aspose.cells.griddesktop/griddesktop/refreshcontrol/)() | Actualise le contrôle GridDesktop. |
| [RunAllFormulas](../../aspose.cells.griddesktop/griddesktop/runallformulas/)() | Exécute les formules de toutes les cellules. |
| [SetAllScrollBarsVisible](../../aspose.cells.griddesktop/griddesktop/setallscrollbarsvisible/)() | Rend toutes les barres de défilement visibles. |
| [SetCustomResourceManager](../../aspose.cells.griddesktop/griddesktop/setcustomresourcemanager/)(ResourceManager) | Définir un gestionnaire de ressources personnalisé pour implémenter la localisation définie par l'utilisateur |
| [ShowStyleDialog](../../aspose.cells.griddesktop/griddesktop/showstyledialog/)() | Ouvre une boîte de dialogue de style, pour définir le style, la police, les couleurs des cellules, etc. |
| [StartFormatPainter](../../aspose.cells.griddesktop/griddesktop/startformatpainter/)(bool) | Notifie GridDesktop de démarrer le FormatPainter. |
| [UnDoSplit](../../aspose.cells.griddesktop/griddesktop/undosplit/)() | Désactiver la vue fractionnée. |
| static [GetVersion](../../aspose.cells.griddesktop/griddesktop/getversion/)() | Obtient la version de publication. |

## Champs

| Nom | Description |
| --- | --- |
| [LoadDataFilter](../../aspose.cells.griddesktop/griddesktop/loaddatafilter/) | les options pour filtrer les données lors du chargement du classeur depuis un modèle. |
| [ShowImportMessage](../../aspose.cells.griddesktop/griddesktop/showimportmessage/) | détermine s'il faut afficher une boîte de dialogue lorsqu'il échoue à importer le fichier, la valeur par défaut est vraie |

## Événements

| Nom | Description |
| --- | --- |
| event [AfterDeleteColumns](../../aspose.cells.griddesktop/griddesktop/afterdeletecolumns/) | Se produit après la suppression d'une colonne. |
| event [AfterDeleteRows](../../aspose.cells.griddesktop/griddesktop/afterdeleterows/) | Se produit après la suppression d'une ligne. |
| event [AfterInsertColumns](../../aspose.cells.griddesktop/griddesktop/afterinsertcolumns/) | Se produit après l'insertion d'une nouvelle colonne. |
| event [AfterInsertRows](../../aspose.cells.griddesktop/griddesktop/afterinsertrows/) | Se produit après l'insertion d'une nouvelle ligne. |
| event [BeforeCalculate](../../aspose.cells.griddesktop/griddesktop/beforecalculate/) | Se produit avant le calcul de la formule dans le classeur. |
| event [BeforeLoadFile](../../aspose.cells.griddesktop/griddesktop/beforeloadfile/) | Se produit avant le chargement du classeur depuis le fichier. |
| event [CellButtonClick](../../aspose.cells.griddesktop/griddesktop/cellbuttonclick/) | Se produit lorsque le bouton de la cellule est cliqué. |
| event [CellCheckedChanged](../../aspose.cells.griddesktop/griddesktop/cellcheckedchanged/) | Se produit lorsque la propriété Checked de la case à cocher de la cellule est modifiée. |
| event [CellClick](../../aspose.cells.griddesktop/griddesktop/cellclick/) | Se produit lorsque le gridcell est cliqué. |
| event [CellComboBoxCopy](../../aspose.cells.griddesktop/griddesktop/cellcomboboxcopy/) | Se produit lorsqu'une ComboBox de cellule de grille est copiée. |
| event [CellDataChanged](../../aspose.cells.griddesktop/griddesktop/celldatachanged/) | Se produit lorsque la propriété de données de la cellule de la grille est modifiée. |
| event [CellDoubleClick](../../aspose.cells.griddesktop/griddesktop/celldoubleclick/) | Se produit lorsque le gridcell est double-cliqué. |
| event [CellFormatChanged](../../aspose.cells.griddesktop/griddesktop/cellformatchanged/) | Se produit lorsque le format de la cellule est modifié via la boîte de dialogue Format de cellules. |
| event [CellKeyPressed](../../aspose.cells.griddesktop/griddesktop/cellkeypressed/) | Se produit lorsqu'une touche est enfoncée alors qu'une cellule a le focus. |
| event [CellSelectedIndexChanged](../../aspose.cells.griddesktop/griddesktop/cellselectedindexchanged/) | Se produit lorsque la propriété SelectedIndex de la combobox de cellule a changé. |
| event [CellTextBoxChanging](../../aspose.cells.griddesktop/griddesktop/celltextboxchanging/) | Se produit lors de la saisie de caractères dans une cellule de grille. |
| event [CellValidationFailed](../../aspose.cells.griddesktop/griddesktop/cellvalidationfailed/) | Se produit lorsqu'une validation de cellule de grille échoue. |
| event [ColumnHeaderClick](../../aspose.cells.griddesktop/griddesktop/columnheaderclick/) | Se produit lorsque l'en-tête de colonne est cliqué. |
| event [ColumnHeaderDoubleClick](../../aspose.cells.griddesktop/griddesktop/columnheaderdoubleclick/) | Se produit lorsque l'en-tête de colonne est double-cliqué. |
| event [CommentDataChanged](../../aspose.cells.griddesktop/griddesktop/commentdatachanged/) | Se produit lorsque les données du commentaire ont changé. |
| event [FailLoadFile](../../aspose.cells.griddesktop/griddesktop/failloadfile/) |  |
| event [FinishCalculate](../../aspose.cells.griddesktop/griddesktop/finishcalculate/) | Se produit après le calcul de la formule dans le classeur. |
| event [FinishLoadFile](../../aspose.cells.griddesktop/griddesktop/finishloadfile/) | Se produit lorsque le classeur est chargé. |
| event [FocusedCellChanged](../../aspose.cells.griddesktop/griddesktop/focusedcellchanged/) | Se produit lorsque la cellule focalisée est modifiée. |
| event [PictureClick](../../aspose.cells.griddesktop/griddesktop/pictureclick/) | Se produit lorsque la forme est cliquée. |
| event [RowColumnHiddenChanged](../../aspose.cells.griddesktop/griddesktop/rowcolumnhiddenchanged/) | Se produit lorsque l'état de masquage de la ligne/colonne a changé. |
| event [RowFilteredEvent](../../aspose.cells.griddesktop/griddesktop/rowfilteredevent/) | Se produit après la sélection d'un élément de filtre de ligne. |
| event [RowHeaderClick](../../aspose.cells.griddesktop/griddesktop/rowheaderclick/) | Se produit lorsque l'en-tête de ligne est cliqué. |
| event [RowHeaderDoubleClick](../../aspose.cells.griddesktop/griddesktop/rowheaderdoubleclick/) | Se produit lorsque l'en-tête de ligne est double-cliqué. |
| event [SelectedCellRangeChanged](../../aspose.cells.griddesktop/griddesktop/selectedcellrangechanged/) | Se produit lorsque la plage de cellules sélectionnée est modifiée. |
| event [SelectedSheetIndexChanged](../../aspose.cells.griddesktop/griddesktop/selectedsheetindexchanged/) | Se produit lorsque la propriété SelectedSheetIndex est modifiée. |
| event [ShapeClick](../../aspose.cells.griddesktop/griddesktop/shapeclick/) | Se produit lorsque la forme est cliquée. |

### Remarques

Veuillez vous référer à la documentation du SDK .NET pour plus d'informations sur System.Windows.Forms.UserControl.

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

### Voir aussi

* namespace [Aspose.Cells.GridDesktop](../../aspose.cells.griddesktop/)
* assembly [Aspose.Cells.GridDesktop](../../)


