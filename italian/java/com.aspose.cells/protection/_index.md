---
title: "Protezione"
second_title: "Riferimento API di Aspose.Cells per Java"
description: "Rappresenta i vari tipi di opzioni di protezione disponibili per un foglio di lavoro."
type: docs
url: /it/java/com.aspose.cells/protection/
---

**Inheritance:**
java.lang.Object
```
public class Protection
```

Rappresenta i vari tipi di opzioni di protezione disponibili per un foglio di lavoro.

**Example**

```
         //Instantiating a Workbook object
         Workbook workbook = new Workbook();
 
         Worksheet worksheet = workbook.getWorksheets().get(0);
         //Allowing users to select locked cells of the worksheet
         worksheet.getProtection().setAllowSelectingLockedCell(true);
         //Allowing users to select unlocked cells of the worksheet
         worksheet.getProtection().setAllowSelectingUnlockedCell(true);
```
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [copy(Protection source)](#copy-com.aspose.cells.Protection-) | Copia le informazioni di protezione. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAllowDeletingColumn()](#getAllowDeletingColumn--) | Rappresenta se l'eliminazione delle colonne è consentita su un foglio di lavoro protetto. |
| [getAllowDeletingRow()](#getAllowDeletingRow--) | Rappresenta se l'eliminazione delle righe è consentita su un foglio di lavoro protetto. |
| [getAllowEditingContent()](#getAllowEditingContent--) | Rappresenta se all'utente è consentito modificare il contenuto delle celle bloccate su un foglio di lavoro protetto. |
| [getAllowEditingObject()](#getAllowEditingObject--) | Rappresenta se all'utente è consentito manipolare gli oggetti di disegno su un foglio di lavoro protetto. |
| [getAllowEditingScenario()](#getAllowEditingScenario--) | Rappresenta se all'utente è consentito modificare gli scenari su un foglio di lavoro protetto. |
| [getAllowFiltering()](#getAllowFiltering--) | Rappresenta se all'utente è consentito utilizzare un AutoFilter creato prima che il foglio fosse protetto. |
| [getAllowFormattingCell()](#getAllowFormattingCell--) | Rappresenta se la formattazione delle celle è consentita su un foglio di lavoro protetto. |
| [getAllowFormattingColumn()](#getAllowFormattingColumn--) | Rappresenta se la formattazione delle colonne è consentita su un foglio di lavoro protetto |
| [getAllowFormattingRow()](#getAllowFormattingRow--) | Rappresenta se la formattazione delle righe è consentita su un foglio di lavoro protetto |
| [getAllowInsertingColumn()](#getAllowInsertingColumn--) | Rappresenta se l'inserimento delle colonne è consentito su un foglio di lavoro protetto |
| [getAllowInsertingHyperlink()](#getAllowInsertingHyperlink--) | Rappresenta se l'inserimento di collegamenti ipertestuali è consentito in un foglio di lavoro protetto |
| [getAllowInsertingRow()](#getAllowInsertingRow--) | Rappresenta se l'inserimento di righe è consentito in un foglio di lavoro protetto |
| [getAllowSelectingLockedCell()](#getAllowSelectingLockedCell--) | Rappresenta se all'utente è consentito selezionare le celle bloccate in un foglio di lavoro protetto. |
| [getAllowSelectingUnlockedCell()](#getAllowSelectingUnlockedCell--) | Rappresenta se all'utente è consentito selezionare le celle sbloccate in un foglio di lavoro protetto. |
| [getAllowSorting()](#getAllowSorting--) | Rappresenta se l'opzione di ordinamento è consentita in un foglio di lavoro protetto. |
| [getAllowUsingPivotTable()](#getAllowUsingPivotTable--) | Rappresenta se all'utente è consentito manipolare le tabelle pivot in un foglio di lavoro protetto. |
| [getClass()](#getClass--) |  |
| [getPassword()](#getPassword--) | Rappresenta la password per proteggere il foglio di lavoro. |
| [getPasswordHash()](#getPasswordHash--) | Ottiene l'hash della password corrente. |
| [hashCode()](#hashCode--) |  |
| [isProtectedWithPassword()](#isProtectedWithPassword--) | Indica se il foglio di lavoro è protetto da password. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAllowDeletingColumn(boolean value)](#setAllowDeletingColumn-boolean-) | Rappresenta se l'eliminazione delle colonne è consentita su un foglio di lavoro protetto. |
| [setAllowDeletingRow(boolean value)](#setAllowDeletingRow-boolean-) | Rappresenta se l'eliminazione delle righe è consentita su un foglio di lavoro protetto. |
| [setAllowEditingContent(boolean value)](#setAllowEditingContent-boolean-) | Rappresenta se all'utente è consentito modificare il contenuto delle celle bloccate su un foglio di lavoro protetto. |
| [setAllowEditingObject(boolean value)](#setAllowEditingObject-boolean-) | Rappresenta se all'utente è consentito manipolare gli oggetti di disegno su un foglio di lavoro protetto. |
| [setAllowEditingScenario(boolean value)](#setAllowEditingScenario-boolean-) | Rappresenta se all'utente è consentito modificare gli scenari su un foglio di lavoro protetto. |
| [setAllowFiltering(boolean value)](#setAllowFiltering-boolean-) | Rappresenta se all'utente è consentito utilizzare un AutoFilter creato prima che il foglio fosse protetto. |
| [setAllowFormattingCell(boolean value)](#setAllowFormattingCell-boolean-) | Rappresenta se la formattazione delle celle è consentita su un foglio di lavoro protetto. |
| [setAllowFormattingColumn(boolean value)](#setAllowFormattingColumn-boolean-) | Rappresenta se la formattazione delle colonne è consentita su un foglio di lavoro protetto |
| [setAllowFormattingRow(boolean value)](#setAllowFormattingRow-boolean-) | Rappresenta se la formattazione delle righe è consentita su un foglio di lavoro protetto |
| [setAllowInsertingColumn(boolean value)](#setAllowInsertingColumn-boolean-) | Rappresenta se l'inserimento delle colonne è consentito su un foglio di lavoro protetto |
| [setAllowInsertingHyperlink(boolean value)](#setAllowInsertingHyperlink-boolean-) | Rappresenta se l'inserimento di collegamenti ipertestuali è consentito in un foglio di lavoro protetto |
| [setAllowInsertingRow(boolean value)](#setAllowInsertingRow-boolean-) | Rappresenta se l'inserimento di righe è consentito in un foglio di lavoro protetto |
| [setAllowSelectingLockedCell(boolean value)](#setAllowSelectingLockedCell-boolean-) | Rappresenta se all'utente è consentito selezionare le celle bloccate in un foglio di lavoro protetto. |
| [setAllowSelectingUnlockedCell(boolean value)](#setAllowSelectingUnlockedCell-boolean-) | Rappresenta se all'utente è consentito selezionare le celle sbloccate in un foglio di lavoro protetto. |
| [setAllowSorting(boolean value)](#setAllowSorting-boolean-) | Rappresenta se l'opzione di ordinamento è consentita in un foglio di lavoro protetto. |
| [setAllowUsingPivotTable(boolean value)](#setAllowUsingPivotTable-boolean-) | Rappresenta se all'utente è consentito manipolare le tabelle pivot in un foglio di lavoro protetto. |
| [setPassword(String value)](#setPassword-java.lang.String-) | Rappresenta la password per proteggere il foglio di lavoro. |
| [toString()](#toString--) |  |
| [verifyPassword(String password)](#verifyPassword-java.lang.String-) | Verifica la password. |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### copy(Protection source) {#copy-com.aspose.cells.Protection-}
```
public void copy(Protection source)
```


Copia le informazioni di protezione.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| source | [Protection](../../com.aspose.cells/protection) |  |

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
### getAllowDeletingColumn() {#getAllowDeletingColumn--}
```
public boolean getAllowDeletingColumn()
```


Rappresenta se l'eliminazione delle colonne è consentita su un foglio di lavoro protetto.

**Remarks**

Le colonne contenenti le celle da eliminare devono essere sbloccate quando il foglio è protetto, e l'opzione "Seleziona celle sbloccate" deve essere abilitata.

**Returns:**
boolean
### getAllowDeletingRow() {#getAllowDeletingRow--}
```
public boolean getAllowDeletingRow()
```


Rappresenta se l'eliminazione delle righe è consentita su un foglio di lavoro protetto.

**Remarks**

Le righe contenenti le celle da eliminare devono essere sbloccate quando il foglio è protetto, e l'opzione "Seleziona celle sbloccate" deve essere abilitata.

**Returns:**
boolean
### getAllowEditingContent() {#getAllowEditingContent--}
```
public boolean getAllowEditingContent()
```


Rappresenta se all'utente è consentito modificare il contenuto delle celle bloccate su un foglio di lavoro protetto.

**Returns:**
boolean
### getAllowEditingObject() {#getAllowEditingObject--}
```
public boolean getAllowEditingObject()
```


Rappresenta se all'utente è consentito manipolare gli oggetti di disegno su un foglio di lavoro protetto.

**Returns:**
boolean
### getAllowEditingScenario() {#getAllowEditingScenario--}
```
public boolean getAllowEditingScenario()
```


Rappresenta se all'utente è consentito modificare gli scenari su un foglio di lavoro protetto.

**Returns:**
boolean
### getAllowFiltering() {#getAllowFiltering--}
```
public boolean getAllowFiltering()
```


Rappresenta se all'utente è consentito utilizzare un AutoFilter creato prima che il foglio fosse protetto.

**Returns:**
boolean
### getAllowFormattingCell() {#getAllowFormattingCell--}
```
public boolean getAllowFormattingCell()
```


Rappresenta se la formattazione delle celle è consentita su un foglio di lavoro protetto.

**Returns:**
boolean
### getAllowFormattingColumn() {#getAllowFormattingColumn--}
```
public boolean getAllowFormattingColumn()
```


Rappresenta se la formattazione delle colonne è consentita su un foglio di lavoro protetto

**Returns:**
boolean
### getAllowFormattingRow() {#getAllowFormattingRow--}
```
public boolean getAllowFormattingRow()
```


Rappresenta se la formattazione delle righe è consentita su un foglio di lavoro protetto

**Returns:**
boolean
### getAllowInsertingColumn() {#getAllowInsertingColumn--}
```
public boolean getAllowInsertingColumn()
```


Rappresenta se l'inserimento delle colonne è consentito su un foglio di lavoro protetto

**Returns:**
boolean
### getAllowInsertingHyperlink() {#getAllowInsertingHyperlink--}
```
public boolean getAllowInsertingHyperlink()
```


Rappresenta se l'inserimento di collegamenti ipertestuali è consentito in un foglio di lavoro protetto

**Returns:**
boolean
### getAllowInsertingRow() {#getAllowInsertingRow--}
```
public boolean getAllowInsertingRow()
```


Rappresenta se l'inserimento di righe è consentito in un foglio di lavoro protetto

**Returns:**
boolean
### getAllowSelectingLockedCell() {#getAllowSelectingLockedCell--}
```
public boolean getAllowSelectingLockedCell()
```


Rappresenta se all'utente è consentito selezionare le celle bloccate in un foglio di lavoro protetto.

**Returns:**
boolean
### getAllowSelectingUnlockedCell() {#getAllowSelectingUnlockedCell--}
```
public boolean getAllowSelectingUnlockedCell()
```


Rappresenta se all'utente è consentito selezionare le celle sbloccate in un foglio di lavoro protetto.

**Returns:**
boolean
### getAllowSorting() {#getAllowSorting--}
```
public boolean getAllowSorting()
```


Rappresenta se l'opzione di ordinamento è consentita in un foglio di lavoro protetto.

**Returns:**
boolean
### getAllowUsingPivotTable() {#getAllowUsingPivotTable--}
```
public boolean getAllowUsingPivotTable()
```


Rappresenta se all'utente è consentito manipolare le tabelle pivot in un foglio di lavoro protetto.

**Returns:**
boolean
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getPassword() {#getPassword--}
```
public String getPassword()
```


Rappresenta la password per proteggere il foglio di lavoro.

**Remarks**

Se la password è impostata a null o a stringa vuota, è possibile deproteggere il foglio di lavoro o la cartella di lavoro senza usare una password. Altrimenti, è necessario specificare la password per deproteggere il foglio di lavoro o la cartella di lavoro.

**Returns:**
java.lang.String
### getPasswordHash() {#getPasswordHash--}
```
public int getPasswordHash()
```


Ottiene l'hash della password corrente.

**Returns:**
int
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isProtectedWithPassword() {#isProtectedWithPassword--}
```
public boolean isProtectedWithPassword()
```


Indica se il foglio di lavoro è protetto da password.

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




### setAllowDeletingColumn(boolean value) {#setAllowDeletingColumn-boolean-}
```
public void setAllowDeletingColumn(boolean value)
```


Rappresenta se l'eliminazione delle colonne è consentita su un foglio di lavoro protetto.

**Remarks**

Le colonne contenenti le celle da eliminare devono essere sbloccate quando il foglio è protetto, e l'opzione "Seleziona celle sbloccate" deve essere abilitata.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setAllowDeletingRow(boolean value) {#setAllowDeletingRow-boolean-}
```
public void setAllowDeletingRow(boolean value)
```


Rappresenta se l'eliminazione delle righe è consentita su un foglio di lavoro protetto.

**Remarks**

Le righe contenenti le celle da eliminare devono essere sbloccate quando il foglio è protetto, e l'opzione "Seleziona celle sbloccate" deve essere abilitata.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setAllowEditingContent(boolean value) {#setAllowEditingContent-boolean-}
```
public void setAllowEditingContent(boolean value)
```


Rappresenta se all'utente è consentito modificare il contenuto delle celle bloccate su un foglio di lavoro protetto.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setAllowEditingObject(boolean value) {#setAllowEditingObject-boolean-}
```
public void setAllowEditingObject(boolean value)
```


Rappresenta se all'utente è consentito manipolare gli oggetti di disegno su un foglio di lavoro protetto.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setAllowEditingScenario(boolean value) {#setAllowEditingScenario-boolean-}
```
public void setAllowEditingScenario(boolean value)
```


Rappresenta se all'utente è consentito modificare gli scenari su un foglio di lavoro protetto.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setAllowFiltering(boolean value) {#setAllowFiltering-boolean-}
```
public void setAllowFiltering(boolean value)
```


Rappresenta se all'utente è consentito utilizzare un AutoFilter creato prima che il foglio fosse protetto.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setAllowFormattingCell(boolean value) {#setAllowFormattingCell-boolean-}
```
public void setAllowFormattingCell(boolean value)
```


Rappresenta se la formattazione delle celle è consentita su un foglio di lavoro protetto.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setAllowFormattingColumn(boolean value) {#setAllowFormattingColumn-boolean-}
```
public void setAllowFormattingColumn(boolean value)
```


Rappresenta se la formattazione delle colonne è consentita su un foglio di lavoro protetto

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setAllowFormattingRow(boolean value) {#setAllowFormattingRow-boolean-}
```
public void setAllowFormattingRow(boolean value)
```


Rappresenta se la formattazione delle righe è consentita su un foglio di lavoro protetto

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setAllowInsertingColumn(boolean value) {#setAllowInsertingColumn-boolean-}
```
public void setAllowInsertingColumn(boolean value)
```


Rappresenta se l'inserimento delle colonne è consentito su un foglio di lavoro protetto

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setAllowInsertingHyperlink(boolean value) {#setAllowInsertingHyperlink-boolean-}
```
public void setAllowInsertingHyperlink(boolean value)
```


Rappresenta se l'inserimento di collegamenti ipertestuali è consentito in un foglio di lavoro protetto

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setAllowInsertingRow(boolean value) {#setAllowInsertingRow-boolean-}
```
public void setAllowInsertingRow(boolean value)
```


Rappresenta se l'inserimento di righe è consentito in un foglio di lavoro protetto

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setAllowSelectingLockedCell(boolean value) {#setAllowSelectingLockedCell-boolean-}
```
public void setAllowSelectingLockedCell(boolean value)
```


Rappresenta se all'utente è consentito selezionare le celle bloccate in un foglio di lavoro protetto.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setAllowSelectingUnlockedCell(boolean value) {#setAllowSelectingUnlockedCell-boolean-}
```
public void setAllowSelectingUnlockedCell(boolean value)
```


Rappresenta se all'utente è consentito selezionare le celle sbloccate in un foglio di lavoro protetto.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setAllowSorting(boolean value) {#setAllowSorting-boolean-}
```
public void setAllowSorting(boolean value)
```


Rappresenta se l'opzione di ordinamento è consentita in un foglio di lavoro protetto.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setAllowUsingPivotTable(boolean value) {#setAllowUsingPivotTable-boolean-}
```
public void setAllowUsingPivotTable(boolean value)
```


Rappresenta se all'utente è consentito manipolare le tabelle pivot in un foglio di lavoro protetto.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setPassword(String value) {#setPassword-java.lang.String-}
```
public void setPassword(String value)
```


Rappresenta la password per proteggere il foglio di lavoro.

**Remarks**

Se la password è impostata a null o a stringa vuota, è possibile deproteggere il foglio di lavoro o la cartella di lavoro senza usare una password. Altrimenti, è necessario specificare la password per deproteggere il foglio di lavoro o la cartella di lavoro.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### toString() {#toString--}
```
public String toString()
```




**Returns:**
java.lang.String
### verifyPassword(String password) {#verifyPassword-java.lang.String-}
```
public boolean verifyPassword(String password)
```


Verifica la password.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| password | java.lang.String | La password. |

**Returns:**
boolean -
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

