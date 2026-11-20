---
title: "GroupCharacterEquationNode"
second_title: "Riferimento API di Aspose.Cells per Java"
description: "Questa classe specifica la funzione Group-Character composta da un carattere disegnato sopra o sotto il testo, spesso con lo scopo di raggruppare visivamente gli elementi."
type: docs
url: /it/java/com.aspose.cells/groupcharacterequationnode/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.FontSetting](../../com.aspose.cells/fontsetting), [com.aspose.cells.EquationNode](../../com.aspose.cells/equationnode)
```
public class GroupCharacterEquationNode extends EquationNode
```

Questa classe specifica la funzione Group-Character, composta da un carattere disegnato sopra o sotto il testo, spesso con lo scopo di raggruppare visivamente gli elementi.
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [addChild(EquationNode node)](#addChild-com.aspose.cells.EquationNode-) | Inserisce il nodo specificato alla fine dell'elenco dei nodi figlio del nodo corrente. |
| [addChild(int equationType)](#addChild-int-) | Inserisci un nodo del tipo specificato alla fine dell'elenco dei nodi figlio del nodo corrente. |
| [createNode(int equationType, Workbook workbook, EquationNode parent)](#createNode-int-com.aspose.cells.Workbook-com.aspose.cells.EquationNode-) | Crea un nodo del tipo specificato. |
| [equals(Object obj)](#equals-java.lang.Object-) | Determina se il nodo dell'equazione corrente è uguale al nodo specificato |
| [getChild(int index)](#getChild-int-) | Restituisce il nodo all'indice specificato tra i figli del nodo corrente. |
| [getChrType()](#getChrType--) | Specifica i caratteri combinanti per valore di tipo. |
| [getClass()](#getClass--) |  |
| [getEquationType()](#getEquationType--) | Ottieni il tipo di equazione del nodo corrente |
| [getFont()](#getFont--) | Restituisce il carattere di questo oggetto. |
| [getGroupChr()](#getGroupChr--) | Specifica un simbolo (predefinito U+23DF). |
| [getLength()](#getLength--) | Ottiene la lunghezza dei caratteri. |
| [getParentNode()](#getParentNode--) | Specifica il nodo genitore del nodo corrente |
| [getPosition()](#getPosition--) | Questo attributo specifica la posizione del carattere nell'oggetto |
| [getStartIndex()](#getStartIndex--) | Ottiene l'indice di inizio dei caratteri. |
| [getTextOptions()](#getTextOptions--) | Restituisce le opzioni di testo. |
| [getType()](#getType--) | Rappresenta il tipo del nodo. |
| [getVertJc()](#getVertJc--) | Questo attributo, combinato con pos di groupChrPr, specifica il layout verticale dell'oggetto groupChr. |
| [hashCode()](#hashCode--) |  |
| [insertAfter(int equationType)](#insertAfter-int-) | Inserisce il nodo specificato dopo il nodo corrente. |
| [insertBefore(int equationType)](#insertBefore-int-) | Inserisce il nodo specificato prima del nodo corrente. |
| [insertChild(int index, int equationType)](#insertChild-int-int-) | Inserisce un nodo del tipo specificato nella posizione di indice specificata nell'elenco dei nodi figlio del nodo corrente. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [remove()](#remove--) | Si rimuove dal genitore. |
| [removeAllChildren()](#removeAllChildren--) | Rimuove tutti i nodi figlio del nodo corrente. |
| [removeChild(EquationNode node)](#removeChild-com.aspose.cells.EquationNode-) | Rimuove il nodo specificato dai figli del nodo corrente. |
| [removeChild(int index)](#removeChild-int-) | Rimuove il nodo all'indice specificato dai figli del nodo corrente. |
| [setChrType(int value)](#setChrType-int-) | Specifica i caratteri combinanti per valore di tipo. |
| [setGroupChr(String value)](#setGroupChr-java.lang.String-) | Specifica un simbolo (predefinito U+23DF). |
| [setParentNode(EquationNode value)](#setParentNode-com.aspose.cells.EquationNode-) | Specifica il nodo genitore del nodo corrente |
| [setPosition(int value)](#setPosition-int-) | Questo attributo specifica la posizione del carattere nell'oggetto |
| [setVertJc(int value)](#setVertJc-int-) | Questo attributo, combinato con pos di groupChrPr, specifica il layout verticale dell'oggetto groupChr. |
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
### getChrType() {#getChrType--}
```
public int getChrType()
```


Specifica i caratteri combinanti per valore di tipo.

Vedi [EquationCombiningCharacterType](../../com.aspose.cells/equationcombiningcharactertype).

**Returns:**
int
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
### getGroupChr() {#getGroupChr--}
```
public String getGroupChr()
```


Specifica un simbolo (predefinito U+23DF). Si consiglia vivamente di utilizzare l'attributo ChrType per impostare il carattere di accento. Utilizza questa impostazione della proprietà se non riesci a trovare il carattere necessario in un tipo noto.

**Remarks**

Va notato che questa proprietà accetta solo un carattere e, se vengono passati più caratteri, viene accettato solo il primo.

**Returns:**
java.lang.String
### getLength() {#getLength--}
```
public int getLength()
```


Ottiene la lunghezza dei caratteri.

**Returns:**
int
### getParentNode() {#getParentNode--}
```
public EquationNode getParentNode()
```


Specifica il nodo genitore del nodo corrente

**Returns:**
[EquationNode](../../com.aspose.cells/equationnode)
### getPosition() {#getPosition--}
```
public int getPosition()
```


Questo attributo specifica la posizione del carattere nell'oggetto

Vedi [EquationCharacterPositionType](../../com.aspose.cells/equationcharacterpositiontype).

**Returns:**
int
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
### getVertJc() {#getVertJc--}
```
public int getVertJc()
```


Questo attributo, combinato con pos di groupChrPr, specifica il layout verticale dell'oggetto groupChr. Dove pos specifica la posizione del carattere di raggruppamento, vertJc specifica l'allineamento dell'oggetto rispetto alla linea di base.

Vedi [EquationCharacterPositionType](../../com.aspose.cells/equationcharacterpositiontype).

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

### setChrType(int value) {#setChrType-int-}
```
public void setChrType(int value)
```


Specifica i caratteri combinanti per valore di tipo.

Vedi [EquationCombiningCharacterType](../../com.aspose.cells/equationcombiningcharactertype).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setGroupChr(String value) {#setGroupChr-java.lang.String-}
```
public void setGroupChr(String value)
```


Specifica un simbolo (predefinito U+23DF). Si consiglia vivamente di utilizzare l'attributo ChrType per impostare il carattere di accento. Utilizza questa impostazione della proprietà se non riesci a trovare il carattere necessario in un tipo noto.

**Remarks**

Va notato che questa proprietà accetta solo un carattere e, se vengono passati più caratteri, viene accettato solo il primo.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### setParentNode(EquationNode value) {#setParentNode-com.aspose.cells.EquationNode-}
```
public void setParentNode(EquationNode value)
```


Specifica il nodo genitore del nodo corrente

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| value | [EquationNode](../../com.aspose.cells/equationnode) |  |

### setPosition(int value) {#setPosition-int-}
```
public void setPosition(int value)
```


Questo attributo specifica la posizione del carattere nell'oggetto

Vedi [EquationCharacterPositionType](../../com.aspose.cells/equationcharacterpositiontype).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setVertJc(int value) {#setVertJc-int-}
```
public void setVertJc(int value)
```


Questo attributo, combinato con pos di groupChrPr, specifica il layout verticale dell'oggetto groupChr. Dove pos specifica la posizione del carattere di raggruppamento, vertJc specifica l'allineamento dell'oggetto rispetto alla linea di base.

Vedi [EquationCharacterPositionType](../../com.aspose.cells/equationcharacterpositiontype).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

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

