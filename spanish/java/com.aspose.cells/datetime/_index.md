---
title: "DateTime"
second_title: "Referencia de API de Aspose.Cells para Java"
description: "Representa un instante en el tiempo, típicamente expresado como una fecha y hora del día."
type: docs
url: /es/java/com.aspose.cells/datetime/
---

**Inheritance:**
java.lang.Object
```
public class DateTime
```

Representa un instante en el tiempo, típicamente expresado como una fecha y hora del día.
## Constructores

| Constructor | Descripción |
| --- | --- |
| [DateTime(int year, int month, int day)](#DateTime-int-int-int-) | Inicializa una nueva instancia del objeto DateTime con el año, mes y día especificados. |
| [DateTime(int year, int month, int day, int hour, int minute, int second)](#DateTime-int-int-int-int-int-int-) | Inicializa una nueva instancia del objeto DateTime con el año, mes, día, hora, minuto y segundo especificados. |
| [DateTime(int year, int month, int day, int hour, int minute, int second, int millisecond)](#DateTime-int-int-int-int-int-int-int-) | Inicializa una nueva instancia del objeto DateTime con el año, mes, día, hora, minuto, segundo y milisegundo especificados. |
| [DateTime(Date date)](#DateTime-java.util.Date-) | Inicializa una nueva instancia del objeto DateTime con el objeto Date especificado |
| [DateTime(Calendar cld)](#DateTime-java.util.Calendar-) | Inicializa una nueva instancia del objeto DateTime con el objeto Calendar especificado |
## Métodos

| Método | Descripción |
| --- | --- |
| [addDays(double value)](#addDays-double-) | Agrega la cantidad especificada de días al valor de esta instancia. |
| [addHours(double value)](#addHours-double-) | Agrega la cantidad especificada de horas al valor de esta instancia. |
| [addMilliseconds(double value)](#addMilliseconds-double-) | Agrega la cantidad especificada de milisegundos al valor de esta instancia. |
| [addMinutes(double value)](#addMinutes-double-) | Agrega la cantidad especificada de minutos al valor de esta instancia. |
| [addMonths(int months)](#addMonths-int-) | Agrega la cantidad especificada de meses al valor de esta instancia. |
| [addSeconds(double value)](#addSeconds-double-) | Agrega la cantidad especificada de segundos al valor de esta instancia. |
| [addYears(int value)](#addYears-int-) | Agrega la cantidad especificada de años al valor de esta instancia. |
| [compareTo(DateTime value)](#compareTo-com.aspose.cells.DateTime-) | Compara el valor de esta instancia con un valor DateTime especificado y devuelve un entero que indica si esta instancia es anterior, igual o posterior al valor DateTime especificado. |
| [compareTo(Object value)](#compareTo-java.lang.Object-) | Compara el valor de esta instancia con un objeto especificado que contiene un valor DateTime, y devuelve un entero que indica si esta instancia es anterior, igual o posterior al valor DateTime especificado. |
| [equals(Object value)](#equals-java.lang.Object-) | Devuelve un valor que indica si esta instancia es igual a un objeto especificado. |
| [getClass()](#getClass--) |  |
| [getDay()](#getDay--) | Obtiene el día del mes representado por esta instancia. |
| [getDayOfWeek()](#getDayOfWeek--) | Obtiene el día de la semana representado por esta instancia. |
| [getDayOfYear()](#getDayOfYear--) | Obtiene el día del año representado por esta instancia. |
| [getHour()](#getHour--) | Obtiene el componente de hora de la fecha representada por esta instancia. |
| [getMillisecond()](#getMillisecond--) | Obtiene el componente de milisegundos de la fecha representada por esta instancia. |
| [getMinute()](#getMinute--) | Obtiene el componente de minuto de la fecha representada por esta instancia. |
| [getMonth()](#getMonth--) | Obtiene el componente de mes de la fecha representada por esta instancia. |
| [getNow()](#getNow--) | Obtiene un objeto DateTime que está configurado a la fecha y hora actuales de este equipo, expresado como hora local. |
| [getSecond()](#getSecond--) | Obtiene el componente de segundos de la fecha representada por esta instancia. |
| [getYear()](#getYear--) | Obtiene el componente de año de la fecha representada por esta instancia. |
| [hashCode()](#hashCode--) | Devuelve el código hash de esta instancia. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [toCalendar()](#toCalendar--) | Convierte el valor del objeto DateTime actual a un objeto Calendar. |
| [toDate()](#toDate--) | Convierte el valor del objeto DateTime actual a un objeto Date. |
| [toLocalTime()](#toLocalTime--) | Convierte el valor del objeto DateTime actual a la hora local. |
| [toString()](#toString--) | Convierte el valor del objeto DateTime actual a su representación de cadena equivalente. |
| [toUniversalTime()](#toUniversalTime--) | Convierte el valor del objeto DateTime actual a Tiempo Universal Coordinado(UTC). |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### DateTime(int year, int month, int day) {#DateTime-int-int-int-}
```
public DateTime(int year, int month, int day)
```


Inicializa una nueva instancia del objeto DateTime con el año, mes y día especificados.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| año | int | El año (1 a 9999). |
| mes | int | El mes (1 a 12). |
| día | int | El día (1 al número de días del mes). |

### DateTime(int year, int month, int day, int hour, int minute, int second) {#DateTime-int-int-int-int-int-int-}
```
public DateTime(int year, int month, int day, int hour, int minute, int second)
```


Inicializa una nueva instancia del objeto DateTime con el año, mes, día, hora, minuto y segundo especificados.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| año | int | El año (1 a 9999). |
| mes | int | El mes (1 a 12). |
| día | int | El día (1 al número de días del mes). |
| hora | int | Las horas (0 a 23). |
| minuto | int | Los minutos (0 a 59). |
| segundo | int | Los segundos (0 a 59). |

### DateTime(int year, int month, int day, int hour, int minute, int second, int millisecond) {#DateTime-int-int-int-int-int-int-int-}
```
public DateTime(int year, int month, int day, int hour, int minute, int second, int millisecond)
```


Inicializa una nueva instancia del objeto DateTime con el año, mes, día, hora, minuto, segundo y milisegundo especificados.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| año | int | El año (1 a 9999). |
| mes | int | El mes (1 a 12). |
| día | int | El día (1 al número de días del mes). |
| hora | int | Las horas (0 a 23). |
| minuto | int | Los minutos (0 a 59). |
| segundo | int | Los segundos (0 a 59). |
| milisegundo | int | Los milisegundos (0 a 999). |

### DateTime(Date date) {#DateTime-java.util.Date-}
```
public DateTime(Date date)
```


Inicializa una nueva instancia del objeto DateTime con el objeto Date especificado

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fecha | java.util.Date | El objeto Date |

### DateTime(Calendar cld) {#DateTime-java.util.Calendar-}
```
public DateTime(Calendar cld)
```


Inicializa una nueva instancia del objeto DateTime con el objeto Calendar especificado

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| cld | java.util.Calendar | El objeto Calendar |

### addDays(double value) {#addDays-double-}
```
public DateTime addDays(double value)
```


Agrega la cantidad especificada de días al valor de esta instancia.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | double | Un número de días enteros y fraccionarios. El parámetro value puede ser negativo o positivo. |

**Returns:**
[DateTime](../../com.aspose.cells/datetime) - A DateTime object whose value is the sum of the date and time represented by this instance and the number of days represented by value.
### addHours(double value) {#addHours-double-}
```
public DateTime addHours(double value)
```


Agrega la cantidad especificada de horas al valor de esta instancia.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | double | Un número de horas enteras y fraccionarias. El parámetro value puede ser negativo o positivo. |

**Returns:**
[DateTime](../../com.aspose.cells/datetime) - A DateTime object whose value is the sum of the date and time represented by this instance and the number of hours represented by value.
### addMilliseconds(double value) {#addMilliseconds-double-}
```
public DateTime addMilliseconds(double value)
```


Agrega la cantidad especificada de milisegundos al valor de esta instancia.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | double | Un número de milisegundos enteros y fraccionarios. El parámetro value puede ser negativo o positivo. Tenga en cuenta que este valor se redondea al entero más cercano. |

**Returns:**
[DateTime](../../com.aspose.cells/datetime) - A DateTime object whose value is the sum of the date and time represented by this instance and the number of milliseconds represented by value.
### addMinutes(double value) {#addMinutes-double-}
```
public DateTime addMinutes(double value)
```


Agrega la cantidad especificada de minutos al valor de esta instancia.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | double | Un número de minutos enteros y fraccionarios. El parámetro value puede ser negativo o positivo. |

**Returns:**
[DateTime](../../com.aspose.cells/datetime) - A DateTime object whose value is the sum of the date and time represented by this instance and the number of minutes represented by value.
### addMonths(int months) {#addMonths-int-}
```
public DateTime addMonths(int months)
```


Agrega la cantidad especificada de meses al valor de esta instancia.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| meses | int | Un número de meses. El parámetro months puede ser negativo o positivo. |

**Returns:**
[DateTime](../../com.aspose.cells/datetime) - A DateTime object whose value is the sum of the date and time represented by this instance and months.
### addSeconds(double value) {#addSeconds-double-}
```
public DateTime addSeconds(double value)
```


Agrega la cantidad especificada de segundos al valor de esta instancia.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | double | Un número de segundos enteros y fraccionarios. El parámetro value puede ser negativo o positivo. |

**Returns:**
[DateTime](../../com.aspose.cells/datetime) - A DateTime object whose value is the sum of the date and time represented by this instance and the number of seconds represented by value.
### addYears(int value) {#addYears-int-}
```
public DateTime addYears(int value)
```


Agrega la cantidad especificada de años al valor de esta instancia.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int | Un número de años. El parámetro value puede ser negativo o positivo. |

**Returns:**
[DateTime](../../com.aspose.cells/datetime) - A DateTime object whose value is the sum of the date and time represented by this instance and the number of years represented by value.
### compareTo(DateTime value) {#compareTo-com.aspose.cells.DateTime-}
```
public int compareTo(DateTime value)
```


Compara el valor de esta instancia con un valor DateTime especificado y devuelve un entero que indica si esta instancia es anterior, igual o posterior al valor DateTime especificado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | [DateTime](../../com.aspose.cells/datetime) | Un objeto DateTime para comparar. |

**Returns:**
int - Un número con signo que indica los valores relativos de esta instancia y el parámetro value. Descripción del valor Menor que cero Esta instancia es anterior a value. Cero Esta instancia es igual a value. Mayor que cero Esta instancia es posterior a value.
### compareTo(Object value) {#compareTo-java.lang.Object-}
```
public int compareTo(Object value)
```


Compara el valor de esta instancia con un objeto especificado que contiene un valor DateTime, y devuelve un entero que indica si esta instancia es anterior, igual o posterior al valor DateTime especificado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.Object | Un objeto DateTime empaquetado para comparar, o null. |

**Returns:**
int - Un número con signo que indica los valores relativos de esta instancia y value. Descripción del valor Menor que cero Esta instancia es anterior a value. Cero Esta instancia es igual a value. Mayor que cero Esta instancia es posterior a value, o value es null.
### equals(Object value) {#equals-java.lang.Object-}
```
public boolean equals(Object value)
```


Devuelve un valor que indica si esta instancia es igual a un objeto especificado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.Object | Un objeto para comparar con esta instancia. |

**Returns:**
boolean - true si value es una instancia de DateTime y es igual al valor de esta instancia; de lo contrario, false.
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


Obtiene el día del mes representado por esta instancia.

**Returns:**
int - El componente día, expresado como un valor entre 1 y 31.
### getDayOfWeek() {#getDayOfWeek--}
```
public int getDayOfWeek()
```


Obtiene el día de la semana representado por esta instancia.

**Returns:**
int - el día de la semana de este valor DateTime.
### getDayOfYear() {#getDayOfYear--}
```
public int getDayOfYear()
```


Obtiene el día del año representado por esta instancia.

**Returns:**
int - El día del año, expresado como un valor entre 1 y 366.
### getHour() {#getHour--}
```
public int getHour()
```


Obtiene el componente de hora de la fecha representada por esta instancia.

**Returns:**
int - El componente hora, expresado como un valor entre 0 y 23.
### getMillisecond() {#getMillisecond--}
```
public int getMillisecond()
```


Obtiene el componente de milisegundos de la fecha representada por esta instancia.

**Returns:**
int - El componente milisegundos, expresado como un valor entre 0 y 999.
### getMinute() {#getMinute--}
```
public int getMinute()
```


Obtiene el componente de minuto de la fecha representada por esta instancia.

**Returns:**
int - El componente minuto, expresado como un valor entre 0 y 59.
### getMonth() {#getMonth--}
```
public int getMonth()
```


Obtiene el componente de mes de la fecha representada por esta instancia.

**Returns:**
int - El componente mes, expresado como un valor entre 1 y 12.
### getNow() {#getNow--}
```
public static DateTime getNow()
```


Obtiene un objeto DateTime que está configurado a la fecha y hora actuales de este equipo, expresado como hora local.

**Returns:**
[DateTime](../../com.aspose.cells/datetime) - A DateTime object whose value is the current local date and time.
### getSecond() {#getSecond--}
```
public int getSecond()
```


Obtiene el componente de segundos de la fecha representada por esta instancia.

**Returns:**
int - Los segundos, entre 0 y 59.
### getYear() {#getYear--}
```
public int getYear()
```


Obtiene el componente de año de la fecha representada por esta instancia.

**Returns:**
int - El año, entre 1 y 9999.
### hashCode() {#hashCode--}
```
public int hashCode()
```


Devuelve el código hash de esta instancia.

**Returns:**
int - Un código hash de entero con signo de 32 bits.
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


Convierte el valor del objeto DateTime actual a un objeto Calendar.

**Returns:**
java.util.Calendar - Objeto Calendar
### toDate() {#toDate--}
```
public Date toDate()
```


Convierte el valor del objeto DateTime actual a un objeto Date.

**Returns:**
java.util.Date - Objeto Date
### toLocalTime() {#toLocalTime--}
```
public DateTime toLocalTime()
```


Convierte el valor del objeto DateTime actual a la hora local.

**Returns:**
[DateTime](../../com.aspose.cells/datetime) - A DateTime object of local
### toString() {#toString--}
```
public String toString()
```


Convierte el valor del objeto DateTime actual a su representación de cadena equivalente.

**Returns:**
java.lang.String - Una representación en cadena del valor del objeto DateTime actual.
### toUniversalTime() {#toUniversalTime--}
```
public DateTime toUniversalTime()
```


Convierte el valor del objeto DateTime actual a Tiempo Universal Coordinado(UTC).

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
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

