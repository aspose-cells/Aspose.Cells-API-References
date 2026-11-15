---
title: "Espacio de nombres Aspose::Cells::Drawing::Equations"
linktitle: "Aspose::Cells::Drawing::Equations"
second_title: "Referencia de la API de Aspose.Cells para C++"
description: "Cómo usar el espacio de nombres Aspose::Cells::Drawing::Equations en C++."
type: docs
weight: 700
url: /es/cpp/aspose.cells.drawing.equations/
---



## Clases

| Clase | Descripción |
| --- | --- |
| [AccentEquationNode](./accentequationnode/) | Esta clase especifica una ecuación de acento, que consta de un componente base y un diacrítico combinante. |
| [ArrayEquationNode](./arrayequationnode/) | Especifica la función Equation-Array, un objeto que consta de una o más ecuaciones. |
| [BarEquationNode](./barequationnode/) | Esta clase especifica la ecuación de barra, que consta de un argumento base y una barra superior o inferior. |
| [BorderBoxEquationNode](./borderboxequationnode/) | Esta clase especifica la función [Border](../aspose.cells/border/) Box, que consta de un borde dibujado alrededor de una ecuación. |
| [BoxEquationNode](./boxequationnode/) | Esta clase especifica la función box, que se usa para agrupar componentes de una ecuación. |
| [DelimiterEquationNode](./delimiterequationnode/) | Esta clase especifica la ecuación delimitadora, que consta de delimitadores de apertura y cierre (como paréntesis, llaves, corchetes y barras verticales), y un componente contenido dentro. El delimitador puede tener más de un componente, con un carácter separador designado entre cada componente. |
| [EquationComponentNode](./equationcomponentnode/) | Esta clase especifica los componentes de una ecuación o expresión matemática. Diferentes tipos de componentes se combinan en distintas ecuaciones. Por ejemplo, una fracción consta de dos partes, un componente numerador y un componente denominador. Para más tipos de componentes, consulte 'EquationNodeType'. |
| [EquationNode](./equationnode/) | Clase abstracta para derivar otros nodos de ecuación. |
| [EquationNodeParagraph](./equationnodeparagraph/) | Esta clase especifica un párrafo matemático que contiene uno o más elementos MathEquationNode(OMath). |
| [FractionEquationNode](./fractionequationnode/) | Esta clase especifica la ecuación de fracción, que consta de un numerador y un denominador separados por una barra de fracción. La barra de fracción puede ser horizontal o diagonal, según las propiedades de la fracción. La ecuación de fracción también se usa para representar la función stack, que coloca un elemento sobre otro, sin barra de fracción. |
| [FunctionEquationNode](./functionequationnode/) | Esta clase especifica la ecuación Function-Apply, que consiste en un nombre de función y un argumento al que se aplica. Los tipos de los componentes de nombre y argumento son '[EquationNodeType.FunctionName](./equationnodetype/)' y '[EquationNodeType.Base](./equationnodetype/)' respectivamente. |
| [GroupCharacterEquationNode](./groupcharacterequationnode/) | Esta clase especifica la función Group-Character, que consta de un carácter dibujado encima o debajo del texto, a menudo con el propósito de agrupar visualmente los elementos. |
| [LimLowUppEquationNode](./limlowuppequationnode/) | Esta clase especifica la función límite. |
| [MathematicalEquationNode](./mathematicalequationnode/) | Esta clase especifica una ecuación o expresión matemática. Todo el texto matemático de ecuaciones o expresiones matemáticas está contenido en esta clase. |
| [MatrixEquationNode](./matrixequationnode/) | Esta clase especifica la ecuación Matrix, que consta de uno o más elementos dispuestos en una o más filas y una o más columnas. |
| [NaryEquationNode](./naryequationnode/) | Esta clase especifica una ecuación de operador n-ario que consta de un operador n-ario, una base (u operando) y límites superior e inferior opcionales. |
| [RadicalEquationNode](./radicalequationnode/) | Esta clase especifica la ecuación radical, que consta de un grado opcional deg([EquationNodeType.Degree](./equationnodetype/)) y una base. |
| [SubSupEquationNode](./subsupequationnode/) | Esta clase especifica una ecuación que puede ser opcionalmente superíndice o subíndice. Hay cuatro formas principales de esta ecuación: superíndice, subíndice, superíndice y subíndice colocados a la izquierda de la base, superíndice y subíndice colocados a la derecha de la base. |
| [TextRunEquationNode](./textrunequationnode/) | Esta clase en el nodo de ecuación se usa para almacenar el contenido real (una secuencia de texto matemático) de la ecuación. Normalmente un objeto nodo por carácter. |
| [UnknowEquationNode](./unknowequationnode/) | Clase de nodo de ecuación de tipo desconocido. |
## Enums

| Enumeración | Descripción |
| --- | --- |
| [EquationCharacterPositionType](./equationcharacterpositiontype/) | Especifica la posición de un subobjeto particular dentro de su padre. |
| [EquationCombiningCharacterType](./equationcombiningcharactertype/) | Tipo de caracteres combinantes. |
| [EquationDelimiterShapeType](./equationdelimitershapetype/) | Esto especifica la forma de los delimitadores en el objeto delimitador. |
| [EquationFractionType](./equationfractiontype/) | Esto especifica el estilo de visualización de la barra de fracción. |
| [EquationHorizontalJustificationType](./equationhorizontaljustificationtype/) | Esto especifica la justificación horizontal predeterminada de las ecuaciones en el documento. |
| [EquationLimitLocationType](./equationlimitlocationtype/) | Especifica la ubicación del límite en un operador. |
| [EquationMathematicalOperatorType](./equationmathematicaloperatortype/) | Tipo de operadores matemáticos. |
| [EquationNodeType](./equationnodetype/) | Tipo de nodo de ecuación. Aviso: (1)[1-99] Actualmente solo hay un nodo en el alcance, y su valor de enumeración es 1. El nodo que especifica se usa para almacenar texto matemático. (2)[100-199] Indica que el nodo es un componente de algunos nodos de funciones especiales. (3)[200-] Indica que el nodo tiene algunas funciones especiales. |
| [EquationVerticalJustificationType](./equationverticaljustificationtype/) | Esto especifica la justificación vertical predeterminada de las ecuaciones en el documento. |
