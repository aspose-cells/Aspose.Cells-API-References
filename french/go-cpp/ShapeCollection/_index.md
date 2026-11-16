---
title: "Classe ShapeCollection"
linktitle: "ShapeCollection"
second_title: "Référence API C++ d'Aspose.Cells pour Go"
description: "Classe ShapeCollection. Encapsule l'objet qui représente shapecollection en Go."
type: docs
weight: 200
url: /fr/go-cpp/shapecollection/
---

## ShapeCollection class

Représente toutes les formes dans une feuille de calcul/graphique.

```go

type ShapeCollection struct  {
	ptr unsafe.Pointer
}

```
## Constructeurs

| Méthode | Description |
| --- | --- |

## Méthodes

| Méthode | Description |
| --- | --- |
| [IsNull](./isnull/) | Vérifie si l'objet d'implémentation est nullptr. |
| [Get_Int](./get_int/) | Récupère l'objet Shape à l'index spécifique dans la liste. |
| [Get_String](./get_string/) | Récupère l'objet Shape par le nom de la forme. |
| [AddCopy_Shape_Int_Int_Int_Int](./addcopy_shape_int_int_int_int/) | Ajoute et copie une forme dans le worksheet. |
| [AddCopy_Shape_Int_Int_Int_Int_CopyOptions](./addcopy_shape_int_int_int_int_copyoptions/) | Ajoute et copie une forme dans le worksheet. |
| [AddCheckBox](./addcheckbox/) | Ajoute une case à cocher dans le worksheet. |
| [AddTextBox](./addtextbox/) | Ajoute une zone de texte dans le worksheet. |
| [AddEquation](./addequation/) | Ajoute un objet équation dans le worksheet. |
| [AddLaTeXEquation](./addlatexequation/) | Ajoute un objet équation à la feuille de calcul en utilisant des chaînes au format LaTeX. |
| [AddSpinner](./addspinner/) | Ajoute un Spinner à la feuille de calcul. |
| [AddScrollBar](./addscrollbar/) | Ajoute un ScrollBar à la feuille de calcul. |
| [AddRadioButton](./addradiobutton/) | Ajoute un RadioButton à la feuille de calcul. |
| [AddListBox](./addlistbox/) | Ajoute un ListBox à la feuille de calcul. |
| [AddComboBox](./addcombobox/) | Ajoute un ComboBox à la feuille de calcul. |
| [AddGroupBox](./addgroupbox/) | Ajoute un GroupBox à la feuille de calcul. |
| [AddButton](./addbutton/) | Ajoute un Button à la feuille de calcul. |
| [AddLabel](./addlabel/) | Ajoute un Label à la feuille de calcul. |
| [AddLabelInChart](./addlabelinchart/) | Ajoute un label au graphique. |
| [AddTextBoxInChart](./addtextboxinchart/) | Ajoute une zone de texte au graphique. |
| [AddTextEffectInChart](./addtexteffectinchart/) | Insère un objet WordArt au graphique |
| [AddTextEffect](./addtexteffect/) | Insère un objet WordArt. |
| [AddWordArt](./addwordart/) | Ajoute un WordArt prédéfini depuis Excel 2007.s |
| [AddRectangle](./addrectangle/) | Ajoute un RectangleShape à la feuille de calcul. |
| [AddOval](./addoval/) | Ajoute un Oval à la feuille de calcul. |
| [AddLine](./addline/) | Ajoute un LineShape à la feuille de calcul. |
| [AddFreeFloatingShape](./addfreefloatingshape/) | Ajoute une forme flottante libre à la feuille de calcul.S'applique uniquement aux formes ligne/image. |
| [AddShapeInChart_MsoDrawingType_PlacementType_Int_Int_Int_Int_Stream](./addshapeinchart_msodrawingtype_placementtype_int_int_int_int_stream/) | Ajoute une forme au graphique .Toutes les unités sont 1/4000 de la zone du graphique. |
| [AddShapeInChart_MsoDrawingType_PlacementType_Int_Int_Int_Int](./addshapeinchart_msodrawingtype_placementtype_int_int_int_int/) | Ajoute une forme au graphique .Toutes les unités sont 1/4000 de la zone du graphique. |
| [AddShapeInChartByScale_MsoDrawingType_PlacementType_Double_Double_Double_Double](./addshapeinchartbyscale_msodrawingtype_placementtype_double_double_double_double/) | Ajoute une forme au graphique. Toutes les unités sont exprimées en pourcentage de la zone du graphique. |
| [AddShapeInChartByScale_MsoDrawingType_PlacementType_Double_Double_Double_Double_Stream](./addshapeinchartbyscale_msodrawingtype_placementtype_double_double_double_double_stream/) | Ajoute une forme au graphique .Toutes les unités sont 1/4000 de la zone du graphique. |
| [AddArc](./addarc/) | Ajoute un ArcShape à la feuille de calcul. |
| [AddShape](./addshape/) | Ajoute un Shape à la feuille de calcul. |
| [AddAutoShape](./addautoshape/) | Ajoute un AutoShape à la feuille de calcul. |
| [AddAutoShapeInChart](./addautoshapeinchart/) | Ajoute un AutoShape au graphique. |
| [AddActiveXControl](./addactivexcontrol/) | Crée un Contrôle Activex. |
| [AddPicture_Int_Int_Int_Int_Stream](./addpicture_int_int_int_int_stream/) | Ajoute une image à la collection. |
| [AddPicture_Int_Int_Stream_Int_Int](./addpicture_int_int_stream_int_int/) | Ajoute une image à la collection. |
| [AddSvg](./addsvg/) | Ajoute une image svg. |
| [AddIcons](./addicons/) | Ajoute une image svg. |
| [AddLinkedPicture](./addlinkedpicture/) | Ajoutez une image liée. |
| [AddOleObjectWithLinkedImage](./addoleobjectwithlinkedimage/) | Ajoutez une image liée. |
| [AddPictureInChart](./addpictureinchart/) | Ajoute une image au graphique. |
| [AddOleObject](./addoleobject/) | Ajoute un OleObject. |
| [CopyCommentsInRange](./copycommentsinrange/) | Copiez tous les commentaires dans la plage. |
| [CopyInRange](./copyinrange/) | Copiez les formes de la plage vers la plage de destination. |
| [DeleteInRange](./deleteinrange/) | Supprimez les formes dans la plage. Les formes de commentaire ne seront pas supprimées. |
| [DeleteShape](./deleteshape/) | Supprimez une forme. Si la forme se trouve dans le groupe ou est une forme de commentaire, elle ne sera pas supprimée. |
| [Group](./group/) | Regroupez les formes. |
| [Ungroup](./ungroup/) | Dégroupez les éléments de forme. |
| [RemoveAt](./removeat/) | Supprimez la forme. |
| [Remove](./remove/) | Supprimez la forme. |
| [Clear](./clear/) | Effacez toutes les formes dans la feuille de calcul. |
| [UpdateSelectedValue](./updateselectedvalue/) | Mettez à jour la valeur sélectionnée avec la valeur de la cellule liée ou de la plage de la forme. |
| [AddFreeform](./addfreeform/) | Ajoute une forme libre à la feuille de calcul. |
| [AddSignatureLine](./addsignatureline/) | Ajoute une ligne de signature à la feuille de calcul. |
| [GetCount](./getcount/) | Obtient le nombre d'éléments contenus dans l'instance. |
