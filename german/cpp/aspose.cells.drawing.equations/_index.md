---
title: "Aspose::Cells::Drawing::Equations Namespace"
linktitle: "Aspose::Cells::Drawing::Equations"
second_title: "Aspose.Cells für C++ API-Referenz"
description: "Wie man das Aspose::Cells::Drawing::Equations Namespace in C++ verwendet."
type: docs
weight: 700
url: /de/cpp/aspose.cells.drawing.equations/
---



## Klassen

| Klasse | Beschreibung |
| --- | --- |
| [AccentEquationNode](./accentequationnode/) | Diese Klasse definiert eine Akzentgleichung, die aus einer Basiskomponente und einem kombinierenden Diakritikum besteht. |
| [ArrayEquationNode](./arrayequationnode/) | Definiert die Equation-Array-Funktion, ein Objekt, das aus einer oder mehreren Gleichungen besteht. |
| [BarEquationNode](./barequationnode/) | Diese Klasse definiert die Balkengleichung, die aus einem Basisargument und einem Überstrich oder Unterstrich besteht. |
| [BorderBoxEquationNode](./borderboxequationnode/) | Diese Klasse definiert die [Border](../aspose.cells/border/) Box-Funktion, die aus einem um eine Gleichung gezeichneten Rahmen besteht. |
| [BoxEquationNode](./boxequationnode/) | Diese Klasse definiert die Box-Funktion, die verwendet wird, um Komponenten einer Gleichung zu gruppieren. |
| [DelimiterEquationNode](./delimiterequationnode/) | Diese Klasse definiert die Trennzeichen-Gleichung, die aus öffnenden und schließenden Trennzeichen (wie Klammern, geschweiften Klammern, eckigen Klammern und senkrechten Strichen) und einer darin enthaltenen Komponente besteht. Das Trennzeichen kann mehr als eine Komponente enthalten, mit einem festgelegten Trennzeichen zwischen den einzelnen Komponenten. |
| [EquationComponentNode](./equationcomponentnode/) | Diese Klasse definiert die Komponenten einer Gleichung oder eines mathematischen Ausdrucks. Verschiedene Arten von Komponenten werden zu unterschiedlichen Gleichungen kombiniert. Zum Beispiel besteht ein Bruch aus zwei Teilen, einer Zählerkomponente und einer Nennerkomponente. Für weitere Komponententypen verweisen Sie bitte auf 'EquationNodeType'. |
| [EquationNode](./equationnode/) | Abstrakte Klasse zum Ableiten anderer Gleichungsknoten. |
| [EquationNodeParagraph](./equationnodeparagraph/) | Diese Klasse definiert einen mathematischen Absatz, der ein oder mehrere MathEquationNode(OMath)-Elemente enthält. |
| [FractionEquationNode](./fractionequationnode/) | Diese Klasse definiert die Bruchgleichung, die aus einem Zähler und einem Nenner besteht, die durch einen Bruchstrich getrennt sind. Der Bruchstrich kann horizontal oder diagonal sein, abhängig von den Bruch-Eigenschaften. Die Bruchgleichung wird auch verwendet, um die Stapelfunktion darzustellen, die ein Element über einem anderen platziert, ohne Bruchstrich. |
| [FunctionEquationNode](./functionequationnode/) | Diese Klasse definiert die Function-Apply-Gleichung, die aus einem Funktionsnamen und einem darauf angewendeten Argument besteht. Die Typen der Namens- und Argumentkomponenten sind jeweils '[EquationNodeType.FunctionName](./equationnodetype/)' und '[EquationNodeType.Base](./equationnodetype/)'. |
| [GroupCharacterEquationNode](./groupcharacterequationnode/) | Diese Klasse definiert die Group-Character-Funktion, die aus einem über oder unter dem Text platzierten Zeichen besteht, oft mit dem Zweck, Elemente visuell zu gruppieren. |
| [LimLowUppEquationNode](./limlowuppequationnode/) | Diese Klasse definiert die Grenzwertfunktion. |
| [MathematicalEquationNode](./mathematicalequationnode/) | Diese Klasse definiert eine Gleichung oder einen mathematischen Ausdruck. Alle mathematischen Texte von Gleichungen oder mathematischen Ausdrücken werden von dieser Klasse enthalten. |
| [MatrixEquationNode](./matrixequationnode/) | Diese Klasse definiert die Matrixgleichung, die aus einem oder mehreren Elementen besteht, die in ein oder mehreren Zeilen und ein oder mehreren Spalten angeordnet sind. |
| [NaryEquationNode](./naryequationnode/) | Diese Klasse definiert eine n-stellige Operatorgleichung, die aus einem n-stelligen Operator, einer Basis (oder Operanden) und optionalen oberen und unteren Grenzen besteht. |
| [RadicalEquationNode](./radicalequationnode/) | Diese Klasse definiert die Radikalgleichung, die aus einem optionalen Grad deg([EquationNodeType.Degree](./equationnodetype/)) und einer Basis besteht. |
| [SubSupEquationNode](./subsupequationnode/) | Diese Klasse spezifiziert eine Gleichung, die optional hoch- oder tiefgestellt sein kann. Es gibt vier Hauptformen dieser Gleichung: Hochstellung, Tiefstellung, Hoch- und Tiefstellung links vom Basiszeichen sowie Hoch- und Tiefstellung rechts vom Basiszeichen. |
| [TextRunEquationNode](./textrunequationnode/) | Diese Klasse im Gleichungsknoten wird verwendet, um den tatsächlichen Inhalt (eine Sequenz mathematischen Textes) der Gleichung zu speichern. Normalerweise ein Knotenobjekt pro Zeichen. |
| [UnknowEquationNode](./unknowequationnode/) | Gleichungsknotenklasse unbekannten Typs. |
## Enums

| Aufzählung | Beschreibung |
| --- | --- |
| [EquationCharacterPositionType](./equationcharacterpositiontype/) | Gibt die Position eines bestimmten Unterobjekts innerhalb seines übergeordneten Elements an. |
| [EquationCombiningCharacterType](./equationcombiningcharactertype/) | Typ von Kombinationszeichen. |
| [EquationDelimiterShapeType](./equationdelimitershapetype/) | Dies gibt die Form der Trennzeichen im Trennzeichenobjekt an. |
| [EquationFractionType](./equationfractiontype/) | Dies gibt den Anzeigestil des Bruchstrichs an. |
| [EquationHorizontalJustificationType](./equationhorizontaljustificationtype/) | Dies legt die standardmäßige horizontale Ausrichtung von Gleichungen im Dokument fest. |
| [EquationLimitLocationType](./equationlimitlocationtype/) | Gibt den Grenzort eines Operators an. |
| [EquationMathematicalOperatorType](./equationmathematicaloperatortype/) | Typ mathematischer Operatoren. |
| [EquationNodeType](./equationnodetype/) | Gleichungsknoten-Typ. Hinweis: (1)[1-99] Derzeit gibt es nur einen Knoten im Geltungsbereich, und sein Enumerationswert ist 1. Der angegebene Knoten wird verwendet, um mathematischen Text zu speichern. (2)[100-199] Zeigt an, dass der Knoten Bestandteil einiger spezieller Funktionsknoten ist. (3)[200-] Zeigt an, dass der Knoten besondere Funktionen hat. |
| [EquationVerticalJustificationType](./equationverticaljustificationtype/) | Dies legt die standardmäßige vertikale Ausrichtung von Gleichungen im Dokument fest. |
