---
title: "DateTime"
second_title: "Aspose.Cells för Java API-referens"
description: "Representerar ett ögonblick i tiden som vanligtvis uttrycks som ett datum och en tid på dagen."
type: docs
url: /sv/java/com.aspose.cells/datetime/
---

**Inheritance:**
java.lang.Object
```
public class DateTime
```

Representerar ett ögonblick i tiden, vanligtvis uttryckt som ett datum och en tid på dagen.
## Konstruktörer

| Konstruktör | Beskrivning |
| --- | --- |
| [DateTime(int year, int month, int day)](#DateTime-int-int-int-) | Initierar en ny instans av DateTime-objektet till det angivna året, månaden och dagen. |
| [DateTime(int year, int month, int day, int hour, int minute, int second)](#DateTime-int-int-int-int-int-int-) | Initierar en ny instans av DateTime-objektet till det angivna året, månaden, dagen, timmen, minuten och sekunden. |
| [DateTime(int year, int month, int day, int hour, int minute, int second, int millisecond)](#DateTime-int-int-int-int-int-int-int-) | Initierar en ny instans av DateTime-objektet till det angivna året, månaden, dagen, timmen, minuten, sekunden och millisekunden. |
| [DateTime(Date date)](#DateTime-java.util.Date-) | Initierar en ny instans av DateTime-objektet till det angivna Date-objektet |
| [DateTime(Calendar cld)](#DateTime-java.util.Calendar-) | Initierar en ny instans av DateTime-objektet till det angivna Calendar-objektet |
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [addDays(double value)](#addDays-double-) | Lägger till det angivna antalet dagar till värdet av denna instans. |
| [addHours(double value)](#addHours-double-) | Lägger till det angivna antalet timmar till värdet av denna instans. |
| [addMilliseconds(double value)](#addMilliseconds-double-) | Lägger till det angivna antalet millisekunder till värdet av denna instans. |
| [addMinutes(double value)](#addMinutes-double-) | Lägger till det angivna antalet minuter till värdet av denna instans. |
| [addMonths(int months)](#addMonths-int-) | Lägger till det angivna antalet månader till värdet av denna instans. |
| [addSeconds(double value)](#addSeconds-double-) | Lägger till det angivna antalet sekunder till värdet av denna instans. |
| [addYears(int value)](#addYears-int-) | Lägger till det angivna antalet år till värdet av denna instans. |
| [compareTo(DateTime value)](#compareTo-com.aspose.cells.DateTime-) | Jämför värdet av denna instans med ett angivet DateTime‑värde och returnerar ett heltal som indikerar om denna instans är tidigare än, samma som eller senare än det angivna DateTime‑värdet. |
| [compareTo(Object value)](#compareTo-java.lang.Object-) | Jämför värdet av denna instans med ett angivet objekt som innehåller ett angivet DateTime‑värde och returnerar ett heltal som indikerar om denna instans är tidigare än, samma som eller senare än det angivna DateTime‑värdet. |
| [equals(Object value)](#equals-java.lang.Object-) | Returnerar ett värde som indikerar om denna instans är lika med ett angivet objekt. |
| [getClass()](#getClass--) |  |
| [getDay()](#getDay--) | Hämtar dagen i månaden som representeras av denna instans. |
| [getDayOfWeek()](#getDayOfWeek--) | Hämtar veckodagen som representeras av denna instans. |
| [getDayOfYear()](#getDayOfYear--) | Hämtar dagen på året som representeras av denna instans. |
| [getHour()](#getHour--) | Hämtar timkomponenten i datumet som representeras av denna instans. |
| [getMillisecond()](#getMillisecond--) | Hämtar millisekundkomponenten i datumet som representeras av denna instans. |
| [getMinute()](#getMinute--) | Hämtar minutkomponenten i datumet som representeras av denna instans. |
| [getMonth()](#getMonth--) | Hämtar månadskomponenten i datumet som representeras av denna instans. |
| [getNow()](#getNow--) | Hämtar ett DateTime‑objekt som är inställt på det aktuella datumet och tiden på den här datorn, uttryckt som lokal tid. |
| [getSecond()](#getSecond--) | Hämtar sekundkomponenten i datumet som representeras av denna instans. |
| [getYear()](#getYear--) | Hämtar årskomponenten i datumet som representeras av detta objekt. |
| [hashCode()](#hashCode--) | Returnerar hashkoden för detta objekt. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [toCalendar()](#toCalendar--) | Konverterar värdet för det aktuella DateTime-objektet till ett Calendar-objekt. |
| [toDate()](#toDate--) | Konverterar värdet för det aktuella DateTime-objektet till ett Date-objekt. |
| [toLocalTime()](#toLocalTime--) | Konverterar värdet för det aktuella DateTime-objektet till lokal tid. |
| [toString()](#toString--) | Konverterar värdet för det aktuella DateTime-objektet till dess motsvarande strängrepresentation. |
| [toUniversalTime()](#toUniversalTime--) | Konverterar värdet för det aktuella DateTime-objektet till koordinerad universell tid (UTC). |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### DateTime(int year, int month, int day) {#DateTime-int-int-int-}
```
public DateTime(int year, int month, int day)
```


Initierar en ny instans av DateTime-objektet till det angivna året, månaden och dagen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| år | int | Året (1 till 9999). |
| månad | int | Månad (1 till 12). |
| dag | int | Dag (1 till antalet dagar i månaden). |

### DateTime(int year, int month, int day, int hour, int minute, int second) {#DateTime-int-int-int-int-int-int-}
```
public DateTime(int year, int month, int day, int hour, int minute, int second)
```


Initierar en ny instans av DateTime-objektet till det angivna året, månaden, dagen, timmen, minuten och sekunden.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| år | int | Året (1 till 9999). |
| månad | int | Månad (1 till 12). |
| dag | int | Dag (1 till antalet dagar i månaden). |
| timme | int | Timmar (0 till 23). |
| minut | int | Minuter (0 till 59). |
| sekund | int | Sekunder (0 till 59). |

### DateTime(int year, int month, int day, int hour, int minute, int second, int millisecond) {#DateTime-int-int-int-int-int-int-int-}
```
public DateTime(int year, int month, int day, int hour, int minute, int second, int millisecond)
```


Initierar en ny instans av DateTime-objektet till det angivna året, månaden, dagen, timmen, minuten, sekunden och millisekunden.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| år | int | Året (1 till 9999). |
| månad | int | Månad (1 till 12). |
| dag | int | Dag (1 till antalet dagar i månaden). |
| timme | int | Timmar (0 till 23). |
| minut | int | Minuter (0 till 59). |
| sekund | int | Sekunder (0 till 59). |
| millisekund | int | Millisekunder (0 till 999). |

### DateTime(Date date) {#DateTime-java.util.Date-}
```
public DateTime(Date date)
```


Initierar en ny instans av DateTime-objektet till det angivna Date-objektet

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| datum | java.util.Date | Date-objektet |

### DateTime(Calendar cld) {#DateTime-java.util.Calendar-}
```
public DateTime(Calendar cld)
```


Initierar en ny instans av DateTime-objektet till det angivna Calendar-objektet

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| cld | java.util.Calendar | Calendar-objektet |

### addDays(double value) {#addDays-double-}
```
public DateTime addDays(double value)
```


Lägger till det angivna antalet dagar till värdet av denna instans.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | double | Ett antal hela och bråkdelar dagar. Värdeparametern kan vara negativ eller positiv. |

**Returns:**
[DateTime](../../com.aspose.cells/datetime) - A DateTime object whose value is the sum of the date and time represented by this instance and the number of days represented by value.
### addHours(double value) {#addHours-double-}
```
public DateTime addHours(double value)
```


Lägger till det angivna antalet timmar till värdet av denna instans.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | double | Ett antal hela och bråkdelar timmar. Värdeparametern kan vara negativ eller positiv. |

**Returns:**
[DateTime](../../com.aspose.cells/datetime) - A DateTime object whose value is the sum of the date and time represented by this instance and the number of hours represented by value.
### addMilliseconds(double value) {#addMilliseconds-double-}
```
public DateTime addMilliseconds(double value)
```


Lägger till det angivna antalet millisekunder till värdet av denna instans.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | double | Ett antal hela och bråkdelar millisekunder. Värdeparametern kan vara negativ eller positiv. Observera att detta värde avrundas till närmaste heltal. |

**Returns:**
[DateTime](../../com.aspose.cells/datetime) - A DateTime object whose value is the sum of the date and time represented by this instance and the number of milliseconds represented by value.
### addMinutes(double value) {#addMinutes-double-}
```
public DateTime addMinutes(double value)
```


Lägger till det angivna antalet minuter till värdet av denna instans.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | double | Ett antal hela och bråkdelar minuter. Värdeparametern kan vara negativ eller positiv. |

**Returns:**
[DateTime](../../com.aspose.cells/datetime) - A DateTime object whose value is the sum of the date and time represented by this instance and the number of minutes represented by value.
### addMonths(int months) {#addMonths-int-}
```
public DateTime addMonths(int months)
```


Lägger till det angivna antalet månader till värdet av denna instans.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| månader | int | Ett antal månader. months‑parametern kan vara negativ eller positiv. |

**Returns:**
[DateTime](../../com.aspose.cells/datetime) - A DateTime object whose value is the sum of the date and time represented by this instance and months.
### addSeconds(double value) {#addSeconds-double-}
```
public DateTime addSeconds(double value)
```


Lägger till det angivna antalet sekunder till värdet av denna instans.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | double | Ett antal hela och bråkdelar av sekunder. value‑parametern kan vara negativ eller positiv. |

**Returns:**
[DateTime](../../com.aspose.cells/datetime) - A DateTime object whose value is the sum of the date and time represented by this instance and the number of seconds represented by value.
### addYears(int value) {#addYears-int-}
```
public DateTime addYears(int value)
```


Lägger till det angivna antalet år till värdet av denna instans.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int | Ett antal år. value‑parametern kan vara negativ eller positiv. |

**Returns:**
[DateTime](../../com.aspose.cells/datetime) - A DateTime object whose value is the sum of the date and time represented by this instance and the number of years represented by value.
### compareTo(DateTime value) {#compareTo-com.aspose.cells.DateTime-}
```
public int compareTo(DateTime value)
```


Jämför värdet av denna instans med ett angivet DateTime‑värde och returnerar ett heltal som indikerar om denna instans är tidigare än, samma som eller senare än det angivna DateTime‑värdet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [DateTime](../../com.aspose.cells/datetime) | Ett DateTime‑objekt att jämföra. |

**Returns:**
int - Ett teckenburet tal som indikerar de relativa värdena för detta objekt och value‑parametern. Värde Beskrivning Mindre än noll Detta objekt är tidigare än value. Noll Detta objekt är samma som value. Större än noll Detta objekt är senare än value.
### compareTo(Object value) {#compareTo-java.lang.Object-}
```
public int compareTo(Object value)
```


Jämför värdet av denna instans med ett angivet objekt som innehåller ett angivet DateTime‑värde och returnerar ett heltal som indikerar om denna instans är tidigare än, samma som eller senare än det angivna DateTime‑värdet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.Object | Ett boxed DateTime‑objekt att jämföra, eller null. |

**Returns:**
int - Ett teckenburet tal som indikerar de relativa värdena för detta objekt och value. Värde Beskrivning Mindre än noll Detta objekt är tidigare än value. Noll Detta objekt är samma som value. Större än noll Detta objekt är senare än value, eller value är null.
### equals(Object value) {#equals-java.lang.Object-}
```
public boolean equals(Object value)
```


Returnerar ett värde som indikerar om denna instans är lika med ett angivet objekt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.Object | Ett objekt att jämföra med detta objekt. |

**Returns:**
boolean - sant om value är en instans av DateTime och är lika med värdet för detta objekt; annars falskt.
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


Hämtar dagen i månaden som representeras av denna instans.

**Returns:**
int - Dagkomponenten, uttryckt som ett värde mellan 1 och 31.
### getDayOfWeek() {#getDayOfWeek--}
```
public int getDayOfWeek()
```


Hämtar veckodagen som representeras av denna instans.

**Returns:**
int - veckodagen för detta DateTime‑värde.
### getDayOfYear() {#getDayOfYear--}
```
public int getDayOfYear()
```


Hämtar dagen på året som representeras av denna instans.

**Returns:**
int - Dagen på året, uttryckt som ett värde mellan 1 och 366.
### getHour() {#getHour--}
```
public int getHour()
```


Hämtar timkomponenten i datumet som representeras av denna instans.

**Returns:**
int - Timkomponenten, uttryckt som ett värde mellan 0 och 23.
### getMillisecond() {#getMillisecond--}
```
public int getMillisecond()
```


Hämtar millisekundkomponenten i datumet som representeras av denna instans.

**Returns:**
int - Millisekundkomponenten, uttryckt som ett värde mellan 0 och 999.
### getMinute() {#getMinute--}
```
public int getMinute()
```


Hämtar minutkomponenten i datumet som representeras av denna instans.

**Returns:**
int - Minutkomponenten, uttryckt som ett värde mellan 0 och 59.
### getMonth() {#getMonth--}
```
public int getMonth()
```


Hämtar månadskomponenten i datumet som representeras av denna instans.

**Returns:**
int - Månadskomponenten, uttryckt som ett värde mellan 1 och 12.
### getNow() {#getNow--}
```
public static DateTime getNow()
```


Hämtar ett DateTime‑objekt som är inställt på det aktuella datumet och tiden på den här datorn, uttryckt som lokal tid.

**Returns:**
[DateTime](../../com.aspose.cells/datetime) - A DateTime object whose value is the current local date and time.
### getSecond() {#getSecond--}
```
public int getSecond()
```


Hämtar sekundkomponenten i datumet som representeras av denna instans.

**Returns:**
int - Sekunderna, mellan 0 och 59.
### getYear() {#getYear--}
```
public int getYear()
```


Hämtar årskomponenten i datumet som representeras av detta objekt.

**Returns:**
int - Året, mellan 1 och 9999.
### hashCode() {#hashCode--}
```
public int hashCode()
```


Returnerar hashkoden för detta objekt.

**Returns:**
int - En 32-bitars teckenburet heltalshashkod.
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


Konverterar värdet för det aktuella DateTime-objektet till ett Calendar-objekt.

**Returns:**
java.util.Calendar - Kalenderobjekt
### toDate() {#toDate--}
```
public Date toDate()
```


Konverterar värdet för det aktuella DateTime-objektet till ett Date-objekt.

**Returns:**
java.util.Date - Datumobjekt
### toLocalTime() {#toLocalTime--}
```
public DateTime toLocalTime()
```


Konverterar värdet för det aktuella DateTime-objektet till lokal tid.

**Returns:**
[DateTime](../../com.aspose.cells/datetime) - A DateTime object of local
### toString() {#toString--}
```
public String toString()
```


Konverterar värdet för det aktuella DateTime-objektet till dess motsvarande strängrepresentation.

**Returns:**
java.lang.String - En strängrepresentation av värdet för det aktuella DateTime‑objektet.
### toUniversalTime() {#toUniversalTime--}
```
public DateTime toUniversalTime()
```


Konverterar värdet för det aktuella DateTime-objektet till koordinerad universell tid (UTC).

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

