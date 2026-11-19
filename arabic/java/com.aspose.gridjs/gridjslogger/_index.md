---
title: "GridJsLogger"
second_title: "Aspose.Cells for Java API Reference"
description: "يوفر نظام تسجيل خفيف الوزن لخادم GridJs."
type: docs
url: /ar/java/com.aspose.gridjs/gridjslogger/
---

**Inheritance:**
java.lang.Object
```
public class GridJsLogger
```

يوفر نظام تسجيل خفيف الوزن لخادم GridJs. يدعم الإخراج إلى وحدة التحكم والملف مع مستويات سجل قابلة للتكوين. المستوى الافتراضي هو None. في بناء DEBUG، المستوى الافتراضي هو Debug (يعرض جميع الرسائل). يدعم تدوير ملفات السجل يوميًا/أسبوعيًا/شهريًا.
## الطرق

| طريقة | الوصف |
| --- | --- |
| [closeLogFile()](#closeLogFile--) | يغلق كاتب ملف السجل ويعطل إخراج الملف. |
| [debug(String message)](#debug-java.lang.String-) | يسجل رسالة بمستوى debug. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [error(String message)](#error-java.lang.String-) | يسجل رسالة بمستوى error. |
| [getClass()](#getClass--) |  |
| [getEnableConsoleOutput()](#getEnableConsoleOutput--) | يحصل على ما إذا كان سيتم إخراج رسائل السجل إلى وحدة التحكم. |
| [getEnableFileOutput()](#getEnableFileOutput--) | يحصل على ما إذا كان سيتم إخراج رسائل السجل إلى ملف. |
| [getLevel()](#getLevel--) | يحصل على الحد الأدنى لمستوى السجل. |
| [getLogFilePath()](#getLogFilePath--) | يحصل على مسار ملف السجل الحالي، أو null إذا لم يتم تعيينه. |
| [getMaxFileSize()](#getMaxFileSize--) | يحصل على الحد الأقصى للحجم (بالبايت) لملف سجل واحد قبل التدوير. |
| [hashCode()](#hashCode--) |  |
| [info(String message)](#info-java.lang.String-) | يسجل رسالة بمستوى info. |
| [log(int level, String message)](#log-int-java.lang.String-) | يسجل رسالة بالمستوى المحدد. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setEnableConsoleOutput(boolean value)](#setEnableConsoleOutput-boolean-) | يضبط ما إذا كان سيتم إخراج رسائل السجل إلى وحدة التحكم. |
| [setEnableFileOutput(boolean value)](#setEnableFileOutput-boolean-) | يضبط ما إذا كان سيتم إخراج رسائل السجل إلى ملف. |
| [setLevel(int value)](#setLevel-int-) | يضبط الحد الأدنى لمستوى السجل. |
| [setLogDirectory(String directory)](#setLogDirectory-java.lang.String-) | يضبط دليل السجل باستخدام استراتيجية تدوير الملفات اليومية ويفعل إخراج الملف. |
| [setLogDirectory(String directory, int rolling)](#setLogDirectory-java.lang.String-int-) | يضبط دليل السجل باستخدام استراتيجية تدوير الملفات ويفعل إخراج الملف. |
| [setLogDirectory(String directory, int rolling, String filePrefix)](#setLogDirectory-java.lang.String-int-java.lang.String-) | يضبط دليل السجل باستخدام استراتيجية تدوير الملفات ويفعل إخراج الملف. |
| [setLogFile(String filePath)](#setLogFile-java.lang.String-) | يضبط مسار ملف السجل ويفعل إخراج الملف (وضع ملف واحد، بدون تدوير). |
| [setLogFile(String filePath, boolean append)](#setLogFile-java.lang.String-boolean-) | يضبط مسار ملف السجل ويفعل إخراج الملف (وضع ملف واحد، بدون تدوير). |
| [setMaxFileSize(long value)](#setMaxFileSize-long-) | يضبط الحد الأقصى للحجم (بالبايت) لملف سجل واحد قبل التدوير. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
| [warn(String message)](#warn-java.lang.String-) | يسجل رسالة بمستوى التحذير. |
### closeLogFile() {#closeLogFile--}
```
public static void closeLogFile()
```


يغلق كاتب ملف السجل ويعطل إخراج الملف.

### debug(String message) {#debug-java.lang.String-}
```
public static void debug(String message)
```


يسجل رسالة بمستوى debug.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| رسالة | java.lang.String |  |

### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| arg0 | java.lang.Object |  |

**Returns:**
boolean
### error(String message) {#error-java.lang.String-}
```
public static void error(String message)
```


يسجل رسالة بمستوى error.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| رسالة | java.lang.String |  |

### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getEnableConsoleOutput() {#getEnableConsoleOutput--}
```
public static boolean getEnableConsoleOutput()
```


يحصل على ما إذا كان سيتم إخراج رسائل السجل إلى وحدة التحكم. القيمة الافتراضية هي false.

**Returns:**
boolean
### getEnableFileOutput() {#getEnableFileOutput--}
```
public static boolean getEnableFileOutput()
```


يحصل على ما إذا كان سيتم إخراج رسائل السجل إلى ملف. القيمة الافتراضية هي false. يجب استدعاء [setLogFile(String)](../../com.aspose.gridjs/gridjslogger\#setLogFile-String-) أو [setLogDirectory(String)](../../com.aspose.gridjs/gridjslogger\#setLogDirectory-String-) قبل التفعيل.

**Returns:**
boolean
### getLevel() {#getLevel--}
```
public static int getLevel()
```


يحصل على الحد الأدنى لمستوى السجل. سيتم تجاهل الرسائل التي أدنى من هذا المستوى. القيمة الافتراضية هي None.

انظر [GridJsLogLevel](../../com.aspose.gridjs/gridjsloglevel).

**Returns:**
int
### getLogFilePath() {#getLogFilePath--}
```
public static String getLogFilePath()
```


يحصل على مسار ملف السجل الحالي، أو null إذا لم يتم تعيينه.

**Returns:**
java.lang.String
### getMaxFileSize() {#getMaxFileSize--}
```
public static long getMaxFileSize()
```


يحصل على الحد الأقصى للحجم (بالبايت) لملف سجل واحد قبل التدوير. يكون فعالًا فقط عندما يكون التدوير مفعلاً. 0 يعني عدم وجود حد للحجم. القيمة الافتراضية هي 0.

**Returns:**
long
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### info(String message) {#info-java.lang.String-}
```
public static void info(String message)
```


يسجل رسالة بمستوى info.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| رسالة | java.lang.String |  |

### log(int level, String message) {#log-int-java.lang.String-}
```
public static void log(int level, String message)
```


يسجل رسالة بالمستوى المحدد.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| level | int | [GridJsLogLevel](../../com.aspose.gridjs/gridjsloglevel). مستوى السجل. |
| رسالة | java.lang.String | الرسالة المراد تسجيلها. |

### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### setEnableConsoleOutput(boolean value) {#setEnableConsoleOutput-boolean-}
```
public static void setEnableConsoleOutput(boolean value)
```


يضبط ما إذا كان سيتم إخراج رسائل السجل إلى وحدة التحكم. القيمة الافتراضية هي false.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setEnableFileOutput(boolean value) {#setEnableFileOutput-boolean-}
```
public static void setEnableFileOutput(boolean value)
```


يضبط ما إذا كان سيتم إخراج رسائل السجل إلى ملف. القيمة الافتراضية هي false. يجب استدعاء [setLogFile(String)](../../com.aspose.gridjs/gridjslogger\#setLogFile-String-) أو [setLogDirectory(String)](../../com.aspose.gridjs/gridjslogger\#setLogDirectory-String-) قبل التفعيل.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setLevel(int value) {#setLevel-int-}
```
public static void setLevel(int value)
```


يضبط الحد الأدنى لمستوى السجل. سيتم تجاهل الرسائل التي أدنى من هذا المستوى. القيمة الافتراضية هي None.

انظر [GridJsLogLevel](../../com.aspose.gridjs/gridjsloglevel).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setLogDirectory(String directory) {#setLogDirectory-java.lang.String-}
```
public static void setLogDirectory(String directory)
```


يضبط دليل السجل باستخدام استراتيجية تدوير الملفات اليومية ويفعل إخراج الملف. سيتم تسمية ملفات السجل كالتالي: gridjs\_\{period\}.log

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| الدليل | java.lang.String | الدليل لتخزين ملفات السجل. |

### setLogDirectory(String directory, int rolling) {#setLogDirectory-java.lang.String-int-}
```
public static void setLogDirectory(String directory, int rolling)
```


يضبط دليل السجل باستخدام استراتيجية تدوير الملفات ويفعل إخراج الملف. سيتم تسمية ملفات السجل كالتالي: gridjs\_\{period\}.log

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| الدليل | java.lang.String | الدليل لتخزين ملفات السجل. |
| rolling | int | [GridJsLogRolling](../../com.aspose.gridjs/gridjslogrolling). استراتيجية التدوير (يومي/أسبوعي/شهري). |

### setLogDirectory(String directory, int rolling, String filePrefix) {#setLogDirectory-java.lang.String-int-java.lang.String-}
```
public static void setLogDirectory(String directory, int rolling, String filePrefix)
```


يضبط دليل السجل باستخدام استراتيجية تدوير الملفات ويفعل إخراج الملف. سيتم تسمية ملفات السجل كالتالي: \{prefix\}\_\{period\}.log أمثلة: gridjs\_2026-07-27.log (يومي)، gridjs\_2026-W30.log (أسبوعي)، gridjs\_2026-07.log (شهري)

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| الدليل | java.lang.String | الدليل لتخزين ملفات السجل. |
| rolling | int | [GridJsLogRolling](../../com.aspose.gridjs/gridjslogrolling). استراتيجية التدوير (يومي/أسبوعي/شهري). |
| filePrefix | java.lang.String | بادئة اسم الملف. |

### setLogFile(String filePath) {#setLogFile-java.lang.String-}
```
public static void setLogFile(String filePath)
```


يضبط مسار ملف السجل ويفعل إخراج الملف (وضع ملف واحد، بدون تدوير). يلحق بالملف الموجود.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| filePath | java.lang.String | المسار الكامل لملف السجل. |

### setLogFile(String filePath, boolean append) {#setLogFile-java.lang.String-boolean-}
```
public static void setLogFile(String filePath, boolean append)
```


يضبط مسار ملف السجل ويفعل إخراج الملف (وضع ملف واحد، بدون تدوير).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| filePath | java.lang.String | المسار الكامل لملف السجل. |
| إلحاق | boolean | ما إذا كان سيتم الإلحاق بالملف الموجود. |

### setMaxFileSize(long value) {#setMaxFileSize-long-}
```
public static void setMaxFileSize(long value)
```


يضبط الحد الأقصى للحجم (بالبايت) لملف سجل واحد قبل التدوير. يكون فعالًا فقط عندما يكون التدوير مفعلاً. 0 يعني عدم وجود حد للحجم. القيمة الافتراضية هي 0.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | long |  |

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
| معامل | نوع | الوصف |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

### warn(String message) {#warn-java.lang.String-}
```
public static void warn(String message)
```


يسجل رسالة بمستوى التحذير.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| رسالة | java.lang.String |  |

