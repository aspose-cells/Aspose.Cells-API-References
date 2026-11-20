---
title: "FormulaParseOptions"
second_title: "Riferimento API di Aspose.Cells per Java"
description: "Rappresenta le opzioni durante l'analisi della formula."
type: docs
url: /it/java/com.aspose.cells/formulaparseoptions/
---

**Inheritance:**
java.lang.Object
```
public class FormulaParseOptions
```

Rappresenta le opzioni durante l'analisi della formula.
## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [FormulaParseOptions()](#FormulaParseOptions--) |  |
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getCheckAddIn()](#getCheckAddIn--) | Indica se verificare i componenti aggiuntivi nei collegamenti esterni esistenti della cartella di lavoro corrente per le funzioni definite dall'utente senza collegamento esterno. |
| [getClass()](#getClass--) |  |
| [getCustomFunctionDefinition()](#getCustomFunctionDefinition--) | Definizione per l'analisi delle funzioni personalizzate. |
| [getLocaleDependent()](#getLocaleDependent--) | Se la formula è formattata per la locale. |
| [getParse()](#getParse--) | Indica se analizzare la formula fornita. |
| [getR1C1Style()](#getR1C1Style--) | Indica se la formula è nello stile di riferimento R1C1. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setCheckAddIn(boolean value)](#setCheckAddIn-boolean-) | Indica se verificare i componenti aggiuntivi nei collegamenti esterni esistenti della cartella di lavoro corrente per le funzioni definite dall'utente senza collegamento esterno. |
| [setCustomFunctionDefinition(CustomFunctionDefinition value)](#setCustomFunctionDefinition-com.aspose.cells.CustomFunctionDefinition-) | Definizione per l'analisi delle funzioni personalizzate. |
| [setLocaleDependent(boolean value)](#setLocaleDependent-boolean-) | Se la formula è formattata per la locale. |
| [setParse(boolean value)](#setParse-boolean-) | Indica se analizzare la formula fornita. |
| [setR1C1Style(boolean value)](#setR1C1Style-boolean-) | Indica se la formula è nello stile di riferimento R1C1. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### FormulaParseOptions() {#FormulaParseOptions--}
```
public FormulaParseOptions()
```


### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| arg0 | java.lang.Object |  |

**Returns:**
boolean
### getCheckAddIn() {#getCheckAddIn--}
```
public boolean getCheckAddIn()
```


Indica se verificare i componenti aggiuntivi nei collegamenti esterni esistenti della cartella di lavoro corrente per le funzioni definite dall'utente senza collegamento esterno. Il valore predefinito è true (se la funzione definita dall'utente corrisponde a un componente aggiuntivo nei collegamenti esterni esistenti, allora viene considerata come tale).

**Returns:**
boolean
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getCustomFunctionDefinition() {#getCustomFunctionDefinition--}
```
public CustomFunctionDefinition getCustomFunctionDefinition()
```


Definizione per l'analisi delle funzioni personalizzate.

**Remarks**

Per alcuni requisiti speciali, come quando si calcola una funzione personalizzata nel motore personalizzato dell'utente, alcuni parametri devono essere calcolati in modalità array; l'utilizzo di questa proprietà può contrassegnare tali parametri come modalità array durante l'analisi della formula. In caso contrario, l'utente deve aggiornare successivamente quelle funzioni personalizzate tramite [Workbook.updateCustomFunctionDefinition(CustomFunctionDefinition)](../../com.aspose.cells/workbook\#updateCustomFunctionDefinition-CustomFunctionDefinition-) per ottenere lo stesso risultato.

**Returns:**
[CustomFunctionDefinition](../../com.aspose.cells/customfunctiondefinition)
### getLocaleDependent() {#getLocaleDependent--}
```
public boolean getLocaleDependent()
```


Indica se la formula è formattata per la lingua locale. Il valore predefinito è false.

**Returns:**
boolean
### getParse() {#getParse--}
```
public boolean getParse()
```


Indica se analizzare la formula fornita. Il valore predefinito è true. Se è false, la stringa della formula fornita verrà mantenuta così com'è per la cella finché l'utente non chiamerà altri metodi per analizzarla o finché i dati della formula analizzata non saranno richiesti da altre operazioni, come il calcolo delle formule.

**Returns:**
boolean
### getR1C1Style() {#getR1C1Style--}
```
public boolean getR1C1Style()
```


Indica se la formula è nello stile di riferimento R1C1. Il valore predefinito è false.

**Returns:**
boolean
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### setCheckAddIn(boolean value) {#setCheckAddIn-boolean-}
```
public void setCheckAddIn(boolean value)
```


Indica se verificare i componenti aggiuntivi nei collegamenti esterni esistenti della cartella di lavoro corrente per le funzioni definite dall'utente senza collegamento esterno. Il valore predefinito è true (se la funzione definita dall'utente corrisponde a un componente aggiuntivo nei collegamenti esterni esistenti, allora viene considerata come tale).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setCustomFunctionDefinition(CustomFunctionDefinition value) {#setCustomFunctionDefinition-com.aspose.cells.CustomFunctionDefinition-}
```
public void setCustomFunctionDefinition(CustomFunctionDefinition value)
```


Definizione per l'analisi delle funzioni personalizzate.

**Remarks**

Per alcuni requisiti speciali, come quando si calcola una funzione personalizzata nel motore personalizzato dell'utente, alcuni parametri devono essere calcolati in modalità array; l'utilizzo di questa proprietà può contrassegnare tali parametri come modalità array durante l'analisi della formula. In caso contrario, l'utente deve aggiornare successivamente quelle funzioni personalizzate tramite [Workbook.updateCustomFunctionDefinition(CustomFunctionDefinition)](../../com.aspose.cells/workbook\#updateCustomFunctionDefinition-CustomFunctionDefinition-) per ottenere lo stesso risultato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| value | [CustomFunctionDefinition](../../com.aspose.cells/customfunctiondefinition) |  |

### setLocaleDependent(boolean value) {#setLocaleDependent-boolean-}
```
public void setLocaleDependent(boolean value)
```


Indica se la formula è formattata per la lingua locale. Il valore predefinito è false.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setParse(boolean value) {#setParse-boolean-}
```
public void setParse(boolean value)
```


Indica se analizzare la formula fornita. Il valore predefinito è true. Se è false, la stringa della formula fornita verrà mantenuta così com'è per la cella finché l'utente non chiamerà altri metodi per analizzarla o finché i dati della formula analizzata non saranno richiesti da altre operazioni, come il calcolo delle formule.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setR1C1Style(boolean value) {#setR1C1Style-boolean-}
```
public void setR1C1Style(boolean value)
```


Indica se la formula è nello stile di riferimento R1C1. Il valore predefinito è false.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

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

