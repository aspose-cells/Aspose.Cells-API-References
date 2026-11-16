---
title: "Classe ScrollBar"
linktitle: "ScrollBar"
second_title: "Référence API C++ d'Aspose.Cells pour Go"
description: "ScrollBar class. Encapsule l'objet qui représente scrollbar en Go."
type: docs
weight: 200
url: /fr/go-cpp/scrollbar/
---

## ScrollBar class

Représente un objet de barre de défilement.

```go

type ScrollBar struct  {
	ptr unsafe.Pointer
}

```
## Constructeurs

| Méthode | Description |
| --- | --- |
| [NewScrollBar](./newscrollbar/) | Construit à partir d'un objet parent. |

## Méthodes

| Méthode | Description |
| --- | --- |
| [IsNull](./isnull/) | Vérifie si l'objet d'implémentation est nullptr. |
| [GetCurrentValue](./getcurrentvalue/) | Obtient ou définit la valeur actuelle. |
| [SetCurrentValue](./setcurrentvalue/) | Obtient ou définit la valeur actuelle. |
| [GetMin](./getmin/) | Obtient ou définit la valeur minimale d'une barre de défilement ou d'une plage de spinner. |
| [SetMin](./setmin/) | Obtient ou définit la valeur minimale d'une barre de défilement ou d'une plage de spinner. |
| [GetMax](./getmax/) | Obtient ou définit la valeur maximale d'une barre de défilement ou d'une plage de spinner. |
| [SetMax](./setmax/) | Obtient ou définit la valeur maximale d'une barre de défilement ou d'une plage de spinner. |
| [GetIncrementalChange](./getincrementalchange/) | Obtient ou définit la quantité d'incrémentation d'une ligne pour la barre de défilement ou le spinner. |
| [SetIncrementalChange](./setincrementalchange/) | Obtient ou définit la quantité d'incrémentation d'une ligne pour la barre de défilement ou le spinner. |
| [GetPageChange](./getpagechange/) | Obtient ou définit le changement de page |
| [SetPageChange](./setpagechange/) | Obtient ou définit le changement de page |
| [GetShadow](./getshadow/) | Indique si la forme possède un ombrage 3D. |
| [SetShadow](./setshadow/) | Indique si la forme possède un ombrage 3D. |
| [IsHorizontal](./ishorizontal/) | Indique s'il s'agit d'une barre de défilement horizontale. |
| [SetIsHorizontal](./setishorizontal/) | Indique s'il s'agit d'une barre de défilement horizontale. |
| [GetMacroName](./getmacroname/) | Obtient et définit le nom de la macro. |
| [SetMacroName](./setmacroname/) | Obtient et définit le nom de la macro. |
| [IsEquation](./isequation/) | Indique si la forme ne contient qu'une équation. |
| [IsSmartArt](./issmartart/) | Indique si la forme est un SmartArt. |
| [ToFrontOrBack](./tofrontorback/) | Place la forme au premier plan ou l'envoie à l'arrière-plan. |
| [GetZOrderPosition](./getzorderposition/) | Renvoie la position d'une forme dans l'ordre Z. |
| [SetZOrderPosition](./setzorderposition/) | Renvoie la position d'une forme dans l'ordre Z. |
| [GetName](./getname/) | Obtient et définit le nom de la forme. |
| [SetName](./setname/) | Obtient et définit le nom de la forme. |
| [GetAlternativeText](./getalternativetext/) | Renvoie ou définit la chaîne de texte descriptive (alternative) de l'objet Shape. |
| [SetAlternativeText](./setalternativetext/) | Renvoie ou définit la chaîne de texte descriptive (alternative) de l'objet Shape. |
| [GetTitle](./gettitle/) | Spécifie le titre (légende) de l'objet forme actuel. |
| [SetTitle](./settitle/) | Spécifie le titre (légende) de l'objet forme actuel. |
| [GetLine](./getline/) | Obtient le style de ligne |
| [GetFill](./getfill/) | Renvoie un objet FillFormat qui contient les propriétés de formatage de remplissage pour la forme spécifiée. |
| [GetShadowEffect](./getshadoweffect/) | Représente un objet Drawing.ShadowEffect qui spécifie l'effet d'ombre pour l'élément de graphique ou la forme. |
| [GetReflection](./getreflection/) | Représente un objet ReflectionEffect qui spécifie l'effet de réflexion pour l'élément de graphique ou la forme. |
| [GetGlow](./getglow/) | Représente un objet GlowEffect qui spécifie l'effet de lueur pour l'élément de graphique ou la forme. |
| [GetSoftEdges](./getsoftedges/) | Obtient et définit le rayon du flou à appliquer aux bords, en points. |
| [SetSoftEdges](./setsoftedges/) | Obtient et définit le rayon du flou à appliquer aux bords, en points. |
| [GetThreeDFormat](./getthreedformat/) | Obtient et définit le format 3D de la forme. |
| [GetFormatPicture](./getformatpicture/) | Obtient et définit les options du format d'image. |
| [IsHidden](./ishidden/) | Indique si l'objet est visible. |
| [SetIsHidden](./setishidden/) | Indique si l'objet est visible. |
| [IsAspectRatioLocked](./isaspectratiolocked/) | Vrai signifie que le rapport d'aspect de la forme est verrouillé. |
| [SetIsAspectRatioLocked](./setisaspectratiolocked/) | Vrai signifie que le rapport d'aspect de la forme est verrouillé. |
| [GetLockedProperty](./getlockedproperty/) | Obtient la valeur de la propriété locked. |
| [SetLockedProperty](./setlockedproperty/) | Définit la propriété locked. |
| [GetRotationAngle](./getrotationangle/) | Obtient et définit la rotation de la forme. |
| [SetRotationAngle](./setrotationangle/) | Obtient et définit la rotation de la forme. |
| [AddHyperlink](./addhyperlink/) | Ajoute un hyperlien à la forme. |
| [RemoveHyperlink](./removehyperlink/) | Supprime l'hyperlien de la forme. |
| [GetHyperlink](./gethyperlink/) | Obtient l'hyperlien de la forme. |
| [MoveToRange](./movetorange/) | Déplace la forme vers une plage spécifiée. |
| [AlignTopRightCorner](./aligntoprightcorner/) | Déplace l'image vers le coin supérieur droit. |
| [GetId](./getid/) | Obtient l'identifiant de cette forme. |
| [GetSpid](./getspid/) | Spécifie un identifiant de chaîne facultatif qu'une application peut utiliser pour identifier la forme particulière. |
| [GetSpt](./getspt/) | Spécifie un nombre facultatif qu'une application peut utiliser pour associer la forme particulière à un type de forme défini. |
| [GetWorksheet](./getworksheet/) | Obtient l'objet Aspose.Cells.Worksheet qui contient cette forme. |
| [IsGroup](./isgroup/) | Indique si cette forme est une forme groupée. |
| [IsInGroup](./isingroup/) | Indique si la forme est groupée. |
| [IsWordArt](./iswordart/) | Indique si cette forme est un WordArt. |
| [GetTextEffect](./gettexteffect/) | Renvoie un objet TextEffectFormat qui contient les propriétés de mise en forme d'effet de texte pour la forme spécifiée. S'applique aux objets Shape qui représentent WordArt. |
| [IsLocked](./islocked/) | Vrai signifie que l'objet ne peut pas être modifié lorsque la feuille est protégée. Notez que cette valeur n'est pertinente que si la feuille de calcul ou les objets de la feuille de calcul sont protégés. |
| [SetIsLocked](./setislocked/) | Vrai signifie que l'objet ne peut pas être modifié lorsque la feuille est protégée. Notez que cette valeur n'est pertinente que si la feuille de calcul ou les objets de la feuille de calcul sont protégés. |
| [IsPrintable](./isprintable/) | Indique si l'objet est imprimable. Si False, cette forme ne sera pas imprimée lors de l'impression. |
| [SetIsPrintable](./setisprintable/) | Indique si l'objet est imprimable. Si False, cette forme ne sera pas imprimée lors de l'impression. |
| [GetMsoDrawingType](./getmsodrawingtype/) | Obtient le type de dessin. |
| [GetAutoShapeType](./getautoshapetype/) | Obtient et définit le type de forme automatique. |
| [SetAutoShapeType](./setautoshapetype/) | Obtient et définit le type de forme automatique. |
| [GetAnchorType](./getanchortype/) | Obtient et définit le type de l'espace réservé d'ancrage de la forme. |
| [SetAnchorType](./setanchortype/) | Obtient et définit le type de l'espace réservé d'ancrage de la forme. |
| [GetPlacement](./getplacement/) | Représente la façon dont l'objet de dessin est attaché aux cellules en dessous. La propriété contrôle le placement d'un objet sur une feuille de calcul. |
| [SetPlacement](./setplacement/) | Représente la façon dont l'objet de dessin est attaché aux cellules en dessous. La propriété contrôle le placement d'un objet sur une feuille de calcul. |
| [GetUpperLeftRow](./getupperleftrow/) | Représente l'index de la ligne supérieure. |
| [SetUpperLeftRow](./setupperleftrow/) | Représente l'index de la ligne supérieure. |
| [GetUpperDeltaY](./getupperdeltay/) | Obtient ou définit le décalage vertical de la forme à partir de la ligne de son coin supérieur gauche. |
| [SetUpperDeltaY](./setupperdeltay/) | Obtient ou définit le décalage vertical de la forme à partir de la ligne de son coin supérieur gauche. |
| [GetUpperLeftColumn](./getupperleftcolumn/) | Représente l'index de la colonne du coin supérieur gauche. |
| [SetUpperLeftColumn](./setupperleftcolumn/) | Représente l'index de la colonne du coin supérieur gauche. |
| [GetUpperDeltaX](./getupperdeltax/) | Obtient ou définit le décalage horizontal de la forme à partir de la colonne de son coin supérieur gauche. |
| [SetUpperDeltaX](./setupperdeltax/) | Obtient ou définit le décalage horizontal de la forme à partir de la colonne de son coin supérieur gauche. |
| [GetLowerRightRow](./getlowerrightrow/) | Représente l'index de la ligne du coin inférieur droit. |
| [SetLowerRightRow](./setlowerrightrow/) | Représente l'index de la ligne du coin inférieur droit. |
| [GetLowerDeltaY](./getlowerdeltay/) | Obtient ou définit le décalage vertical de la forme à partir de la ligne de son coin inférieur droit. |
| [SetLowerDeltaY](./setlowerdeltay/) | Obtient ou définit le décalage vertical de la forme à partir de la ligne de son coin inférieur droit. |
| [GetLowerRightColumn](./getlowerrightcolumn/) | Représente l'index de la colonne du coin inférieur droit. |
| [SetLowerRightColumn](./setlowerrightcolumn/) | Représente l'index de la colonne du coin inférieur droit. |
| [GetLowerDeltaX](./getlowerdeltax/) | Obtient ou définit le décalage horizontal de la forme à partir de la colonne de son coin inférieur droit. |
| [SetLowerDeltaX](./setlowerdeltax/) | Obtient ou définit le décalage horizontal de la forme à partir de la colonne de son coin inférieur droit. |
| [GetRight](./getright/) | Représente la largeur du décalage horizontal de la forme à partir de la colonne de son coin inférieur droit, en pixels. |
| [SetRight](./setright/) | Représente la largeur du décalage horizontal de la forme à partir de la colonne de son coin inférieur droit, en pixels. |
| [GetBottom](./getbottom/) | Représente la largeur du décalage vertical de la forme à partir de la ligne de son coin inférieur, en pixels. |
| [SetBottom](./setbottom/) | Représente la largeur du décalage vertical de la forme à partir de la ligne de son coin inférieur, en pixels. |
| [GetWidth](./getwidth/) | Représente la largeur de la forme, en pixels. |
| [SetWidth](./setwidth/) | Représente la largeur de la forme, en pixels. |
| [GetWidthInch](./getwidthinch/) | Représente la largeur de la forme, en pouces. |
| [SetWidthInch](./setwidthinch/) | Représente la largeur de la forme, en pouces. |
| [GetWidthPt](./getwidthpt/) | Représente la largeur de la forme, en points. |
| [SetWidthPt](./setwidthpt/) | Représente la largeur de la forme, en points. |
| [GetWidthCM](./getwidthcm/) | Représente la largeur de la forme, en centimètres. |
| [SetWidthCM](./setwidthcm/) | Représente la largeur de la forme, en centimètres. |
| [GetHeight](./getheight/) | Représente la hauteur de la forme, en unité de pixel. |
| [SetHeight](./setheight/) | Représente la hauteur de la forme, en unité de pixel. |
| [GetHeightInch](./getheightinch/) | Représente la hauteur de la forme, en unité de pouces. |
| [SetHeightInch](./setheightinch/) | Représente la hauteur de la forme, en unité de pouces. |
| [GetHeightPt](./getheightpt/) | Représente la hauteur de la forme, en unité de points. |
| [SetHeightPt](./setheightpt/) | Représente la hauteur de la forme, en unité de points. |
| [GetHeightCM](./getheightcm/) | Représente la hauteur de la forme, en unité de centimètres. |
| [SetHeightCM](./setheightcm/) | Représente la hauteur de la forme, en unité de centimètres. |
| [GetLeft](./getleft/) | Représente le décalage horizontal de la forme par rapport à sa colonne de gauche, en unité de pixels. |
| [SetLeft](./setleft/) | Représente le décalage horizontal de la forme par rapport à sa colonne de gauche, en unité de pixels. |
| [GetLeftInch](./getleftinch/) | Représente le décalage horizontal de la forme par rapport à sa colonne de gauche, en unité de pouces. |
| [SetLeftInch](./setleftinch/) | Représente le décalage horizontal de la forme par rapport à sa colonne de gauche, en unité de pouces. |
| [GetLeftCM](./getleftcm/) | Représente le décalage horizontal de la forme par rapport à sa colonne de gauche, en unité de centimètres. |
| [SetLeftCM](./setleftcm/) | Représente le décalage horizontal de la forme par rapport à sa colonne de gauche, en unité de centimètres. |
| [GetTop](./gettop/) | Représente le décalage vertical de la forme par rapport à sa rangée supérieure, en unité de pixels. |
| [SetTop](./settop/) | Représente le décalage vertical de la forme par rapport à sa rangée supérieure, en unité de pixels. |
| [GetTopInch](./gettopinch/) | Représente le décalage vertical de la forme par rapport à sa rangée supérieure, en unité de pouces. |
| [SetTopInch](./settopinch/) | Représente le décalage vertical de la forme par rapport à sa rangée supérieure, en unité de pouces. |
| [GetTopCM](./gettopcm/) | Représente le décalage vertical de la forme par rapport à sa rangée supérieure, en unité de centimètres. |
| [SetTopCM](./settopcm/) | Représente le décalage vertical de la forme par rapport à sa rangée supérieure, en unité de centimètres. |
| [GetTopToCorner](./gettoptocorner/) | Obtient et définit le décalage vertical de la forme par rapport à la bordure supérieure de la feuille de calcul, en unité de pixels. |
| [SetTopToCorner](./settoptocorner/) | Obtient et définit le décalage vertical de la forme par rapport à la bordure supérieure de la feuille de calcul, en unité de pixels. |
| [GetLeftToCorner](./getlefttocorner/) | Obtient et définit le décalage horizontal de la forme par rapport à la bordure gauche de la feuille de calcul. |
| [SetLeftToCorner](./setlefttocorner/) | Obtient et définit le décalage horizontal de la forme par rapport à la bordure gauche de la feuille de calcul. |
| [GetX](./getx/) | Obtient et définit le décalage horizontal de la forme par rapport à la bordure gauche de la feuille de calcul, en unité de pixels. |
| [SetX](./setx/) | Obtient et définit le décalage horizontal de la forme par rapport à la bordure gauche de la feuille de calcul, en unité de pixels. |
| [GetY](./gety/) | Obtient et définit le décalage vertical de la forme par rapport à la bordure supérieure de la feuille de calcul, en unité de pixels. |
| [SetY](./sety/) | Obtient et définit le décalage vertical de la forme par rapport à la bordure supérieure de la feuille de calcul, en unité de pixels. |
| [GetWidthScale](./getwidthscale/) | Obtient et définit l'échelle de largeur, en pourcentage de la largeur d'origine de l'image. Si la forme n'est pas une image, la propriété WidthScale ne renvoie que 100 ; |
| [SetWidthScale](./setwidthscale/) | Obtient et définit l'échelle de largeur, en pourcentage de la largeur d'origine de l'image. Si la forme n'est pas une image, la propriété WidthScale ne renvoie que 100 ; |
| [GetHeightScale](./getheightscale/) | Obtient et définit l'échelle de hauteur, en pourcentage de la hauteur d'origine de l'image. Si la forme n'est pas une image, la propriété HeightScale ne renvoie que 100 ; |
| [SetHeightScale](./setheightscale/) | Obtient et définit l'échelle de hauteur, en pourcentage de la hauteur d'origine de l'image. Si la forme n'est pas une image, la propriété HeightScale ne renvoie que 100 ; |
| [GetTopInShape](./gettopinshape/) | Représente le décalage vertical de la forme par rapport à la bordure supérieure de la forme parente, en unité de 1/4000 de la hauteur de la forme parente. |
| [SetTopInShape](./settopinshape/) | Représente le décalage vertical de la forme par rapport à la bordure supérieure de la forme parente, en unité de 1/4000 de la hauteur de la forme parente. |
| [GetLeftInShape](./getleftinshape/) | Représente le décalage horizontal de la forme par rapport à la bordure gauche de la forme parente, en unité de 1/4000 de la largeur de la forme parente. |
| [SetLeftInShape](./setleftinshape/) | Représente le décalage horizontal de la forme par rapport à la bordure gauche de la forme parente, en unité de 1/4000 de la largeur de la forme parente. |
| [GetWidthInShape](./getwidthinshape/) | Représente la largeur de la forme, en unité de 1/4000 de la forme parente. |
| [SetWidthInShape](./setwidthinshape/) | Représente la largeur de la forme, en unité de 1/4000 de la forme parente. |
| [GetHeightInShape](./getheightinshape/) | Représente le décalage vertical de la forme par rapport à la bordure supérieure de la forme parente, en unité de 1/4000 de la hauteur de la forme parente.. |
| [SetHeightInShape](./setheightinshape/) | Représente le décalage vertical de la forme par rapport à la bordure supérieure de la forme parente, en unité de 1/4000 de la hauteur de la forme parente.. |
| [GetGroup](./getgroup/) | Obtient la forme de groupe qui contient cette forme. |
| [GetType](./gettype/) | Obtient le type de forme automatique. |
| [GetHasLine](./gethasline/) | Obtient et définit si la bordure de ligne de la forme est visible. |
| [SetHasLine](./sethasline/) | Obtient et définit si la bordure de ligne de la forme est visible. |
| [IsFilled](./isfilled/) | Indique si le format de remplissage est visible. |
| [SetIsFilled](./setisfilled/) | Indique si le format de remplissage est visible. |
| [IsFlippedHorizontally](./isflippedhorizontally/) | Obtient et définit si la forme est retournée horizontalement. |
| [SetIsFlippedHorizontally](./setisflippedhorizontally/) | Obtient et définit si la forme est retournée horizontalement. |
| [IsFlippedVertically](./isflippedvertically/) | Obtient et définit si la forme est retournée verticalement . |
| [SetIsFlippedVertically](./setisflippedvertically/) | Obtient et définit si la forme est retournée verticalement . |
| [GetActualLowerRightRow](./getactuallowerrightrow/) | Obtenez la ligne inférieure réelle. |
| [GetConnectionPoints](./getconnectionpoints/) | Obtenez les points de connexion |
| [ToImage_ImageType](./toimage_imagetype/) | Crée l'image de la forme et l'enregistre dans un flux au format spécifié. |
| [GetRelativeToOriginalPictureSize](./getrelativetooriginalpicturesize/) | Indique si la forme est relative à la taille de l'image originale. |
| [SetRelativeToOriginalPictureSize](./setrelativetooriginalpicturesize/) | Indique si la forme est relative à la taille de l'image originale. |
| [GetLinkedCell](./getlinkedcell/) | Obtient ou définit la plage de feuille de calcul liée à la valeur du contrôle. |
| [SetLinkedCell_String](./setlinkedcell_string/) | Obtient ou définit la plage de feuille de calcul liée à la valeur du contrôle. |
| [GetInputRange](./getinputrange/) | Obtient ou définit la plage de feuille de calcul utilisée pour remplir la zone combinée spécifiée. |
| [SetInputRange_String](./setinputrange_string/) | Obtient ou définit la plage de feuille de calcul utilisée pour remplir la zone combinée spécifiée. |
| [UpdateSelectedValue](./updateselectedvalue/) | Mettez à jour la valeur sélectionnée avec la valeur de la cellule liée. |
| [GetTextShapeType](./gettextshapetype/) | Obtient et définit le type de forme de texte prédéfini. |
| [SetTextShapeType](./settextshapetype/) | Obtient et définit le type de forme de texte prédéfini. |
| [GetTextBody](./gettextbody/) | Obtient et définit le paramètre du texte de la forme. |
| [GetFont](./getfont/) | Représente la police de la forme. |
| [SetFont](./setfont/) | Représente la police de la forme. |
| [GetTextOptions](./gettextoptions/) | Représente les options de texte de la forme. |
| [SetTextOptions](./settextoptions/) | Représente les options de texte de la forme. |
| [CalculateTextSize](./calculatetextsize/) | Recalculer la zone de texte |
| [GetText](./gettext/) | Obtient et définit le texte de cette forme. |
| [SetText](./settext/) | Obtient et définit le texte de cette forme. |
| [IsRichText](./isrichtext/) | Indique si le texte est enrichi ou non. |
| [GetHtmlText](./gethtmltext/) | Obtient et définit la chaîne HTML qui contient des données et certains formats dans cette zone de texte. |
| [SetHtmlText](./sethtmltext/) | Obtient et définit la chaîne HTML qui contient des données et certains formats dans cette zone de texte. |
| [FormatCharacters](./formatcharacters/) | Formate certains caractères avec le paramètre de police. |
| [Characters](./characters/) | Renvoie un objet Characters qui représente une plage de caractères dans le texte. |
| [GetRichFormattings](./getrichformattings/) | Renvoie tous les objets Characters qui représentent une plage de caractères dans le texte . |
| [GetTextVerticalOverflow](./gettextverticaloverflow/) | Obtient et définit le type de dépassement vertical du texte de la forme qui contient du texte. |
| [SetTextVerticalOverflow](./settextverticaloverflow/) | Obtient et définit le type de dépassement vertical du texte de la forme qui contient du texte. |
| [GetTextHorizontalOverflow](./gettexthorizontaloverflow/) | Obtient et définit le type de dépassement horizontal du texte de la forme qui contient du texte. |
| [SetTextHorizontalOverflow](./settexthorizontaloverflow/) | Obtient et définit le type de dépassement horizontal du texte de la forme qui contient du texte. |
| [IsTextWrapped](./istextwrapped/) | Obtient et définit le type d'habillage du texte de la forme qui contient du texte. |
| [SetIsTextWrapped](./setistextwrapped/) | Obtient et définit le type d'habillage du texte de la forme qui contient du texte. |
| [GetTextOrientationType](./gettextorientationtype/) | Obtient et définit le type d'orientation du texte de la forme. |
| [SetTextOrientationType](./settextorientationtype/) | Obtient et définit le type d'orientation du texte de la forme. |
| [GetTextHorizontalAlignment](./gettexthorizontalalignment/) | Obtient et définit le type d'alignement horizontal du texte de la forme. |
| [SetTextHorizontalAlignment](./settexthorizontalalignment/) | Obtient et définit le type d'alignement horizontal du texte de la forme. |
| [GetTextVerticalAlignment](./gettextverticalalignment/) | Obtient et définit le type d'alignement vertical du texte de la forme. |
| [SetTextVerticalAlignment](./settextverticalalignment/) | Obtient et définit le type d'alignement vertical du texte de la forme. |
| [GetTextDirection](./gettextdirection/) | Obtient/Définit la direction du flux de texte pour cet objet. |
| [SetTextDirection](./settextdirection/) | Obtient/Définit la direction du flux de texte pour cet objet. |
| [GetTextBoxOptions](./gettextboxoptions/) | Obtient les informations texte dans la forme |
| [GetControlData](./getcontroldata/) | Obtient les données du contrôle. |
| [GetActiveXControl](./getactivexcontrol/) | Obtient le contrôle ActiveX. |
| [RemoveActiveXControl](./removeactivexcontrol/) | Supprime le contrôle ActiveX. |
| [GetPaths](./getpaths/) | Obtient les chemins d'une forme géométrique personnalisée. |
| [GetGeometry](./getgeometry/) | Obtient la géométrie |
| [GetCreateId](./getcreateid/) | Obtient et définit l'ID de création pour cette forme. |
| [SetCreateId](./setcreateid/) | Obtient et définit l'ID de création pour cette forme. |
| [IsDecorative](./isdecorative/) | Indique si l'objet est décoratif. |
| [SetIsDecorative](./setisdecorative/) | Indique si l'objet est décoratif. |
| [GetActualBox](./getactualbox/) | Obtient la position et la taille réelles de la forme (après application de la rotation, du retournement, etc.) |
| [FitToTextSize](./fittotextsize/) | Recalcule une zone de texte adaptée à l'affichage de tout le contenu texte. |
| [GetResultOfSmartArt](./getresultofsmartart/) | Conversion du SmartArt en formes groupées. |
| [IsSameSetting](./issamesetting/) | Renvoie si la forme est identique. |
