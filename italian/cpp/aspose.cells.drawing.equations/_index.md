---
title: Aspose::Cells::Drawing::Equations namespace
linktitle: Aspose::Cells::Drawing::Equations
second_title: Riferimento API di Aspose.Cells per C++
description: 'Come utilizzare lo spazio dei nomi Aspose::Cells::Drawing::Equations in C++.'
type: docs
weight: 600
url: /it/cpp/aspose.cells.drawing.equations/
---



## Classi

| Classe | Descrizione |
| --- | --- |
| [AccentEquationNode](./accentequationnode/) | Questa classe specifica un'equazione di accento, composta da un componente di base e un diacritico combinante. |
| [ArrayEquationNode](./arrayequationnode/) | Specifica la funzione Equation-Array, un oggetto composto da una o più equazioni. |
| [BarEquationNode](./barequationnode/) | Questa classe specifica l'equazione a barra, composta da un argomento di base e da una barra superiore o inferiore. |
| [BorderBoxEquationNode](./borderboxequationnode/) | Questa classe specifica la funzione [Border](../aspose.cells/border/) Box, composta da un bordo disegnato attorno a un'equazione. |
| [BoxEquationNode](./boxequationnode/) | Questa classe specifica la funzione box, utilizzata per raggruppare i componenti di un'equazione. |
| [DelimiterEquationNode](./delimiterequationnode/) | Questa classe specifica l'equazione delimitatore, composta da delimitatori di apertura e chiusura (come parentesi tonde, graffe, quadre e barre verticali), e da un componente contenuto all'interno. Il delimitatore può avere più di un componente, con un carattere separatore designato tra ciascun componente. |
| [EquationComponentNode](./equationcomponentnode/) | Questa classe specifica i componenti di un'equazione o di un'espressione matematica. Diversi tipi di componenti vengono combinati in diverse equazioni. Ad esempio, una frazione è composta da due parti, un componente numeratore e un componente denominatore. Per ulteriori tipi di componenti, consultare 'EquationNodeType'. |
| [EquationNode](./equationnode/) | Classe astratta per derivare altri nodi di equazione. |
| [EquationNodeParagraph](./equationnodeparagraph/) | Questa classe specifica un paragrafo matematico contenente uno o più elementi MathEquationNode(OMath). |
| [FractionEquationNode](./fractionequationnode/) | Questa classe specifica l'equazione frazione, composta da un numeratore e un denominatore separati da una barra di frazione. La barra di frazione può essere orizzontale o diagonale, a seconda delle proprietà della frazione. L'equazione frazione è anche usata per rappresentare la funzione stack, che posiziona un elemento sopra un altro, senza barra di frazione. |
| [FunctionEquationNode](./functionequationnode/) | Questa classe specifica l'equazione Function-Apply, che consiste in un nome di funzione e un argomento su cui agire. I tipi dei componenti nome e argomento sono '[EquationNodeType.FunctionName](./equationnodetype/)' e '[EquationNodeType.Base](./equationnodetype/)' rispettivamente. |
| [GroupCharacterEquationNode](./groupcharacterequationnode/) | Questa classe specifica la funzione Group-Character, composta da un carattere disegnato sopra o sotto il testo, spesso con lo scopo di raggruppare visivamente gli elementi. |
| [LimLowUppEquationNode](./limlowuppequationnode/) | Questa classe specifica la funzione limite. |
| [MathematicalEquationNode](./mathematicalequationnode/) | Questa classe specifica un'equazione o un'espressione matematica. Tutto il testo matematico delle equazioni o delle espressioni matematiche è contenuto in questa classe. |
| [MatrixEquationNode](./matrixequationnode/) | Questa classe specifica l'equazione Matrix, composta da uno o più elementi disposti in una o più righe e una o più colonne. |
| [NaryEquationNode](./naryequationnode/) | Questa classe specifica un'equazione operatore n-ario composta da un operatore n-ario, una base (o operando) e limiti superiori e inferiori opzionali. |
| [RadicalEquationNode](./radicalequationnode/) | Questa classe specifica l'equazione radice, composta da un grado opzionale deg([EquationNodeType.Degree](./equationnodetype/)) e una base. |
| [SubSupEquationNode](./subsupequationnode/) | Questa classe specifica un'equazione che può opzionalmente essere apice o pedice. Ci sono quattro forme principali di questa equazione: apice, pedice, apice e pedice posizionati a sinistra della base, apice e pedice posizionati a destra della base. |
| [TextRunEquationNode](./textrunequationnode/) | Questa classe nel nodo equazione è usata per memorizzare il contenuto reale (una sequenza di testo matematico) dell'equazione. Di solito un oggetto nodo per carattere. |
| [UnknowEquationNode](./unknowequationnode/) | Classe nodo equazione di tipo sconosciuto. |
## Enums

| Enum | Descrizione |
| --- | --- |
| [EquationCharacterPositionType](./equationcharacterpositiontype/) | Specifica la posizione di un particolare sottooggetto all'interno del suo genitore. |
| [EquationCombiningCharacterType](./equationcombiningcharactertype/) | Tipo di caratteri combinanti. |
| [EquationDelimiterShapeType](./equationdelimitershapetype/) | Questo specifica la forma dei delimitatori nell'oggetto delimitatore. |
| [EquationFractionType](./equationfractiontype/) | Questo specifica lo stile di visualizzazione della barra di frazione. |
| [EquationHorizontalJustificationType](./equationhorizontaljustificationtype/) | Questo specifica l'allineamento orizzontale predefinito delle equazioni nel documento. |
| [EquationLimitLocationType](./equationlimitlocationtype/) | Specifica la posizione del limite su un operatore. |
| [EquationMathematicalOperatorType](./equationmathematicaloperatortype/) | Tipo di operatori matematici. |
| [EquationNodeType](./equationnodetype/) | Tipo di nodo equazione. Nota: (1)[1-99] Attualmente c'è solo un nodo nello scope, e il suo valore di enumerazione è 1. Il nodo specificato è usato per memorizzare testo matematico. (2)[100-199] Indica che il nodo è un componente di alcuni nodi di funzioni speciali. (3)[200-] Indica che il nodo ha alcune funzioni speciali. |
| [EquationVerticalJustificationType](./equationverticaljustificationtype/) | Questo specifica l'allineamento verticale predefinito delle equazioni nel documento. |
