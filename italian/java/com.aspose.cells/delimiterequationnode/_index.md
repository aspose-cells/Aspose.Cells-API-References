---
title: "DelimiterEquationNode"
second_title: "Riferimento API di Aspose.Cells per Java"
description: "Questa classe specifica l'equazione del delimitatore composta da delimitatori di apertura e chiusura come parentesi tonde, graffe, quadre e barre verticali e da un componente contenuto all'interno."
type: docs
url: /it/java/com.aspose.cells/delimiterequationnode/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.FontSetting](../../com.aspose.cells/fontsetting), [com.aspose.cells.EquationNode](../../com.aspose.cells/equationnode)
```
public class DelimiterEquationNode extends EquationNode
```

Questa classe specifica l'equazione del delimitatore, composta da delimitatori di apertura e chiusura (come parentesi tonde, graffe, quadre e barre verticali) e da un componente contenuto all'interno. Il delimitatore può avere più di un componente, con un carattere separatore designato tra ciascun componente.
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [addChild(EquationNode node)](#addChild-com.aspose.cells.EquationNode-) | Inserisce il nodo specificato alla fine dell'elenco dei nodi figlio del nodo corrente. |
| [addChild(int equationType)](#addChild-int-) | Inserisci un nodo del tipo specificato alla fine dell'elenco dei nodi figlio del nodo corrente. |
| [createNode(int equationType, Workbook workbook, EquationNode parent)](#createNode-int-com.aspose.cells.Workbook-com.aspose.cells.EquationNode-) | Crea un nodo del tipo specificato. |
| [equals(Object obj)](#equals-java.lang.Object-) | Determina se il nodo dell'equazione corrente è uguale al nodo specificato |
| [getBeginChar()](#getBeginChar--) | Carattere iniziale del delimitatore. |
| [getChild(int index)](#getChild-int-) | Restituisce il nodo all'indice specificato tra i figli del nodo corrente. |
| [getClass()](#getClass--) |  |
| [getDelimiterShape()](#getDelimiterShape--) | Specifica la forma dei delimitatori nell'oggetto delimitatore. |
| [getEndChar()](#getEndChar--) | Carattere finale del delimitatore. |
| [getEquationType()](#getEquationType--) | Ottieni il tipo di equazione del nodo corrente |
| [getFont()](#getFont--) | Restituisce il carattere di questo oggetto. |
| [getLength()](#getLength--) | Ottiene la lunghezza dei caratteri. |
| [getNaryGrow()](#getNaryGrow--) | Specifica se il delimitatore deve espandersi e contrarsi automaticamente con l'altezza della formula. |
| [getParentNode()](#getParentNode--) | Specifica il nodo genitore del nodo corrente |
| [getSeparatorChar()](#getSeparatorChar--) | Carattere separatore del delimitatore. |
| [getStartIndex()](#getStartIndex--) | Ottiene l'indice di inizio dei caratteri. |
| [getTextOptions()](#getTextOptions--) | Restituisce le opzioni di testo. |
| [getType()](#getType--) | Rappresenta il tipo del nodo. |
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
| [setBeginChar(String value)](#setBeginChar-java.lang.String-) | Carattere iniziale del delimitatore. |
| [setDelimiterShape(int value)](#setDelimiterShape-int-) | Specifica la forma dei delimitatori nell'oggetto delimitatore. |
| [setEndChar(String value)](#setEndChar-java.lang.String-) | Carattere finale del delimitatore. |
| [setNaryGrow(boolean value)](#setNaryGrow-boolean-) | Specifica se il delimitatore deve espandersi e contrarsi automaticamente con l'altezza della formula. |
| [setParentNode(EquationNode value)](#setParentNode-com.aspose.cells.EquationNode-) | Specifica il nodo genitore del nodo corrente |
| [setSeparatorChar(String value)](#setSeparatorChar-java.lang.String-) | Carattere separatore del delimitatore. |
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
### getBeginChar() {#getBeginChar--}
```
public String getBeginChar()
```


Carattere iniziale del delimitatore.

**Remarks**

Va notato che questa proprietà accetta solo un carattere e, se vengono passati più caratteri, viene accettato solo il primo.

**Returns:**
java.lang.String
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
### getDelimiterShape() {#getDelimiterShape--}
```
public int getDelimiterShape()
```


Specifica la forma dei delimitatori nell'oggetto delimitatore.

Vedi [EquationDelimiterShapeType](../../com.aspose.cells/equationdelimitershapetype).

**Returns:**
int
### getEndChar() {#getEndChar--}
```
public String getEndChar()
```


Carattere finale del delimitatore.

**Remarks**

Va notato che questa proprietà accetta solo un carattere e, se vengono passati più caratteri, viene accettato solo il primo.

**Returns:**
java.lang.String
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
### getNaryGrow() {#getNaryGrow--}
```
public boolean getNaryGrow()
```


Specifica se il delimitatore deve espandersi e contrarsi automaticamente con l'altezza della formula.

**Remarks**

Questa proprietà specifica la proprietà di crescita del delimitatore a livello di documento. Quando disattivata, il delimitatore non crescerà per corrispondere alle dimensioni dell'altezza del suo componente. Quando abilitata, il delimitatore cresce verticalmente per corrispondere all'altezza del suo componente.

**Returns:**
boolean
### getParentNode() {#getParentNode--}
```
public EquationNode getParentNode()
```


Specifica il nodo genitore del nodo corrente

**Returns:**
[EquationNode](../../com.aspose.cells/equationnode)
### getSeparatorChar() {#getSeparatorChar--}
```
public String getSeparatorChar()
```


Carattere separatore del delimitatore.

**Remarks**

Va notato che questa proprietà accetta solo un carattere e, se vengono passati più caratteri, viene accettato solo il primo.

**Returns:**
java.lang.String
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

### setBeginChar(String value) {#setBeginChar-java.lang.String-}
```
public void setBeginChar(String value)
```


Carattere iniziale del delimitatore.

**Remarks**

Va notato che questa proprietà accetta solo un carattere e, se vengono passati più caratteri, viene accettato solo il primo.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### setDelimiterShape(int value) {#setDelimiterShape-int-}
```
public void setDelimiterShape(int value)
```


Specifica la forma dei delimitatori nell'oggetto delimitatore.

Vedi [EquationDelimiterShapeType](../../com.aspose.cells/equationdelimitershapetype).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setEndChar(String value) {#setEndChar-java.lang.String-}
```
public void setEndChar(String value)
```


Carattere finale del delimitatore.

**Remarks**

Va notato che questa proprietà accetta solo un carattere e, se vengono passati più caratteri, viene accettato solo il primo.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### setNaryGrow(boolean value) {#setNaryGrow-boolean-}
```
public void setNaryGrow(boolean value)
```


Specifica se il delimitatore deve espandersi e contrarsi automaticamente con l'altezza della formula.

**Remarks**

Questa proprietà specifica la proprietà di crescita del delimitatore a livello di documento. Quando disattivata, il delimitatore non crescerà per corrispondere alle dimensioni dell'altezza del suo componente. Quando abilitata, il delimitatore cresce verticalmente per corrispondere all'altezza del suo componente.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setParentNode(EquationNode value) {#setParentNode-com.aspose.cells.EquationNode-}
```
public void setParentNode(EquationNode value)
```


Specifica il nodo genitore del nodo corrente

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| value | [EquationNode](../../com.aspose.cells/equationnode) |  |

### setSeparatorChar(String value) {#setSeparatorChar-java.lang.String-}
```
public void setSeparatorChar(String value)
```


Carattere separatore del delimitatore.

**Remarks**

Va notato che questa proprietà accetta solo un carattere e, se vengono passati più caratteri, viene accettato solo il primo.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

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

