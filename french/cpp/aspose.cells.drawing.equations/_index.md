---
title: Espace de noms Aspose::Cells::Drawing::Equations
linktitle: Aspose::Cells::Drawing::Equations
second_title: Référence de l'API Aspose.Cells pour C++
description: 'Comment utiliser l'espace de noms Aspose::Cells::Drawing::Equations en C++.'
type: docs
weight: 600
url: /fr/cpp/aspose.cells.drawing.equations/
---



## Classes

| Classe | Description |
| --- | --- |
| [AccentEquationNode](./accentequationnode/) | Cette classe spécifie une équation d'accent, composée d'un composant de base et d'un diacritique combiné. |
| [ArrayEquationNode](./arrayequationnode/) | Spécifie la fonction Equation-Array, un objet composé d'une ou plusieurs équations. |
| [BarEquationNode](./barequationnode/) | Cette classe spécifie l'équation à barre, composée d'un argument de base et d'une barre supérieure ou inférieure. |
| [BorderBoxEquationNode](./borderboxequationnode/) | Cette classe spécifie la fonction [Border](../aspose.cells/border/) Box, composée d'une bordure dessinée autour d'une équation. |
| [BoxEquationNode](./boxequationnode/) | Cette classe spécifie la fonction box, qui est utilisée pour regrouper les composants d'une équation. |
| [DelimiterEquationNode](./delimiterequationnode/) | Cette classe spécifie l'équation délimiteur, composée de délimiteurs d'ouverture et de fermeture (tels que les parenthèses, accolades, crochets et barres verticales), ainsi qu'un composant contenu à l'intérieur. Le délimiteur peut comporter plusieurs composants, avec un caractère séparateur désigné entre chaque composant. |
| [EquationComponentNode](./equationcomponentnode/) | Cette classe spécifie les composants d'une équation ou d'une expression mathématique. Différents types de composants sont combinés en différentes équations. Par exemple, une fraction se compose de deux parties, un composant numérateur et un composant dénominateur. Pour plus de types de composants, veuillez vous référer à 'EquationNodeType'. |
| [EquationNode](./equationnode/) | Classe abstraite pour dériver d'autres nœuds d'équation. |
| [EquationNodeParagraph](./equationnodeparagraph/) | Cette classe spécifie un paragraphe mathématique contenant un ou plusieurs éléments MathEquationNode(OMath). |
| [FractionEquationNode](./fractionequationnode/) | Cette classe spécifie l'équation de fraction, composée d'un numérateur et d'un dénominateur séparés par une barre de fraction. La barre de fraction peut être horizontale ou diagonale, selon les propriétés de la fraction. L'équation de fraction est également utilisée pour représenter la fonction empilement, qui place un élément au-dessus d'un autre, sans barre de fraction. |
| [FunctionEquationNode](./functionequationnode/) | Cette classe spécifie l'équation Fonction-Appliquer, qui se compose d'un nom de fonction et d'un argument sur lequel elle agit. Les types des composants nom et argument sont '[EquationNodeType.FunctionName](./equationnodetype/)' et '[EquationNodeType.Base](./equationnodetype/)' respectivement. |
| [GroupCharacterEquationNode](./groupcharacterequationnode/) | Cette classe spécifie la fonction Groupe-Caractère, consistant en un caractère dessiné au-dessus ou en dessous du texte, souvent dans le but de regrouper visuellement les éléments. |
| [LimLowUppEquationNode](./limlowuppequationnode/) | Cette classe spécifie la fonction limite. |
| [MathematicalEquationNode](./mathematicalequationnode/) | Cette classe spécifie une équation ou une expression mathématique. Tout le texte mathématique des équations ou des expressions mathématiques est contenu par cette classe. |
| [MatrixEquationNode](./matrixequationnode/) | Cette classe spécifie l'équation Matrice, composée d'un ou plusieurs éléments disposés en une ou plusieurs lignes et une ou plusieurs colonnes. |
| [NaryEquationNode](./naryequationnode/) | Cette classe spécifie une équation d'opérateur n-aire composée d'un opérateur n-aire, d'une base (ou opérande), et de limites supérieures et inférieures optionnelles. |
| [RadicalEquationNode](./radicalequationnode/) | Cette classe spécifie l'équation radicale, composée d'un degré optionnel deg([EquationNodeType.Degree](./equationnodetype/)) et d'une base. |
| [SubSupEquationNode](./subsupequationnode/) | Cette classe spécifie une équation qui peut être optionnellement en exposant ou en indice. Il existe quatre formes principales de cette équation : exposant, indice, exposant et indice placés à gauche de la base, exposant et indice placés à droite de la base. |
| [TextRunEquationNode](./textrunequationnode/) | Cette classe dans le nœud d'équation est utilisée pour stocker le contenu réel (une séquence de texte mathématique) de l'équation. Généralement un objet nœud par caractère. |
| [UnknowEquationNode](./unknowequationnode/) | Classe de nœud d'équation de type inconnu. |
## Enums

| Enum | Description |
| --- | --- |
| [EquationCharacterPositionType](./equationcharacterpositiontype/) | Spécifie la position d'un sous-objet particulier au sein de son parent. |
| [EquationCombiningCharacterType](./equationcombiningcharactertype/) | Type de caractères combinés. |
| [EquationDelimiterShapeType](./equationdelimitershapetype/) | Cela spécifie la forme des délimiteurs dans l'objet délimiteur. |
| [EquationFractionType](./equationfractiontype/) | Cela spécifie le style d'affichage de la barre de fraction. |
| [EquationHorizontalJustificationType](./equationhorizontaljustificationtype/) | Cela spécifie l'alignement horizontal par défaut des équations dans le document. |
| [EquationLimitLocationType](./equationlimitlocationtype/) | Spécifie l'emplacement de la limite sur un opérateur. |
| [EquationMathematicalOperatorType](./equationmathematicaloperatortype/) | Type d'opérateurs mathématiques. |
| [EquationNodeType](./equationnodetype/) | Type de nœud d'équation. Remarque : (1)[1-99] Actuellement il n'y a qu'un seul nœud dans la portée, et sa valeur d'énumération est 1. Le nœud qu'il spécifie est utilisé pour stocker du texte mathématique. (2)[100-199] Indique que le nœud est un composant de certains nœuds de fonctions spéciales. (3)[200-] Indique que le nœud possède certaines fonctions spéciales. |
| [EquationVerticalJustificationType](./equationverticaljustificationtype/) | Cela spécifie l'alignement vertical par défaut des équations dans le document. |
