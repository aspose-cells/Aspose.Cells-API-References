---
title: "Style Classe"
linktitle: "Style"
second_title: "Référence API C++ d'Aspose.Cells pour Go"
description: "Classe Style. Encapsule l'objet qui représente style en Go."
type: docs
weight: 200
url: /fr/go-cpp/style/
---

## Style class

Représente le style d'affichage du document Excel, tel que la police, la couleur, l'alignement, la bordure, etc. L'objet Style contient tous les attributs de style (police, format numérique, alignement, etc.) en tant que propriétés.

```go

type Style struct  {
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
| [GetBackgroundThemeColor](./getbackgroundthemecolor/) | Obtient et définit la couleur du thème d'arrière-plan. |
| [SetBackgroundThemeColor](./setbackgroundthemecolor/) | Obtient et définit la couleur du thème d'arrière-plan. |
| [GetForegroundThemeColor](./getforegroundthemecolor/) | Obtient et définit la couleur du thème de premier plan. |
| [SetForegroundThemeColor](./setforegroundthemecolor/) | Obtient et définit la couleur du thème de premier plan. |
| [GetName](./getname/) | Obtient ou définit le nom du style. |
| [SetName](./setname/) | Obtient ou définit le nom du style. |
| [GetPattern](./getpattern/) | Obtient ou définit le type de motif d'arrière-plan de la cellule. |
| [SetPattern](./setpattern/) | Obtient ou définit le type de motif d'arrière-plan de la cellule. |
| [SetPatternColor](./setpatterncolor/) | Définit la couleur d'arrière-plan. |
| [GetBorders](./getborders/) | Obtient la BorderCollection du style. |
| [GetBackgroundColor](./getbackgroundcolor/) | Obtient ou définit la couleur d'arrière-plan d'un style. |
| [SetBackgroundColor](./setbackgroundcolor/) | Obtient ou définit la couleur d'arrière-plan d'un style. |
| [GetBackgroundArgbColor](./getbackgroundargbcolor/) | Obtient et définit la couleur d'arrière-plan avec une valeur ARGB 32 bits. |
| [SetBackgroundArgbColor](./setbackgroundargbcolor/) | Obtient et définit la couleur d'arrière-plan avec une valeur ARGB 32 bits. |
| [GetForegroundColor](./getforegroundcolor/) | Obtient ou définit la couleur de premier plan d'un style. |
| [SetForegroundColor](./setforegroundcolor/) | Obtient ou définit la couleur de premier plan d'un style. |
| [GetForegroundArgbColor](./getforegroundargbcolor/) | Obtient et définit la couleur de premier plan avec une valeur ARGB 32 bits. |
| [SetForegroundArgbColor](./setforegroundargbcolor/) | Obtient et définit la couleur de premier plan avec une valeur ARGB 32 bits. |
| [Copy](./copy/) | Copie les données d'un autre objet style |
| [GetHasBorders](./gethasborders/) | Vérifie si des bordures ont été définies pour le style. |
| [GetParentStyle](./getparentstyle/) | Obtient le style parent de ce style. |
| [Update](./update/) | Applique le style nommé aux styles des cellules qui utilisent ce style nommé.Cela fonctionne comme cliquer sur le bouton "ok" après avoir terminé la modification du style.S'applique uniquement aux styles nommés. |
| [IsNumberFormatApplied](./isnumberformatapplied/) | Indique si le formatage des nombres doit être appliqué. |
| [SetIsNumberFormatApplied](./setisnumberformatapplied/) | Indique si le formatage des nombres doit être appliqué. |
| [IsFontApplied](./isfontapplied/) | Indique si le formatage de la police doit être appliqué. |
| [SetIsFontApplied](./setisfontapplied/) | Indique si le formatage de la police doit être appliqué. |
| [IsAlignmentApplied](./isalignmentapplied/) | Indique si le formatage de l'alignement doit être appliqué. |
| [SetIsAlignmentApplied](./setisalignmentapplied/) | Indique si le formatage de l'alignement doit être appliqué. |
| [IsBorderApplied](./isborderapplied/) | Indique si le formatage des bordures doit être appliqué. |
| [SetIsBorderApplied](./setisborderapplied/) | Indique si le formatage des bordures doit être appliqué. |
| [IsFillApplied](./isfillapplied/) | Indique si le formatage du remplissage doit être appliqué. |
| [SetIsFillApplied](./setisfillapplied/) | Indique si le formatage du remplissage doit être appliqué. |
| [IsProtectionApplied](./isprotectionapplied/) | Indique si le formatage de la protection doit être appliqué. |
| [SetIsProtectionApplied](./setisprotectionapplied/) | Indique si le formatage de la protection doit être appliqué. |
| [IsModified](./ismodified/) | Vérifie si les propriétés spécifiées du style ont été modifiées.Utilisé pour le style des ConditionalFormattings afin de vérifier si les propriétés spécifiées de ce style doivent être utilisées lors de l'application des ConditionalFormattings sur une cellule. |
| [Equals](./equals/) | Détermine si deux instances de Style sont égales. |
| [GetHashCode](./gethashcode/) | Servir de fonction de hachage pour un objet Style. |
| [GetIndentLevel](./getindentlevel/) | Représente le niveau d'indentation pour la cellule ou la plage. Ne peut être qu'un entier compris entre 0 et 250. |
| [SetIndentLevel](./setindentlevel/) | Représente le niveau d'indentation pour la cellule ou la plage. Ne peut être qu'un entier compris entre 0 et 250. |
| [GetFont](./getfont/) | Obtient un objet Font. |
| [GetRotationAngle](./getrotationangle/) | Représente l'angle de rotation du texte. |
| [SetRotationAngle](./setrotationangle/) | Représente l'angle de rotation du texte. |
| [GetHorizontalAlignment](./gethorizontalalignment/) | Obtient ou définit le type d'alignement horizontal du texte dans une cellule. |
| [SetHorizontalAlignment](./sethorizontalalignment/) | Obtient ou définit le type d'alignement horizontal du texte dans une cellule. |
| [GetVerticalAlignment](./getverticalalignment/) | Obtient ou définit le type d'alignement vertical du texte dans une cellule. |
| [SetVerticalAlignment](./setverticalalignment/) | Obtient ou définit le type d'alignement vertical du texte dans une cellule. |
| [IsTextWrapped](./istextwrapped/) | Obtient ou définit une valeur indiquant si le texte d'une cellule est renvoyé à la ligne. |
| [SetIsTextWrapped](./setistextwrapped/) | Obtient ou définit une valeur indiquant si le texte d'une cellule est renvoyé à la ligne. |
| [GetNumber](./getnumber/) | Obtient ou définit le format d'affichage des nombres et des dates. Les modèles de formatage diffèrent selon les régions. |
| [SetNumber](./setnumber/) | Obtient ou définit le format d'affichage des nombres et des dates. Les modèles de formatage diffèrent selon les régions. |
| [SetBorder_BorderType_CellBorderType_Color](./setborder_bordertype_cellbordertype_color/) | Définit les bordures du style. |
| [SetBorder_BorderType_CellBorderType_CellsColor](./setborder_bordertype_cellbordertype_cellscolor/) | Définit les bordures du style. |
| [SetOutlineBorders_CellBorderType_Color](./setoutlineborders_cellbordertype_color/) | Définir les bordures de contour |
| [SetOutlineBorders_CellBorderType_CellsColor](./setoutlineborders_cellbordertype_cellscolor/) | Définir les bordures de contour |
| [IsLocked](./islocked/) | Obtient ou définit une valeur indiquant si une cellule peut être modifiée ou non. |
| [SetIsLocked](./setislocked/) | Obtient ou définit une valeur indiquant si une cellule peut être modifiée ou non. |
| [SetCustom_String_Bool](./setcustom_string_bool/) | Définit la chaîne de format numérique personnalisé d'une cellule. |
| [GetCustom](./getcustom/) | Représente la chaîne de format numérique personnalisé de cet objet de style. Si le format numérique personnalisé n'est pas défini (par exemple, le format numérique est intégré), "" sera retourné. |
| [SetCustom_String](./setcustom_string/) | Représente la chaîne de format numérique personnalisé de cet objet de style. Si le format numérique personnalisé n'est pas défini (par exemple, le format numérique est intégré), "" sera retourné. |
| [GetCultureCustom](./getculturecustom/) | Obtient et définit la chaîne de modèle dépendante de la culture pour le format numérique. Si aucun format numérique n'a été défini pour cet objet, null sera retourné. Si le format numérique est intégré, la chaîne de modèle correspondant au numéro intégré sera retournée. |
| [SetCultureCustom](./setculturecustom/) | Obtient et définit la chaîne de modèle dépendante de la culture pour le format numérique. Si aucun format numérique n'a été défini pour cet objet, null sera retourné. Si le format numérique est intégré, la chaîne de modèle correspondant au numéro intégré sera retournée. |
| [GetInvariantCustom](./getinvariantcustom/) | Obtient la chaîne de modèle indépendante de la culture pour le format numérique. Si aucun format numérique n'a été défini pour cet objet, null sera retourné. Si le format numérique est intégré, la chaîne de modèle correspondant au numéro intégré sera retournée. |
| [IsFormulaHidden](./isformulahidden/) | Représente si la formule sera masquée lorsque la feuille de calcul est protégée. |
| [SetIsFormulaHidden](./setisformulahidden/) | Représente si la formule sera masquée lorsque la feuille de calcul est protégée. |
| [GetShrinkToFit](./getshrinktofit/) | Représente si le texte se réduit automatiquement pour s'adapter à la largeur de colonne disponible. |
| [SetShrinkToFit](./setshrinktofit/) | Représente si le texte se réduit automatiquement pour s'adapter à la largeur de colonne disponible. |
| [GetTextDirection](./gettextdirection/) | Représente l'ordre de lecture du texte. |
| [SetTextDirection](./settextdirection/) | Représente l'ordre de lecture du texte. |
| [IsJustifyDistributed](./isjustifydistributed/) | Indique si l'alignement justifié ou réparti des cellules doit être utilisé sur la dernière ligne de texte. |
| [SetIsJustifyDistributed](./setisjustifydistributed/) | Indique si l'alignement justifié ou réparti des cellules doit être utilisé sur la dernière ligne de texte. |
| [GetQuotePrefix](./getquoteprefix/) | Indique si la valeur de la cellule commence par une apostrophe simple. |
| [SetQuotePrefix](./setquoteprefix/) | Indique si la valeur de la cellule commence par une apostrophe simple. |
| [IsGradient](./isgradient/) | Indique si le remplissage de la cellule est un motif de dégradé. |
| [SetIsGradient](./setisgradient/) | Indique si le remplissage de la cellule est un motif de dégradé. |
| [SetTwoColorGradient](./settwocolorgradient/) | Définit le remplissage spécifié comme un dégradé bicolore. |
| [GetTwoColorGradientSetting](./gettwocolorgradientsetting/) | Obtenir le paramètre du dégradé bicolore. |
| [IsPercent](./ispercent/) | Indique si le format numérique est un format de pourcentage. |
| [IsDateTime](./isdatetime/) | Indique si le format numérique est un format de date. |
| [IsCheckBox](./ischeckbox/) | Indique s'il s'agit d'un style de case à cocher |
| [SetIsCheckBox](./setischeckbox/) | Indique s'il s'agit d'un style de case à cocher |
| [ToJson](./tojson/) | Convertir le style en données de structure JSON. |
| [GetLeftBorder](./getleftborder/) | Obtient la bordure gauche. |
| [GetRightBorder](./getrightborder/) | Obtient la bordure droite. |
| [GetTopBorder](./gettopborder/) | Obtient la bordure supérieure. |
| [GetBottomBorder](./getbottomborder/) | Obtient la bordure inférieure. |
