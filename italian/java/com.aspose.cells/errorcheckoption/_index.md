---
title: "ErrorCheckOption"
second_title: "Riferimento API di Aspose.Cells per Java"
description: "Impostazione di verifica errori applicata a determinati intervalli."
type: docs
url: /it/java/com.aspose.cells/errorcheckoption/
---

**Inheritance:**
java.lang.Object
```
public class ErrorCheckOption
```

Impostazione di verifica errori applicata a determinati intervalli.

**Example**

```
           Workbook workbook = new Workbook();
           ErrorCheckOptionCollection opts = workbook.getWorksheets().get(0).getErrorCheckOptions();
           int optionIdx = opts.add();
           ErrorCheckOption opt = opts.get(optionIdx);
           opt.setErrorCheck(com.aspose.cells.ErrorCheckType.INCONSIST_FORMULA, false);
           opt.setErrorCheck(com.aspose.cells.ErrorCheckType.INCONSIST_RANGE, false);
           opt.setErrorCheck(com.aspose.cells.ErrorCheckType.TEXT_DATE, false);
           opt.setErrorCheck(com.aspose.cells.ErrorCheckType.TEXT_NUMBER, false);
           opt.setErrorCheck(com.aspose.cells.ErrorCheckType.VALIDATION, false);
           opt.addRange(CellArea.createCellArea("A1", "B10"));
           workbook.save("Book1.xlsx");
```
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [addRange(CellArea ca)](#addRange-com.aspose.cells.CellArea-) | Aggiunge un intervallo influenzato da questa impostazione. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getCountOfRange()](#getCountOfRange--) | Ottiene il conteggio degli intervalli influenzati da questa impostazione. |
| [getRange(int index)](#getRange-int-) | Ottiene l'intervallo influenzato da questa impostazione per l'indice fornito. |
| [hashCode()](#hashCode--) |  |
| [isErrorCheck(int errorCheckType)](#isErrorCheck-int-) | Verifica se il tipo di errore fornito verrà controllato. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [removeRange(int index)](#removeRange-int-) | Rimuove un intervallo per l'indice fornito. |
| [setErrorCheck(int errorCheckType, boolean isCheck)](#setErrorCheck-int-boolean-) | Imposta se il tipo di errore fornito verrà controllato. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### addRange(CellArea ca) {#addRange-com.aspose.cells.CellArea-}
```
public int addRange(CellArea ca)
```


Aggiunge un intervallo influenzato da questa impostazione.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| ca | [CellArea](../../com.aspose.cells/cellarea) | l'intervallo da aggiungere. |

**Returns:**
int - l'indice dell'intervallo aggiunto nell'elenco degli intervalli di questa impostazione.
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
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getCountOfRange() {#getCountOfRange--}
```
public int getCountOfRange()
```


Ottiene il conteggio degli intervalli influenzati da questa impostazione.

**Returns:**
int - il conteggio degli intervalli influenzati da questa impostazione.
### getRange(int index) {#getRange-int-}
```
public CellArea getRange(int index)
```


Ottiene l'intervallo influenzato da questa impostazione per l'indice fornito.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| indice | int | l'indice dell'intervallo |

**Returns:**
[CellArea](../../com.aspose.cells/cellarea) - return influenced range at given index.
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isErrorCheck(int errorCheckType) {#isErrorCheck-int-}
```
public boolean isErrorCheck(int errorCheckType)
```


Verifica se il tipo di errore fornito verrà controllato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| errorCheckType | int | [ErrorCheckType](../../com.aspose.cells/errorchecktype). il tipo di errore può essere controllato |

**Returns:**
boolean - restituisce true se il tipo di errore specificato verrà controllato (verrà mostrato un triangolo verde nella cella se il controllo fallisce).
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### removeRange(int index) {#removeRange-int-}
```
public void removeRange(int index)
```


Rimuove un intervallo per l'indice fornito.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| indice | int | l'indice dell'intervallo da rimuovere. |

### setErrorCheck(int errorCheckType, boolean isCheck) {#setErrorCheck-int-boolean-}
```
public void setErrorCheck(int errorCheckType, boolean isCheck)
```


Imposta se il tipo di errore fornito verrà controllato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| errorCheckType | int | [ErrorCheckType](../../com.aspose.cells/errorchecktype). il tipo di errore può essere controllato. |
| isCheck | boolean | true se il tipo di errore specificato deve essere controllato (verrà mostrato un triangolo verde nella cella se il controllo fallisce). |

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

