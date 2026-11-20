---
title: "CopyOptions"
second_title: "Riferimento API di Aspose.Cells per Java"
description: "Rappresenta le opzioni di copia."
type: docs
url: /it/java/com.aspose.cells/copyoptions/
---

**Inheritance:**
java.lang.Object
```
public class CopyOptions
```

Rappresenta le opzioni di copia.
## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [CopyOptions()](#CopyOptions--) | CopyOptions costruttore. |
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getColumnCharacterWidth()](#getColumnCharacterWidth--) | Indica se copiare la larghezza della colonna in unità di caratteri. |
| [getCopyInvalidFormulasAsValues()](#getCopyInvalidFormulasAsValues--) | Se la formula non è valida per la destinazione dest destination, copia solo i valori. |
| [getCopyNames()](#getCopyNames--) | Indica se copiare i nomi. |
| [getExtendToAdjacentRange()](#getExtendToAdjacentRange--) | Indica se estendere gli intervalli quando si copia l'intervallo in un intervallo adiacente. |
| [getKeepMacros()](#getKeepMacros--) | Indica se mantenere le macro; |
| [getReferToDestinationSheet()](#getReferToDestinationSheet--) | Quando si copia l'intervallo nello stesso file e il grafico fa riferimento al foglio di origine, False indica che l'origine dati del grafico copiato non verrà modificata. |
| [getReferToSheetWithSameName()](#getReferToSheetWithSameName--) | In MS Excel, quando si copiano formule che fanno riferimento ad altri fogli di lavoro durante la copia di un foglio di lavoro in un altro, le formule copiate dovrebbero fare riferimento alla cartella di lavoro di origine. |
| [getUpdateInvalidReferencesToTargetSheet()](#getUpdateInvalidReferencesToTargetSheet--) | Indica se fare riferimento al foglio di lavoro di destinazione se il foglio di lavoro di riferimento non è stato copiato. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setColumnCharacterWidth(boolean value)](#setColumnCharacterWidth-boolean-) | Indica se copiare la larghezza della colonna in unità di caratteri. |
| [setCopyInvalidFormulasAsValues(boolean value)](#setCopyInvalidFormulasAsValues-boolean-) | Se la formula non è valida per la destinazione dest destination, copia solo i valori. |
| [setCopyNames(boolean value)](#setCopyNames-boolean-) | Indica se copiare i nomi. |
| [setExtendToAdjacentRange(boolean value)](#setExtendToAdjacentRange-boolean-) | Indica se estendere gli intervalli quando si copia l'intervallo in un intervallo adiacente. |
| [setKeepMacros(boolean value)](#setKeepMacros-boolean-) | Indica se mantenere le macro; |
| [setReferToDestinationSheet(boolean value)](#setReferToDestinationSheet-boolean-) | Quando si copia l'intervallo nello stesso file e il grafico fa riferimento al foglio di origine, False indica che l'origine dati del grafico copiato non verrà modificata. |
| [setReferToSheetWithSameName(boolean value)](#setReferToSheetWithSameName-boolean-) | In MS Excel, quando si copiano formule che fanno riferimento ad altri fogli di lavoro durante la copia di un foglio di lavoro in un altro, le formule copiate dovrebbero fare riferimento alla cartella di lavoro di origine. |
| [setUpdateInvalidReferencesToTargetSheet(boolean value)](#setUpdateInvalidReferencesToTargetSheet-boolean-) | Indica se fare riferimento al foglio di lavoro di destinazione se il foglio di lavoro di riferimento non è stato copiato. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### CopyOptions() {#CopyOptions--}
```
public CopyOptions()
```


CopyOptions costruttore.

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
### getColumnCharacterWidth() {#getColumnCharacterWidth--}
```
public boolean getColumnCharacterWidth()
```


Indica se copiare la larghezza della colonna in unità di caratteri.

**Returns:**
boolean
### getCopyInvalidFormulasAsValues() {#getCopyInvalidFormulasAsValues--}
```
public boolean getCopyInvalidFormulasAsValues()
```


Se la formula non è valida per la destinazione dest destination, copia solo i valori.

**Returns:**
boolean
### getCopyNames() {#getCopyNames--}
```
public boolean getCopyNames()
```


Indica se copiare i nomi.

**Returns:**
boolean
### getExtendToAdjacentRange() {#getExtendToAdjacentRange--}
```
public boolean getExtendToAdjacentRange()
```


Indica se estendere gli intervalli quando si copia l'intervallo in un intervallo adiacente.

**Remarks**

Se è true, estende solo l'intervallo del collegamento ipertestuale, non aggiungendo un nuovo collegamento ipertestuale quando si copiano i collegamenti ipertestuali su righe adiacenti.

**Returns:**
boolean
### getKeepMacros() {#getKeepMacros--}
```
public boolean getKeepMacros()
```


Indica se mantenere le macro;

**Remarks**

Solo per la copia della cartella di lavoro.

**Returns:**
boolean
### getReferToDestinationSheet() {#getReferToDestinationSheet--}
```
public boolean getReferToDestinationSheet()
```


Quando si copia l'intervallo nello stesso file e il grafico fa riferimento al foglio di origine, False indica che l'origine dati del grafico copiato non verrà modificata. True indica che l'origine dati del grafico copiato fa riferimento al foglio di destinazione.

**Remarks**

Il valore predefinito è false, funziona come MS Excel. Per esempio: se si copia un grafico con l'origine dati "sheet1!A1:B10" dal foglio di lavoro "sheet1" a un altro foglio di lavoro "sheet2", l'origine dati verrà modificata in "sheet2!A1:B10"

**Returns:**
boolean
### getReferToSheetWithSameName() {#getReferToSheetWithSameName--}
```
public boolean getReferToSheetWithSameName()
```


In MS Excel, quando si copiano formule che fanno riferimento ad altri fogli di lavoro durante la copia di un foglio di lavoro in un altro, le formule copiate dovrebbero fare riferimento alla cartella di lavoro di origine. Tuttavia, in alcune situazioni l'utente potrebbe aver bisogno che le formule copiate facciano riferimento a fogli di lavoro con lo stesso nome nella stessa cartella di lavoro, ad esempio quando quei fogli sono stati copiati prima di questa operazione di copia, allora questa proprietà dovrebbe essere impostata su true.

**Remarks**

Il valore predefinito è true.

**Returns:**
boolean
### getUpdateInvalidReferencesToTargetSheet() {#getUpdateInvalidReferencesToTargetSheet--}
```
public boolean getUpdateInvalidReferencesToTargetSheet()
```


Indica se fare riferimento al foglio di lavoro di destinazione se il foglio di lavoro di riferimento non è stato copiato.

**Remarks**

Funziona solo quando si copia un intervallo o un foglio di lavoro da un altro libro.

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




### setColumnCharacterWidth(boolean value) {#setColumnCharacterWidth-boolean-}
```
public void setColumnCharacterWidth(boolean value)
```


Indica se copiare la larghezza della colonna in unità di caratteri.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setCopyInvalidFormulasAsValues(boolean value) {#setCopyInvalidFormulasAsValues-boolean-}
```
public void setCopyInvalidFormulasAsValues(boolean value)
```


Se la formula non è valida per la destinazione dest destination, copia solo i valori.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setCopyNames(boolean value) {#setCopyNames-boolean-}
```
public void setCopyNames(boolean value)
```


Indica se copiare i nomi.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setExtendToAdjacentRange(boolean value) {#setExtendToAdjacentRange-boolean-}
```
public void setExtendToAdjacentRange(boolean value)
```


Indica se estendere gli intervalli quando si copia l'intervallo in un intervallo adiacente.

**Remarks**

Se è true, estende solo l'intervallo del collegamento ipertestuale, non aggiungendo un nuovo collegamento ipertestuale quando si copiano i collegamenti ipertestuali su righe adiacenti.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setKeepMacros(boolean value) {#setKeepMacros-boolean-}
```
public void setKeepMacros(boolean value)
```


Indica se mantenere le macro;

**Remarks**

Solo per la copia della cartella di lavoro.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setReferToDestinationSheet(boolean value) {#setReferToDestinationSheet-boolean-}
```
public void setReferToDestinationSheet(boolean value)
```


Quando si copia l'intervallo nello stesso file e il grafico fa riferimento al foglio di origine, False indica che l'origine dati del grafico copiato non verrà modificata. True indica che l'origine dati del grafico copiato fa riferimento al foglio di destinazione.

**Remarks**

Il valore predefinito è false, funziona come MS Excel. Per esempio: se si copia un grafico con l'origine dati "sheet1!A1:B10" dal foglio di lavoro "sheet1" a un altro foglio di lavoro "sheet2", l'origine dati verrà modificata in "sheet2!A1:B10"

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setReferToSheetWithSameName(boolean value) {#setReferToSheetWithSameName-boolean-}
```
public void setReferToSheetWithSameName(boolean value)
```


In MS Excel, quando si copiano formule che fanno riferimento ad altri fogli di lavoro durante la copia di un foglio di lavoro in un altro, le formule copiate dovrebbero fare riferimento alla cartella di lavoro di origine. Tuttavia, in alcune situazioni l'utente potrebbe aver bisogno che le formule copiate facciano riferimento a fogli di lavoro con lo stesso nome nella stessa cartella di lavoro, ad esempio quando quei fogli sono stati copiati prima di questa operazione di copia, allora questa proprietà dovrebbe essere impostata su true.

**Remarks**

Il valore predefinito è true.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setUpdateInvalidReferencesToTargetSheet(boolean value) {#setUpdateInvalidReferencesToTargetSheet-boolean-}
```
public void setUpdateInvalidReferencesToTargetSheet(boolean value)
```


Indica se fare riferimento al foglio di lavoro di destinazione se il foglio di lavoro di riferimento non è stato copiato.

**Remarks**

Funziona solo quando si copia un intervallo o un foglio di lavoro da un altro libro.

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

