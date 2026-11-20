---
title: "DateTime"
second_title: "Aspose.Cells for Java API-Referenz"
description: "Stellt einen Zeitpunkt dar, der typischerweise als Datum und Uhrzeit ausgedrückt wird."
type: docs
url: /de/java/com.aspose.gridweb/datetime/
---

**Inheritance:**
java.lang.Object
```
public class DateTime
```

Stellt einen Zeitpunkt dar, typischerweise ausgedrückt als Datum und Uhrzeit.
## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [DateTime(int year, int month, int day)](#DateTime-int-int-int-) | Initialisiert eine neue Instanz des DateTime-Objekts mit dem angegebenen Jahr, Monat und Tag. |
| [DateTime(int year, int month, int day, int hour, int minute, int second)](#DateTime-int-int-int-int-int-int-) | Initialisiert eine neue Instanz des DateTime-Objekts mit dem angegebenen Jahr, Monat, Tag, Stunde, Minute und Sekunde. |
| [DateTime(int year, int month, int day, int hour, int minute, int second, int millisecond)](#DateTime-int-int-int-int-int-int-int-) | Initialisiert eine neue Instanz des DateTime-Objekts mit dem angegebenen Jahr, Monat, Tag, Stunde, Minute, Sekunde und Millisekunde. |
| [DateTime(Date date)](#DateTime-java.util.Date-) | Initialisiert eine neue Instanz des DateTime-Objekts mit dem angegebenen Date-Objekt. |
| [DateTime(Calendar cld)](#DateTime-java.util.Calendar-) | Initialisiert eine neue Instanz des DateTime-Objekts mit dem angegebenen Calendar-Objekt. |
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [addDays(double value)](#addDays-double-) | Addiert die angegebene Anzahl von Tagen zum Wert dieser Instanz. |
| [addHours(double value)](#addHours-double-) | Addiert die angegebene Anzahl von Stunden zum Wert dieser Instanz. |
| [addMilliseconds(double value)](#addMilliseconds-double-) | Addiert die angegebene Anzahl von Millisekunden zum Wert dieser Instanz. |
| [addMinutes(double value)](#addMinutes-double-) | Addiert die angegebene Anzahl von Minuten zum Wert dieser Instanz. |
| [addMonths(int months)](#addMonths-int-) | Addiert die angegebene Anzahl von Monaten zum Wert dieser Instanz. |
| [addSeconds(double value)](#addSeconds-double-) | Addiert die angegebene Anzahl von Sekunden zum Wert dieser Instanz. |
| [addYears(int value)](#addYears-int-) | Addiert die angegebene Anzahl von Jahren zum Wert dieser Instanz. |
| [compareTo(DateTime value)](#compareTo-com.aspose.gridweb.DateTime-) | Vergleicht den Wert dieser Instanz mit einem angegebenen DateTime-Wert und gibt einen Integer zurück, der angibt, ob diese Instanz früher, gleich oder später als der angegebene DateTime-Wert ist. |
| [compareTo(Object value)](#compareTo-java.lang.Object-) | Vergleicht den Wert dieser Instanz mit einem angegebenen Objekt, das einen angegebenen DateTime-Wert enthält, und gibt einen Integer zurück, der angibt, ob diese Instanz früher, gleich oder später als der angegebene DateTime-Wert ist. |
| [equals(Object value)](#equals-java.lang.Object-) | Gibt einen Wert zurück, der angibt, ob diese Instanz einem angegebenen Objekt gleich ist. |
| [getClass()](#getClass--) |  |
| [getDay()](#getDay--) | Ermittelt den Tag des Monats, der von dieser Instanz dargestellt wird. |
| [getDayOfWeek()](#getDayOfWeek--) | Ermittelt den Wochentag, der von dieser Instanz dargestellt wird. |
| [getDayOfYear()](#getDayOfYear--) | Ermittelt den Tag des Jahres, der von dieser Instanz dargestellt wird. |
| [getHour()](#getHour--) | Ermittelt die Stundenkomponente des Datums, das von dieser Instanz dargestellt wird. |
| [getMillisecond()](#getMillisecond--) | Ermittelt die Millisekundenkomponente des Datums, das von dieser Instanz dargestellt wird. |
| [getMinute()](#getMinute--) | Ermittelt die Minutenkomponente des Datums, das von dieser Instanz dargestellt wird. |
| [getMonth()](#getMonth--) | Liefert die Monatskomponente des von dieser Instanz dargestellten Datums. |
| [getNow()](#getNow--) | Liefert ein DateTime-Objekt, das auf das aktuelle Datum und die aktuelle Uhrzeit dieses Computers eingestellt ist und als lokale Zeit ausgedrückt wird. |
| [getSecond()](#getSecond--) | Liefert die Sekundenkomponente des von dieser Instanz dargestellten Datums. |
| [getYear()](#getYear--) | Liefert die Jahreskomponente des von dieser Instanz dargestellten Datums. |
| [hashCode()](#hashCode--) | Gibt den Hashcode für diese Instanz zurück. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [toCalendar()](#toCalendar--) | Konvertiert den Wert des aktuellen DateTime-Objekts in ein Calendar-Objekt. |
| [toDate()](#toDate--) | Konvertiert den Wert des aktuellen DateTime-Objekts in ein Date-Objekt. |
| [toLocalTime()](#toLocalTime--) | Konvertiert den Wert des aktuellen DateTime-Objekts in die lokale Zeit. |
| [toString()](#toString--) | Konvertiert den Wert des aktuellen DateTime-Objekts in seine äquivalente Zeichenkettenrepräsentation. |
| [toUniversalTime()](#toUniversalTime--) | Konvertiert den Wert des aktuellen DateTime-Objekts in die koordinierte Weltzeit (UTC). |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### DateTime(int year, int month, int day) {#DateTime-int-int-int-}
```
public DateTime(int year, int month, int day)
```


Initialisiert eine neue Instanz des DateTime-Objekts mit dem angegebenen Jahr, Monat und Tag.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Jahr | int | Das Jahr (1 bis 9999). |
| Monat | int | Der Monat (1 bis 12). |
| Tag | int | Der Tag (1 bis zur Anzahl der Tage im Monat). |

### DateTime(int year, int month, int day, int hour, int minute, int second) {#DateTime-int-int-int-int-int-int-}
```
public DateTime(int year, int month, int day, int hour, int minute, int second)
```


Initialisiert eine neue Instanz des DateTime-Objekts mit dem angegebenen Jahr, Monat, Tag, Stunde, Minute und Sekunde.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Jahr | int | Das Jahr (1 bis 9999). |
| Monat | int | Der Monat (1 bis 12). |
| Tag | int | Der Tag (1 bis zur Anzahl der Tage im Monat). |
| Stunde | int | Die Stunden (0 bis 23). |
| Minute | int | Die Minuten (0 bis 59). |
| Sekunde | int | Die Sekunden (0 bis 59). |

### DateTime(int year, int month, int day, int hour, int minute, int second, int millisecond) {#DateTime-int-int-int-int-int-int-int-}
```
public DateTime(int year, int month, int day, int hour, int minute, int second, int millisecond)
```


Initialisiert eine neue Instanz des DateTime-Objekts mit dem angegebenen Jahr, Monat, Tag, Stunde, Minute, Sekunde und Millisekunde.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Jahr | int | Das Jahr (1 bis 9999). |
| Monat | int | Der Monat (1 bis 12). |
| Tag | int | Der Tag (1 bis zur Anzahl der Tage im Monat). |
| Stunde | int | Die Stunden (0 bis 23). |
| Minute | int | Die Minuten (0 bis 59). |
| Sekunde | int | Die Sekunden (0 bis 59). |
| Millisekunde | int | Die Millisekunden (0 bis 999). |

### DateTime(Date date) {#DateTime-java.util.Date-}
```
public DateTime(Date date)
```


Initialisiert eine neue Instanz des DateTime-Objekts mit dem angegebenen Date-Objekt.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Datum | java.util.Date | Das Date-Objekt |

### DateTime(Calendar cld) {#DateTime-java.util.Calendar-}
```
public DateTime(Calendar cld)
```


Initialisiert eine neue Instanz des DateTime-Objekts mit dem angegebenen Calendar-Objekt.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| cld | java.util.Calendar | Das Calendar-Objekt |

### addDays(double value) {#addDays-double-}
```
public DateTime addDays(double value)
```


Addiert die angegebene Anzahl von Tagen zum Wert dieser Instanz.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | double | Eine Anzahl von ganzen und gebrochenen Tagen. Der Wertparameter kann negativ oder positiv sein. |

**Returns:**
[DateTime](../../com.aspose.gridweb/datetime) - A DateTime object whose value is the sum of the date and time represented by this instance and the number of days represented by value.
### addHours(double value) {#addHours-double-}
```
public DateTime addHours(double value)
```


Addiert die angegebene Anzahl von Stunden zum Wert dieser Instanz.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | double | Eine Anzahl von ganzen und gebrochenen Stunden. Der Wertparameter kann negativ oder positiv sein. |

**Returns:**
[DateTime](../../com.aspose.gridweb/datetime) - A DateTime object whose value is the sum of the date and time represented by this instance and the number of hours represented by value.
### addMilliseconds(double value) {#addMilliseconds-double-}
```
public DateTime addMilliseconds(double value)
```


Addiert die angegebene Anzahl von Millisekunden zum Wert dieser Instanz.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | double | Eine Anzahl von ganzen und gebrochenen Millisekunden. Der Wertparameter kann negativ oder positiv sein. Hinweis: Dieser Wert wird auf die nächste ganze Zahl gerundet. |

**Returns:**
[DateTime](../../com.aspose.gridweb/datetime) - A DateTime object whose value is the sum of the date and time represented by this instance and the number of milliseconds represented by value.
### addMinutes(double value) {#addMinutes-double-}
```
public DateTime addMinutes(double value)
```


Addiert die angegebene Anzahl von Minuten zum Wert dieser Instanz.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | double | Eine Anzahl von ganzen und gebrochenen Minuten. Der Wertparameter kann negativ oder positiv sein. |

**Returns:**
[DateTime](../../com.aspose.gridweb/datetime) - A DateTime object whose value is the sum of the date and time represented by this instance and the number of minutes represented by value.
### addMonths(int months) {#addMonths-int-}
```
public DateTime addMonths(int months)
```


Addiert die angegebene Anzahl von Monaten zum Wert dieser Instanz.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Monate | int | Eine Anzahl von Monaten. Der Monate-Parameter kann negativ oder positiv sein. |

**Returns:**
[DateTime](../../com.aspose.gridweb/datetime) - A DateTime object whose value is the sum of the date and time represented by this instance and months.
### addSeconds(double value) {#addSeconds-double-}
```
public DateTime addSeconds(double value)
```


Addiert die angegebene Anzahl von Sekunden zum Wert dieser Instanz.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | double | Eine Anzahl von ganzen und gebrochenen Sekunden. Der Wertparameter kann negativ oder positiv sein. |

**Returns:**
[DateTime](../../com.aspose.gridweb/datetime) - A DateTime object whose value is the sum of the date and time represented by this instance and the number of seconds represented by value.
### addYears(int value) {#addYears-int-}
```
public DateTime addYears(int value)
```


Addiert die angegebene Anzahl von Jahren zum Wert dieser Instanz.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int | Eine Anzahl von Jahren. Der Wertparameter kann negativ oder positiv sein. |

**Returns:**
[DateTime](../../com.aspose.gridweb/datetime) - A DateTime object whose value is the sum of the date and time represented by this instance and the number of years represented by value.
### compareTo(DateTime value) {#compareTo-com.aspose.gridweb.DateTime-}
```
public int compareTo(DateTime value)
```


Vergleicht den Wert dieser Instanz mit einem angegebenen DateTime-Wert und gibt einen Integer zurück, der angibt, ob diese Instanz früher, gleich oder später als der angegebene DateTime-Wert ist.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | [DateTime](../../com.aspose.gridweb/datetime) | Ein DateTime-Objekt zum Vergleichen. |

**Returns:**
int - Eine vorzeichenbehaftete Zahl, die die relativen Werte dieser Instanz und des Wertparameters angibt. Wertbeschreibung Weniger als Null Diese Instanz liegt vor dem Wert. Null Diese Instanz ist gleich dem Wert. Größer als Null Diese Instanz liegt nach dem Wert.
### compareTo(Object value) {#compareTo-java.lang.Object-}
```
public int compareTo(Object value)
```


Vergleicht den Wert dieser Instanz mit einem angegebenen Objekt, das einen angegebenen DateTime-Wert enthält, und gibt einen Integer zurück, der angibt, ob diese Instanz früher, gleich oder später als der angegebene DateTime-Wert ist.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.Object | Ein verpacktes DateTime-Objekt zum Vergleichen oder null. |

**Returns:**
int - Eine vorzeichenbehaftete Zahl, die die relativen Werte dieser Instanz und des Wertes angibt. Wertbeschreibung Weniger als Null Diese Instanz liegt vor dem Wert. Null Diese Instanz ist gleich dem Wert. Größer als Null Diese Instanz liegt nach dem Wert oder der Wert ist null.
### equals(Object value) {#equals-java.lang.Object-}
```
public boolean equals(Object value)
```


Gibt einen Wert zurück, der angibt, ob diese Instanz einem angegebenen Objekt gleich ist.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.Object | Ein Objekt zum Vergleich mit dieser Instanz. |

**Returns:**
boolean - true, wenn value eine Instanz von DateTime ist und dem Wert dieser Instanz entspricht; andernfalls false.
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


Ermittelt den Tag des Monats, der von dieser Instanz dargestellt wird.

**Returns:**
int - Die Tageskomponente, ausgedrückt als ein Wert zwischen 1 und 31.
### getDayOfWeek() {#getDayOfWeek--}
```
public int getDayOfWeek()
```


Ermittelt den Wochentag, der von dieser Instanz dargestellt wird.

**Returns:**
int - Der Wochentag dieses DateTime-Wertes.
### getDayOfYear() {#getDayOfYear--}
```
public int getDayOfYear()
```


Ermittelt den Tag des Jahres, der von dieser Instanz dargestellt wird.

**Returns:**
int - Der Tag des Jahres, ausgedrückt als ein Wert zwischen 1 und 366.
### getHour() {#getHour--}
```
public int getHour()
```


Ermittelt die Stundenkomponente des Datums, das von dieser Instanz dargestellt wird.

**Returns:**
int - Die Stundenkomponente, ausgedrückt als ein Wert zwischen 0 und 23.
### getMillisecond() {#getMillisecond--}
```
public int getMillisecond()
```


Ermittelt die Millisekundenkomponente des Datums, das von dieser Instanz dargestellt wird.

**Returns:**
int - Die Millisekundenkomponente, ausgedrückt als ein Wert zwischen 0 und 999.
### getMinute() {#getMinute--}
```
public int getMinute()
```


Ermittelt die Minutenkomponente des Datums, das von dieser Instanz dargestellt wird.

**Returns:**
int - Die Minutenkomponente, ausgedrückt als ein Wert zwischen 0 und 59.
### getMonth() {#getMonth--}
```
public int getMonth()
```


Liefert die Monatskomponente des von dieser Instanz dargestellten Datums.

**Returns:**
int - Die Monatskomponente, ausgedrückt als ein Wert zwischen 1 und 12.
### getNow() {#getNow--}
```
public static DateTime getNow()
```


Liefert ein DateTime-Objekt, das auf das aktuelle Datum und die aktuelle Uhrzeit dieses Computers eingestellt ist und als lokale Zeit ausgedrückt wird.

**Returns:**
[DateTime](../../com.aspose.gridweb/datetime) - A DateTime object whose value is the current local date and time.
### getSecond() {#getSecond--}
```
public int getSecond()
```


Liefert die Sekundenkomponente des von dieser Instanz dargestellten Datums.

**Returns:**
int - Die Sekunden, zwischen 0 und 59.
### getYear() {#getYear--}
```
public int getYear()
```


Liefert die Jahreskomponente des von dieser Instanz dargestellten Datums.

**Returns:**
int - Das Jahr, zwischen 1 und 9999.
### hashCode() {#hashCode--}
```
public int hashCode()
```


Gibt den Hashcode für diese Instanz zurück.

**Returns:**
int - Ein 32‑Bit vorzeichenbehafteter Integer-Hashcode.
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


Konvertiert den Wert des aktuellen DateTime-Objekts in ein Calendar-Objekt.

**Returns:**
java.util.Calendar - Kalenderobjekt
### toDate() {#toDate--}
```
public Date toDate()
```


Konvertiert den Wert des aktuellen DateTime-Objekts in ein Date-Objekt.

**Returns:**
java.util.Date - Datumsobjekt
### toLocalTime() {#toLocalTime--}
```
public DateTime toLocalTime()
```


Konvertiert den Wert des aktuellen DateTime-Objekts in die lokale Zeit.

**Returns:**
[DateTime](../../com.aspose.gridweb/datetime) - A DateTime object of local
### toString() {#toString--}
```
public String toString()
```


Konvertiert den Wert des aktuellen DateTime-Objekts in seine äquivalente Zeichenkettenrepräsentation.

**Returns:**
java.lang.String - Eine Zeichenketten-Darstellung des Werts des aktuellen DateTime-Objekts.
### toUniversalTime() {#toUniversalTime--}
```
public DateTime toUniversalTime()
```


Konvertiert den Wert des aktuellen DateTime-Objekts in die koordinierte Weltzeit (UTC).

**Returns:**
[DateTime](../../com.aspose.gridweb/datetime) - A DateTime object of UTC
### wait() {#wait--}
```
public final void wait()
```




### wait(long arg0) {#wait-long-}
```
public final native void wait(long arg0)
```




**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

