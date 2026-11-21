---
title: "ErrorCheckType"
second_title: "Aspose.Cells för Java API-referens"
description: "Representerar alla felkontrolltyper."
type: docs
url: /sv/java/com.aspose.cells/errorchecktype/
---

**Inheritance:**
java.lang.Object
```
public final class ErrorCheckType
```

Representerar alla felkontrolltyper.
## Fält

| Fält | Beskrivning |
| --- | --- |
| [CALC](#CALC) | **Anmärkningar** |
| [CALCULATED_COLUMN](#CALCULATED-COLUMN) | Ignorera fel när celler innehåller ett värde som skiljer sig från en beräknad kolumnformel. |
| [EMPTY_CELL_REF](#EMPTY-CELL-REF) | Ignorera fel när formler hänvisar till tomma celler. |
| [EVALUATION_ERROR](#EVALUATION-ERROR) | Ignorera fel när celler innehåller formler som resulterar i ett fel. |
| [INCONSIST_FORMULA](#INCONSIST-FORMULA) | Ignorera fel när en formel i ett område i ditt kalkylblad skiljer sig från andra formler i samma område. |
| [INCONSIST_RANGE](#INCONSIST-RANGE) | Ignorera fel när formler utelämnar vissa celler i ett område. |
| [NUMBER_STORED_AS_TEXT](#NUMBER-STORED-AS-TEXT) | Ignorera fel när tal är formaterade som text eller föregås av ett apostrof |
| [TABLE_DATA_VALIDATION](#TABLE-DATA-VALIDATION) | Ignorera fel när ett cells värde i en tabell inte följer de specificerade datavalideringsreglerna. |
| [TEXT_DATE](#TEXT-DATE) | Ignorera fel när formler innehåller textformaterade celler med år representerade med två siffror. |
| [TEXT_NUMBER](#TEXT-NUMBER) | Ignorera fel när tal är formaterade som text eller föregås av ett apostrof |
| [TWO_DIGIT_TEXT_YEAR](#TWO-DIGIT-TEXT-YEAR) | Ignorera fel när formler innehåller textformaterade celler med år representerade med två siffror. |
| [UNLOCKED_FORMULA](#UNLOCKED-FORMULA) | Ignorera fel när olåsta celler innehåller formler. |
| [UNPROCTED_FORMULA](#UNPROCTED-FORMULA) | Ignorera fel när olåsta celler innehåller formler. |
| [VALIDATION](#VALIDATION) | Ignorera fel när ett cells värde i en tabell inte följer de specificerade datavalideringsreglerna. |
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### CALC {#CALC}
```
public static final int CALC
```


**Remarks**

OBS: Denna medlem är nu föråldrad. Använd istället enumen ErrorCheckType.EvaluationError. Denna metod kommer att tas bort 12 månader senare från och med oktober 2023. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

### CALCULATED_COLUMN {#CALCULATED-COLUMN}
```
public static final int CALCULATED_COLUMN
```


Ignorera fel när celler innehåller ett värde som skiljer sig från en beräknad kolumnformel.

### EMPTY_CELL_REF {#EMPTY-CELL-REF}
```
public static final int EMPTY_CELL_REF
```


Ignorera fel när formler hänvisar till tomma celler.

### EVALUATION_ERROR {#EVALUATION-ERROR}
```
public static final int EVALUATION_ERROR
```


Ignorera fel när celler innehåller formler som resulterar i ett fel.

### INCONSIST_FORMULA {#INCONSIST-FORMULA}
```
public static final int INCONSIST_FORMULA
```


Ignorera fel när en formel i ett område i ditt kalkylblad skiljer sig från andra formler i samma område.

### INCONSIST_RANGE {#INCONSIST-RANGE}
```
public static final int INCONSIST_RANGE
```


Ignorera fel när formler utelämnar vissa celler i ett område.

### NUMBER_STORED_AS_TEXT {#NUMBER-STORED-AS-TEXT}
```
public static final int NUMBER_STORED_AS_TEXT
```


Ignorera fel när tal är formaterade som text eller föregås av ett apostrof

### TABLE_DATA_VALIDATION {#TABLE-DATA-VALIDATION}
```
public static final int TABLE_DATA_VALIDATION
```


Ignorera fel när ett cells värde i en tabell inte följer de specificerade datavalideringsreglerna.

### TEXT_DATE {#TEXT-DATE}
```
public static final int TEXT_DATE
```


Ignorera fel när formler innehåller textformaterade celler med år representerade med två siffror.

**Remarks**

OBS: Denna medlem är nu föråldrad. Använd istället enumen ErrorCheckType.TwoDigitTextYear. Denna metod kommer att tas bort 12 månader senare från och med oktober 2023. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

### TEXT_NUMBER {#TEXT-NUMBER}
```
public static final int TEXT_NUMBER
```


Ignorera fel när tal är formaterade som text eller föregås av ett apostrof

**Remarks**

OBS: Denna medlem är nu föråldrad. Använd istället enumen ErrorCheckType.NumberStoredAsText. Denna metod kommer att tas bort 12 månader senare från och med oktober 2023. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

### TWO_DIGIT_TEXT_YEAR {#TWO-DIGIT-TEXT-YEAR}
```
public static final int TWO_DIGIT_TEXT_YEAR
```


Ignorera fel när formler innehåller textformaterade celler med år representerade med två siffror.

### UNLOCKED_FORMULA {#UNLOCKED-FORMULA}
```
public static final int UNLOCKED_FORMULA
```


Ignorera fel när olåsta celler innehåller formler.

### UNPROCTED_FORMULA {#UNPROCTED-FORMULA}
```
public static final int UNPROCTED_FORMULA
```


Ignorera fel när olåsta celler innehåller formler.

**Remarks**

OBS: Denna medlem är nu föråldrad. Använd istället enumen ErrorCheckType.UnproctedFormula. Denna metod kommer att tas bort 12 månader senare från och med oktober 2023. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

### VALIDATION {#VALIDATION}
```
public static final int VALIDATION
```


Ignorera fel när ett cells värde i en tabell inte följer de specificerade datavalideringsreglerna.

**Remarks**

OBS: Denna medlem är nu föråldrad. Använd istället enumen ErrorCheckType.TableDataValidation. Denna metod kommer att tas bort 12 månader senare från och med oktober 2023. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| Parameter | Typ | Beskrivning |
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
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

