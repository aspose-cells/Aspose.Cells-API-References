---
title: "NaryEquationNode"
second_title: "Riferimento API di Aspose.Cells per Java"
description: "Questa classe specifica un'equazione di operatore n-ario composta da un operatore n-ario, una base o operando e limiti superiori e inferiori opzionali."
type: docs
url: /it/java/com.aspose.cells/naryequationnode/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.FontSetting](../../com.aspose.cells/fontsetting), [com.aspose.cells.EquationNode](../../com.aspose.cells/equationnode)
```
public class NaryEquationNode extends EquationNode
```

Questa classe specifica un'equazione di operatore n-ario composta da un operatore n-ario, una base (o operando) e limiti superiori e inferiori opzionali.
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [addChild(EquationNode node)](#addChild-com.aspose.cells.EquationNode-) | Inserisce il nodo specificato alla fine dell'elenco dei nodi figlio del nodo corrente. |
| [addChild(int equationType)](#addChild-int-) | Inserisci un nodo del tipo specificato alla fine dell'elenco dei nodi figlio del nodo corrente. |
| [createNode(int equationType, Workbook workbook, EquationNode parent)](#createNode-int-com.aspose.cells.Workbook-com.aspose.cells.EquationNode-) | Crea un nodo del tipo specificato. |
| [equals(Object obj)](#equals-java.lang.Object-) | Determina se il nodo dell'equazione corrente è uguale al nodo specificato |
| [getChild(int index)](#getChild-int-) | Restituisce il nodo all'indice specificato tra i figli del nodo corrente. |
| [getClass()](#getClass--) |  |
| [getEquationType()](#getEquationType--) | Ottieni il tipo di equazione del nodo corrente |
| [getFont()](#getFont--) | Restituisce il carattere di questo oggetto. |
| [getLength()](#getLength--) | Ottiene la lunghezza dei caratteri. |
| [getLimitLocation()](#getLimitLocation--) | Questo attributo specifica la posizione dei limiti negli operatori n-ari. |
| [getNaryGrow()](#getNaryGrow--) | Questo attributo specifica la proprietà di crescita degli operatori n-ari a livello di documento. |
| [getNaryOperator()](#getNaryOperator--) | un operatore n-ario.e.g "\u922d?. |
| [getNaryOperatorType()](#getNaryOperatorType--) | un operatore n-ario.e.g "\u922d? |
| [getParentNode()](#getParentNode--) | Specifica il nodo genitore del nodo corrente |
| [getStartIndex()](#getStartIndex--) | Ottiene l'indice di inizio dei caratteri. |
| [getTextOptions()](#getTextOptions--) | Restituisce le opzioni di testo. |
| [getType()](#getType--) | Rappresenta il tipo del nodo. |
| [hashCode()](#hashCode--) |  |
| [insertAfter(int equationType)](#insertAfter-int-) | Inserisce il nodo specificato dopo il nodo corrente. |
| [insertBefore(int equationType)](#insertBefore-int-) | Inserisce il nodo specificato prima del nodo corrente. |
| [insertChild(int index, int equationType)](#insertChild-int-int-) | Inserisce un nodo del tipo specificato nella posizione di indice specificata nell'elenco dei nodi figlio del nodo corrente. |
| [isHideSubscript()](#isHideSubscript--) | Se visualizzare il limite inferiore |
| [isHideSuperscript()](#isHideSuperscript--) | Se visualizzare il limite superiore |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [remove()](#remove--) | Si rimuove dal genitore. |
| [removeAllChildren()](#removeAllChildren--) | Rimuove tutti i nodi figlio del nodo corrente. |
| [removeChild(EquationNode node)](#removeChild-com.aspose.cells.EquationNode-) | Rimuove il nodo specificato dai figli del nodo corrente. |
| [removeChild(int index)](#removeChild-int-) | Rimuove il nodo all'indice specificato dai figli del nodo corrente. |
| [setHideSubscript(boolean value)](#setHideSubscript-boolean-) | Se visualizzare il limite inferiore |
| [setHideSuperscript(boolean value)](#setHideSuperscript-boolean-) | Se visualizzare il limite superiore |
| [setLimitLocation(int value)](#setLimitLocation-int-) | Questo attributo specifica la posizione dei limiti negli operatori n-ari. |
| [setNaryGrow(boolean value)](#setNaryGrow-boolean-) | Questo attributo specifica la proprietà di crescita degli operatori n-ari a livello di documento. |
| [setNaryOperator(String value)](#setNaryOperator-java.lang.String-) | un operatore n-ario.e.g "\u922d?. |
| [setNaryOperatorType(int value)](#setNaryOperatorType-int-) | un operatore n-ario.e.g "\u922d? |
| [setParentNode(EquationNode value)](#setParentNode-com.aspose.cells.EquationNode-) | Specifica il nodo genitore del nodo corrente |
| [setWordArtStyle(int style)](#setWordArtStyle-int-) | Imposta lo stile WordArt predefinito. |
| [toLaTeX()](#toLaTeX--) | Converti questa equazione in espressione LaTeX. |
| [toMathML()](#toMathML--) | Converti questa equazione in espressione MathML. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### addChild(EquationNode node) {#addChild-com.aspose.cells.EquationNode-}
```
public void addChild(EquationNode node)
```


Inserisce il nodo specificato alla fine dell'elenco dei nodi figlio del nodo corrente.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| node | [EquationNode](../../com.aspose.cells/equationnode) | Il nodo specificato |

### addChild(int equationType) {#addChild-int-}
```
public EquationNode addChild(int equationType)
```


Inserisci un nodo del tipo specificato alla fine dell'elenco dei nodi figlio del nodo corrente.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| equationType | int | [EquationNodeType](../../com.aspose.cells/equationnodetype). Tipi di nodi di equazione |

**Returns:**
[EquationNode](../../com.aspose.cells/equationnode) - If the specified type exists, the corresponding node is returned, and if the type does not exist, a node of unknown type is returned.
### createNode(int equationType, Workbook workbook, EquationNode parent) {#createNode-int-com.aspose.cells.Workbook-com.aspose.cells.EquationNode-}
```
public static EquationNode createNode(int equationType, Workbook workbook, EquationNode parent)
```


Crea un nodo del tipo specificato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| equationType | int | [EquationNodeType](../../com.aspose.cells/equationnodetype). Tipi di nodi di equazione |
| workbook | [Workbook](../../com.aspose.cells/workbook) | L'oggetto cartella di lavoro associato all'equazione |
| parent | [EquationNode](../../com.aspose.cells/equationnode) | Il nodo genitore dove si trova questo nodo |

**Returns:**
[EquationNode](../../com.aspose.cells/equationnode) - If the specified type exists, the corresponding node is returned, and if the type does not exist, a node of unknown type is returned.
### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```


Determina se il nodo dell'equazione corrente è uguale al nodo specificato

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| obj | java.lang.Object | Il nodo specificato |

**Returns:**
boolean -
### getChild(int index) {#getChild-int-}
```
public EquationNode getChild(int index)
```


Restituisce il nodo all'indice specificato tra i figli del nodo corrente.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| indice | int | Indice del nodo |

**Returns:**
[EquationNode](../../com.aspose.cells/equationnode) - Returns the corresponding node if the specified node exists, otherwise returns null.
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getEquationType() {#getEquationType--}
```
public int getEquationType()
```


Ottieni il tipo di equazione del nodo corrente

Vedi [EquationNodeType](../../com.aspose.cells/equationnodetype).

**Returns:**
int
### getFont() {#getFont--}
```
public Font getFont()
```


Restituisce il carattere di questo oggetto.

**Returns:**
[Font](../../com.aspose.cells/font)
### getLength() {#getLength--}
```
public int getLength()
```


Ottiene la lunghezza dei caratteri.

**Returns:**
int
### getLimitLocation() {#getLimitLocation--}
```
public int getLimitLocation()
```


Questo attributo specifica la posizione dei limiti negli operatori n-ari. I limiti possono essere centrati sopra e sotto l'operatore n-ario, oppure posizionati appena a destra dell'operatore.

Vedi [EquationLimitLocationType](../../com.aspose.cells/equationlimitlocationtype).

**Returns:**
int
### getNaryGrow() {#getNaryGrow--}
```
public boolean getNaryGrow()
```


Questo attributo specifica la proprietà di crescita degli operatori n-ari a livello di documento. Quando disattivata, gli operatori n-ari come integrali e sommatorie non si espandono per corrispondere all'altezza del loro operando. Quando attivata, l'operatore n-ario cresce verticalmente per corrispondere all'altezza del suo operando.

**Returns:**
boolean
### getNaryOperator() {#getNaryOperator--}
```
public String getNaryOperator()
```


un operatore n-ario. ad es. \"\\u922d?. Si consiglia vivamente di utilizzare l'attributo NaryOperatorType per impostare l'operatore n-ario. Utilizza questa impostazione di proprietà se non riesci a trovare il carattere necessario in un tipo noto.

**Remarks**

Va notato che questa proprietà accetta solo un carattere e, se vengono passati più caratteri, viene accettato solo il primo.

**Returns:**
java.lang.String
### getNaryOperatorType() {#getNaryOperatorType--}
```
public int getNaryOperatorType()
```


un operatore n-ario.e.g "\u922d?

Vedi [EquationMathematicalOperatorType](../../com.aspose.cells/equationmathematicaloperatortype).

**Returns:**
int
### getParentNode() {#getParentNode--}
```
public EquationNode getParentNode()
```


Specifica il nodo genitore del nodo corrente

**Returns:**
[EquationNode](../../com.aspose.cells/equationnode)
### getStartIndex() {#getStartIndex--}
```
public int getStartIndex()
```


Ottiene l'indice di inizio dei caratteri.

**Returns:**
int
### getTextOptions() {#getTextOptions--}
```
public TextOptions getTextOptions()
```


Restituisce le opzioni di testo.

**Returns:**
[TextOptions](../../com.aspose.cells/textoptions)
### getType() {#getType--}
```
public int getType()
```


Rappresenta il tipo del nodo.

Vedi [TextNodeType](../../com.aspose.cells/textnodetype).

**Returns:**
int
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### insertAfter(int equationType) {#insertAfter-int-}
```
public EquationNode insertAfter(int equationType)
```


Inserisce il nodo specificato dopo il nodo corrente.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| equationType | int | [EquationNodeType](../../com.aspose.cells/equationnodetype). Tipi di nodi di equazione |

**Returns:**
[EquationNode](../../com.aspose.cells/equationnode) - If the specified type exists, the corresponding node is returned, and if the type does not exist, a node of unknown type is returned.
### insertBefore(int equationType) {#insertBefore-int-}
```
public EquationNode insertBefore(int equationType)
```


Inserisce il nodo specificato prima del nodo corrente.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| equationType | int | [EquationNodeType](../../com.aspose.cells/equationnodetype). Tipi di nodi di equazione |

**Returns:**
[EquationNode](../../com.aspose.cells/equationnode) - If the specified type exists, the corresponding node is returned, and if the type does not exist, a node of unknown type is returned.
### insertChild(int index, int equationType) {#insertChild-int-int-}
```
public EquationNode insertChild(int index, int equationType)
```


Inserisce un nodo del tipo specificato nella posizione di indice specificata nell'elenco dei nodi figlio del nodo corrente.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| indice | int | valore dell'indice |
| equationType | int | [EquationNodeType](../../com.aspose.cells/equationnodetype). Tipi di nodi di equazione |

**Returns:**
[EquationNode](../../com.aspose.cells/equationnode) - If the specified type exists, the corresponding node is returned, and if the type does not exist, a node of unknown type is returned.
### isHideSubscript() {#isHideSubscript--}
```
public boolean isHideSubscript()
```


Se visualizzare il limite inferiore

**Returns:**
boolean
### isHideSuperscript() {#isHideSuperscript--}
```
public boolean isHideSuperscript()
```


Se visualizzare il limite superiore

**Returns:**
boolean
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### remove() {#remove--}
```
public void remove()
```


Si rimuove dal genitore.

### removeAllChildren() {#removeAllChildren--}
```
public void removeAllChildren()
```


Rimuove tutti i nodi figlio del nodo corrente.

### removeChild(EquationNode node) {#removeChild-com.aspose.cells.EquationNode-}
```
public void removeChild(EquationNode node)
```


Rimuove il nodo specificato dai figli del nodo corrente.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| node | [EquationNode](../../com.aspose.cells/equationnode) | Nodo da eliminare. |

### removeChild(int index) {#removeChild-int-}
```
public void removeChild(int index)
```


Rimuove il nodo all'indice specificato dai figli del nodo corrente.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| indice | int | Indice del nodo |

### setHideSubscript(boolean value) {#setHideSubscript-boolean-}
```
public void setHideSubscript(boolean value)
```


Se visualizzare il limite inferiore

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setHideSuperscript(boolean value) {#setHideSuperscript-boolean-}
```
public void setHideSuperscript(boolean value)
```


Se visualizzare il limite superiore

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setLimitLocation(int value) {#setLimitLocation-int-}
```
public void setLimitLocation(int value)
```


Questo attributo specifica la posizione dei limiti negli operatori n-ari. I limiti possono essere centrati sopra e sotto l'operatore n-ario, oppure posizionati appena a destra dell'operatore.

Vedi [EquationLimitLocationType](../../com.aspose.cells/equationlimitlocationtype).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setNaryGrow(boolean value) {#setNaryGrow-boolean-}
```
public void setNaryGrow(boolean value)
```


Questo attributo specifica la proprietà di crescita degli operatori n-ari a livello di documento. Quando disattivata, gli operatori n-ari come integrali e sommatorie non si espandono per corrispondere all'altezza del loro operando. Quando attivata, l'operatore n-ario cresce verticalmente per corrispondere all'altezza del suo operando.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setNaryOperator(String value) {#setNaryOperator-java.lang.String-}
```
public void setNaryOperator(String value)
```


un operatore n-ario. ad es. \"\\u922d?. Si consiglia vivamente di utilizzare l'attributo NaryOperatorType per impostare l'operatore n-ario. Utilizza questa impostazione di proprietà se non riesci a trovare il carattere necessario in un tipo noto.

**Remarks**

Va notato che questa proprietà accetta solo un carattere e, se vengono passati più caratteri, viene accettato solo il primo.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### setNaryOperatorType(int value) {#setNaryOperatorType-int-}
```
public void setNaryOperatorType(int value)
```


un operatore n-ario.e.g "\u922d?

Vedi [EquationMathematicalOperatorType](../../com.aspose.cells/equationmathematicaloperatortype).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setParentNode(EquationNode value) {#setParentNode-com.aspose.cells.EquationNode-}
```
public void setParentNode(EquationNode value)
```


Specifica il nodo genitore del nodo corrente

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| value | [EquationNode](../../com.aspose.cells/equationnode) |  |

### setWordArtStyle(int style) {#setWordArtStyle-int-}
```
public void setWordArtStyle(int style)
```


Imposta lo stile WordArt predefinito.

**Remarks**

Solo per il testo di forma/grafico.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| style | int | [PresetWordArtStyle](../../com.aspose.cells/presetwordartstyle). Lo stile WordArt predefinito. |

### toLaTeX() {#toLaTeX--}
```
public String toLaTeX()
```


Converti questa equazione in espressione LaTeX.

**Returns:**
java.lang.String
### toMathML() {#toMathML--}
```
public String toMathML()
```


Converti questa equazione in espressione MathML.

**Returns:**
java.lang.String -
### toString() {#toString--}
```
public String toString()
```




**Returns:**
java.lang.String
### wait() {#wait--}
```
public final void wait()
```




### wait(long arg0) {#wait-long-}
```
public final native void wait(long arg0)
```




**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

