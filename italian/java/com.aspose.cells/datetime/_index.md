---
title: "DateTime"
second_title: "Riferimento API di Aspose.Cells per Java"
description: "Rappresenta un istante nel tempo tipicamente espresso come data e ora del giorno."
type: docs
url: /it/java/com.aspose.cells/datetime/
---

**Inheritance:**
java.lang.Object
```
public class DateTime
```

Rappresenta un istante nel tempo, tipicamente espresso come data e ora del giorno.
## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [DateTime(int year, int month, int day)](#DateTime-int-int-int-) | Inizializza una nuova istanza dell'oggetto DateTime con l'anno, il mese e il giorno specificati. |
| [DateTime(int year, int month, int day, int hour, int minute, int second)](#DateTime-int-int-int-int-int-int-) | Inizializza una nuova istanza dell'oggetto DateTime con l'anno, il mese, il giorno, l'ora, il minuto e il secondo specificati. |
| [DateTime(int year, int month, int day, int hour, int minute, int second, int millisecond)](#DateTime-int-int-int-int-int-int-int-) | Inizializza una nuova istanza dell'oggetto DateTime con l'anno, il mese, il giorno, l'ora, il minuto, il secondo e il millisecondo specificati. |
| [DateTime(Date date)](#DateTime-java.util.Date-) | Inizializza una nuova istanza dell'oggetto DateTime con l'oggetto Date specificato. |
| [DateTime(Calendar cld)](#DateTime-java.util.Calendar-) | Inizializza una nuova istanza dell'oggetto DateTime con l'oggetto Calendar specificato. |
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [addDays(double value)](#addDays-double-) | Aggiunge il numero specificato di giorni al valore di questa istanza. |
| [addHours(double value)](#addHours-double-) | Aggiunge il numero specificato di ore al valore di questa istanza. |
| [addMilliseconds(double value)](#addMilliseconds-double-) | Aggiunge il numero specificato di millisecondi al valore di questa istanza. |
| [addMinutes(double value)](#addMinutes-double-) | Aggiunge il numero specificato di minuti al valore di questa istanza. |
| [addMonths(int months)](#addMonths-int-) | Aggiunge il numero specificato di mesi al valore di questa istanza. |
| [addSeconds(double value)](#addSeconds-double-) | Aggiunge il numero specificato di secondi al valore di questa istanza. |
| [addYears(int value)](#addYears-int-) | Aggiunge il numero specificato di anni al valore di questa istanza. |
| [compareTo(DateTime value)](#compareTo-com.aspose.cells.DateTime-) | Confronta il valore di questa istanza con un valore DateTime specificato e restituisce un intero che indica se questa istanza è precedente, uguale o successiva al valore DateTime specificato. |
| [compareTo(Object value)](#compareTo-java.lang.Object-) | Confronta il valore di questa istanza con un oggetto specificato che contiene un valore DateTime specificato e restituisce un intero che indica se questa istanza è precedente, uguale o successiva al valore DateTime specificato. |
| [equals(Object value)](#equals-java.lang.Object-) | Restituisce un valore che indica se questa istanza è uguale a un oggetto specificato. |
| [getClass()](#getClass--) |  |
| [getDay()](#getDay--) | Restituisce il giorno del mese rappresentato da questa istanza. |
| [getDayOfWeek()](#getDayOfWeek--) | Restituisce il giorno della settimana rappresentato da questa istanza. |
| [getDayOfYear()](#getDayOfYear--) | Restituisce il giorno dell'anno rappresentato da questa istanza. |
| [getHour()](#getHour--) | Restituisce la componente ora della data rappresentata da questa istanza. |
| [getMillisecond()](#getMillisecond--) | Restituisce la componente millisecondi della data rappresentata da questa istanza. |
| [getMinute()](#getMinute--) | Restituisce la componente minuti della data rappresentata da questa istanza. |
| [getMonth()](#getMonth--) | Restituisce la componente mese della data rappresentata da questa istanza. |
| [getNow()](#getNow--) | Restituisce un oggetto DateTime impostato alla data e ora correnti di questo computer, espresso come ora locale. |
| [getSecond()](#getSecond--) | Restituisce la componente secondi della data rappresentata da questa istanza. |
| [getYear()](#getYear--) | Restituisce la componente anno della data rappresentata da questa istanza. |
| [hashCode()](#hashCode--) | Restituisce il codice hash per questa istanza. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [toCalendar()](#toCalendar--) | Converte il valore dell'oggetto DateTime corrente in un oggetto Calendar. |
| [toDate()](#toDate--) | Converte il valore dell'oggetto DateTime corrente in un oggetto Date. |
| [toLocalTime()](#toLocalTime--) | Converte il valore dell'oggetto DateTime corrente all'ora locale. |
| [toString()](#toString--) | Converte il valore dell'oggetto DateTime corrente nella sua rappresentazione stringa equivalente. |
| [toUniversalTime()](#toUniversalTime--) | Converte il valore dell'oggetto DateTime corrente al Tempo Universale Coordinato (UTC). |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### DateTime(int year, int month, int day) {#DateTime-int-int-int-}
```
public DateTime(int year, int month, int day)
```


Inizializza una nuova istanza dell'oggetto DateTime con l'anno, il mese e il giorno specificati.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| anno | int | L'anno (da 1 a 9999). |
| mese | int | Il mese (da 1 a 12). |
| giorno | int | Il giorno (da 1 al numero di giorni nel mese). |

### DateTime(int year, int month, int day, int hour, int minute, int second) {#DateTime-int-int-int-int-int-int-}
```
public DateTime(int year, int month, int day, int hour, int minute, int second)
```


Inizializza una nuova istanza dell'oggetto DateTime con l'anno, il mese, il giorno, l'ora, il minuto e il secondo specificati.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| anno | int | L'anno (da 1 a 9999). |
| mese | int | Il mese (da 1 a 12). |
| giorno | int | Il giorno (da 1 al numero di giorni nel mese). |
| ora | int | Le ore (da 0 a 23). |
| minuto | int | I minuti (da 0 a 59). |
| secondo | int | I secondi (da 0 a 59). |

### DateTime(int year, int month, int day, int hour, int minute, int second, int millisecond) {#DateTime-int-int-int-int-int-int-int-}
```
public DateTime(int year, int month, int day, int hour, int minute, int second, int millisecond)
```


Inizializza una nuova istanza dell'oggetto DateTime con l'anno, il mese, il giorno, l'ora, il minuto, il secondo e il millisecondo specificati.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| anno | int | L'anno (da 1 a 9999). |
| mese | int | Il mese (da 1 a 12). |
| giorno | int | Il giorno (da 1 al numero di giorni nel mese). |
| ora | int | Le ore (da 0 a 23). |
| minuto | int | I minuti (da 0 a 59). |
| secondo | int | I secondi (da 0 a 59). |
| millisecondo | int | I millisecondi (da 0 a 999). |

### DateTime(Date date) {#DateTime-java.util.Date-}
```
public DateTime(Date date)
```


Inizializza una nuova istanza dell'oggetto DateTime con l'oggetto Date specificato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| data | java.util.Date | L'oggetto Date |

### DateTime(Calendar cld) {#DateTime-java.util.Calendar-}
```
public DateTime(Calendar cld)
```


Inizializza una nuova istanza dell'oggetto DateTime con l'oggetto Calendar specificato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| cld | java.util.Calendar | L'oggetto Calendar |

### addDays(double value) {#addDays-double-}
```
public DateTime addDays(double value)
```


Aggiunge il numero specificato di giorni al valore di questa istanza.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | double | Un numero di giorni interi e frazionari. Il parametro value può essere negativo o positivo. |

**Returns:**
[DateTime](../../com.aspose.cells/datetime) - A DateTime object whose value is the sum of the date and time represented by this instance and the number of days represented by value.
### addHours(double value) {#addHours-double-}
```
public DateTime addHours(double value)
```


Aggiunge il numero specificato di ore al valore di questa istanza.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | double | Un numero di ore intere e frazionarie. Il parametro value può essere negativo o positivo. |

**Returns:**
[DateTime](../../com.aspose.cells/datetime) - A DateTime object whose value is the sum of the date and time represented by this instance and the number of hours represented by value.
### addMilliseconds(double value) {#addMilliseconds-double-}
```
public DateTime addMilliseconds(double value)
```


Aggiunge il numero specificato di millisecondi al valore di questa istanza.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | double | Un numero di millisecondi interi e frazionari. Il parametro value può essere negativo o positivo. Nota che questo valore è arrotondato all'intero più vicino. |

**Returns:**
[DateTime](../../com.aspose.cells/datetime) - A DateTime object whose value is the sum of the date and time represented by this instance and the number of milliseconds represented by value.
### addMinutes(double value) {#addMinutes-double-}
```
public DateTime addMinutes(double value)
```


Aggiunge il numero specificato di minuti al valore di questa istanza.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | double | Un numero di minuti interi e frazionari. Il parametro value può essere negativo o positivo. |

**Returns:**
[DateTime](../../com.aspose.cells/datetime) - A DateTime object whose value is the sum of the date and time represented by this instance and the number of minutes represented by value.
### addMonths(int months) {#addMonths-int-}
```
public DateTime addMonths(int months)
```


Aggiunge il numero specificato di mesi al valore di questa istanza.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| mesi | int | Un numero di mesi. Il parametro months può essere negativo o positivo. |

**Returns:**
[DateTime](../../com.aspose.cells/datetime) - A DateTime object whose value is the sum of the date and time represented by this instance and months.
### addSeconds(double value) {#addSeconds-double-}
```
public DateTime addSeconds(double value)
```


Aggiunge il numero specificato di secondi al valore di questa istanza.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | double | Un numero di secondi interi e frazionari. Il parametro value può essere negativo o positivo. |

**Returns:**
[DateTime](../../com.aspose.cells/datetime) - A DateTime object whose value is the sum of the date and time represented by this instance and the number of seconds represented by value.
### addYears(int value) {#addYears-int-}
```
public DateTime addYears(int value)
```


Aggiunge il numero specificato di anni al valore di questa istanza.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int | Un numero di anni. Il parametro value può essere negativo o positivo. |

**Returns:**
[DateTime](../../com.aspose.cells/datetime) - A DateTime object whose value is the sum of the date and time represented by this instance and the number of years represented by value.
### compareTo(DateTime value) {#compareTo-com.aspose.cells.DateTime-}
```
public int compareTo(DateTime value)
```


Confronta il valore di questa istanza con un valore DateTime specificato e restituisce un intero che indica se questa istanza è precedente, uguale o successiva al valore DateTime specificato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| value | [DateTime](../../com.aspose.cells/datetime) | Un oggetto DateTime da confrontare. |

**Returns:**
int - Un numero con segno che indica i valori relativi di questa istanza e del parametro value. Valore Descrizione Meno di zero Questa istanza è precedente a value. Zero Questa istanza è uguale a value. Maggiore di zero Questa istanza è successiva a value.
### compareTo(Object value) {#compareTo-java.lang.Object-}
```
public int compareTo(Object value)
```


Confronta il valore di questa istanza con un oggetto specificato che contiene un valore DateTime specificato e restituisce un intero che indica se questa istanza è precedente, uguale o successiva al valore DateTime specificato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.Object | Un oggetto DateTime boxed da confrontare, oppure null. |

**Returns:**
int - Un numero con segno che indica i valori relativi di questa istanza e di value. Valore Descrizione Meno di zero Questa istanza è precedente a value. Zero Questa istanza è uguale a value. Maggiore di zero Questa istanza è successiva a value, oppure value è null.
### equals(Object value) {#equals-java.lang.Object-}
```
public boolean equals(Object value)
```


Restituisce un valore che indica se questa istanza è uguale a un oggetto specificato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.Object | Un oggetto da confrontare con questa istanza. |

**Returns:**
boolean - true se value è un'istanza di DateTime e uguale al valore di questa istanza; altrimenti, false.
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getDay() {#getDay--}
```
public int getDay()
```


Restituisce il giorno del mese rappresentato da questa istanza.

**Returns:**
int - Il componente giorno, espresso come valore compreso tra 1 e 31.
### getDayOfWeek() {#getDayOfWeek--}
```
public int getDayOfWeek()
```


Restituisce il giorno della settimana rappresentato da questa istanza.

**Returns:**
int - il giorno della settimana di questo valore DateTime.
### getDayOfYear() {#getDayOfYear--}
```
public int getDayOfYear()
```


Restituisce il giorno dell'anno rappresentato da questa istanza.

**Returns:**
int - Il giorno dell'anno, espresso come valore compreso tra 1 e 366.
### getHour() {#getHour--}
```
public int getHour()
```


Restituisce la componente ora della data rappresentata da questa istanza.

**Returns:**
int - Il componente ora, espresso come valore compreso tra 0 e 23.
### getMillisecond() {#getMillisecond--}
```
public int getMillisecond()
```


Restituisce la componente millisecondi della data rappresentata da questa istanza.

**Returns:**
int - Il componente millisecondi, espresso come valore compreso tra 0 e 999.
### getMinute() {#getMinute--}
```
public int getMinute()
```


Restituisce la componente minuti della data rappresentata da questa istanza.

**Returns:**
int - Il componente minuti, espresso come valore compreso tra 0 e 59.
### getMonth() {#getMonth--}
```
public int getMonth()
```


Restituisce la componente mese della data rappresentata da questa istanza.

**Returns:**
int - Il componente mese, espresso come valore compreso tra 1 e 12.
### getNow() {#getNow--}
```
public static DateTime getNow()
```


Restituisce un oggetto DateTime impostato alla data e ora correnti di questo computer, espresso come ora locale.

**Returns:**
[DateTime](../../com.aspose.cells/datetime) - A DateTime object whose value is the current local date and time.
### getSecond() {#getSecond--}
```
public int getSecond()
```


Restituisce la componente secondi della data rappresentata da questa istanza.

**Returns:**
int - I secondi, compresi tra 0 e 59.
### getYear() {#getYear--}
```
public int getYear()
```


Restituisce la componente anno della data rappresentata da questa istanza.

**Returns:**
int - L'anno, compreso tra 1 e 9999.
### hashCode() {#hashCode--}
```
public int hashCode()
```


Restituisce il codice hash per questa istanza.

**Returns:**
int - Un codice hash intero a 32 bit con segno.
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### toCalendar() {#toCalendar--}
```
public Calendar toCalendar()
```


Converte il valore dell'oggetto DateTime corrente in un oggetto Calendar.

**Returns:**
java.util.Calendar - Oggetto Calendar
### toDate() {#toDate--}
```
public Date toDate()
```


Converte il valore dell'oggetto DateTime corrente in un oggetto Date.

**Returns:**
java.util.Date - Oggetto Date
### toLocalTime() {#toLocalTime--}
```
public DateTime toLocalTime()
```


Converte il valore dell'oggetto DateTime corrente all'ora locale.

**Returns:**
[DateTime](../../com.aspose.cells/datetime) - A DateTime object of local
### toString() {#toString--}
```
public String toString()
```


Converte il valore dell'oggetto DateTime corrente nella sua rappresentazione stringa equivalente.

**Returns:**
java.lang.String - Una rappresentazione stringa del valore dell'oggetto DateTime corrente.
### toUniversalTime() {#toUniversalTime--}
```
public DateTime toUniversalTime()
```


Converte il valore dell'oggetto DateTime corrente al Tempo Universale Coordinato (UTC).

**Returns:**
[DateTime](../../com.aspose.cells/datetime) - A DateTime object of UTC
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

