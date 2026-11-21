---
title: "AutoFitterOptions"
second_title: "Aspose.Cells för Java API-referens"
description: "Representerar alla alternativ för automatisk anpassning."
type: docs
url: /sv/java/com.aspose.cells/autofitteroptions/
---

**Inheritance:**
java.lang.Object
```
public class AutoFitterOptions
```

Representerar alla alternativ för automatisk anpassning.
## Konstruktörer

| Konstruktör | Beskrivning |
| --- | --- |
| [AutoFitterOptions()](#AutoFitterOptions--) |  |
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAutoFitMergedCells()](#getAutoFitMergedCells--) | Anger om radens höjd automatiskt anpassas när cellerna är sammanslagna i en rad. |
| [getAutoFitMergedCellsType()](#getAutoFitMergedCellsType--) | Hämtar typen av automatisk anpassning av radens höjd för sammanslagna celler. |
| [getAutoFitWrappedTextType()](#getAutoFitWrappedTextType--) | Hämtar typen av automatisk anpassning av radbruten text. |
| [getClass()](#getClass--) |  |
| [getDefaultEditLanguage()](#getDefaultEditLanguage--) | Hämtar standardspråk för redigering. |
| [getForRendering()](#getForRendering--) | Anger om anpassning för renderingsändamål. |
| [getFormatStrategy()](#getFormatStrategy--) | Hämtar den formaterade strategin. |
| [getIgnoreHidden()](#getIgnoreHidden--) | Ignorerar dolda rader/kolumner. |
| [getMaxRowHeight()](#getMaxRowHeight--) | Hämtar den maximala radhöjden (i enheten Punkt) när rader automatiskt anpassas. |
| [getOnlyAuto()](#getOnlyAuto--) | Anger om endast rader vars höjd inte är anpassad ska anpassas. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAutoFitMergedCells(boolean value)](#setAutoFitMergedCells-boolean-) | Anger om radens höjd automatiskt anpassas när cellerna är sammanslagna i en rad. |
| [setAutoFitMergedCellsType(int value)](#setAutoFitMergedCellsType-int-) | Ställer in typen av automatisk anpassning av radhöjd för sammanslagna celler. |
| [setAutoFitWrappedTextType(int value)](#setAutoFitWrappedTextType-int-) | Ställer in typen av automatisk anpassning av radbrutet text. |
| [setDefaultEditLanguage(int value)](#setDefaultEditLanguage-int-) | Ställer in standardspråk för redigering. |
| [setForRendering(boolean value)](#setForRendering-boolean-) | Anger om anpassning för renderingsändamål. |
| [setFormatStrategy(int value)](#setFormatStrategy-int-) | Ställer in den formaterade strategin. |
| [setIgnoreHidden(boolean value)](#setIgnoreHidden-boolean-) | Ignorerar dolda rader/kolumner. |
| [setMaxRowHeight(double value)](#setMaxRowHeight-double-) | Ställer in den maximala radhöjden (i enheten Punkt) när rader automatiskt anpassas. |
| [setOnlyAuto(boolean value)](#setOnlyAuto-boolean-) | Anger om endast rader vars höjd inte är anpassad ska anpassas. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### AutoFitterOptions() {#AutoFitterOptions--}
```
public AutoFitterOptions()
```


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
### getAutoFitMergedCells() {#getAutoFitMergedCells--}
```
public boolean getAutoFitMergedCells()
```


Anger om radhöjden automatiskt ska anpassas när cellerna är sammanslagna i en rad. Standardvärdet är falskt.

**Remarks**

OBS: Denna medlem är nu föråldrad. Använd istället egenskapen AutoFitterOptions.AutoFitMergedCellsType. Denna egenskap kommer att tas bort 12 månader senare sedan december 2018. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Returns:**
boolean
### getAutoFitMergedCellsType() {#getAutoFitMergedCellsType--}
```
public int getAutoFitMergedCellsType()
```


Hämtar typen av automatisk anpassning av radens höjd för sammanslagna celler.

Se [AutoFitMergedCellsType](../../com.aspose.cells/autofitmergedcellstype).

**Remarks**

Excel ignorerar som standard sammanslagna celler när radhöjden anpassas, så Aspose.Cells fungerar enligt MS Excels standard. Vänligen ställ in denna typ för att ändra hur den automatiska anpassningen av radhöjd för sammanslagna celler sker.

**Returns:**
int
### getAutoFitWrappedTextType() {#getAutoFitWrappedTextType--}
```
public int getAutoFitWrappedTextType()
```


Hämtar typen av automatisk anpassning av radbruten text.

Se [AutoFitWrappedTextType](../../com.aspose.cells/autofitwrappedtexttype).

**Returns:**
int
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getDefaultEditLanguage() {#getDefaultEditLanguage--}
```
public int getDefaultEditLanguage()
```


Hämtar standardspråk för redigering.

Se [DefaultEditLanguage](../../com.aspose.cells/defaulteditlanguage).

**Remarks**

Det kan visa/rendera olika layouter för textparagraf när olika redigeringsspråk är inställda. Standard är [DefaultEditLanguage.AUTO](../../com.aspose.cells/defaulteditlanguage\#AUTO).

**Returns:**
int
### getForRendering() {#getForRendering--}
```
public boolean getForRendering()
```


Anger om anpassning för renderingsändamål.

**Returns:**
boolean
### getFormatStrategy() {#getFormatStrategy--}
```
public int getFormatStrategy()
```


Hämtar den formaterade strategin.

Se [CellValueFormatStrategy](../../com.aspose.cells/cellvalueformatstrategy).

**Remarks**

Standardvärdet är CellStyle för prestanda.

**Returns:**
int
### getIgnoreHidden() {#getIgnoreHidden--}
```
public boolean getIgnoreHidden()
```


Ignorerar dolda rader/kolumner.

**Returns:**
boolean
### getMaxRowHeight() {#getMaxRowHeight--}
```
public double getMaxRowHeight()
```


Hämtar den maximala radhöjden (i enheten Punkt) när rader automatiskt anpassas.

**Returns:**
double
### getOnlyAuto() {#getOnlyAuto--}
```
public boolean getOnlyAuto()
```


Anger om endast rader vars höjd inte är anpassad ska anpassas.

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




### setAutoFitMergedCells(boolean value) {#setAutoFitMergedCells-boolean-}
```
public void setAutoFitMergedCells(boolean value)
```


Anger om radhöjden automatiskt ska anpassas när cellerna är sammanslagna i en rad. Standardvärdet är falskt.

**Remarks**

OBS: Denna medlem är nu föråldrad. Använd istället egenskapen AutoFitterOptions.AutoFitMergedCellsType. Denna egenskap kommer att tas bort 12 månader senare sedan december 2018. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setAutoFitMergedCellsType(int value) {#setAutoFitMergedCellsType-int-}
```
public void setAutoFitMergedCellsType(int value)
```


Ställer in typen av automatisk anpassning av radhöjd för sammanslagna celler.

Se [AutoFitMergedCellsType](../../com.aspose.cells/autofitmergedcellstype).

**Remarks**

Excel ignorerar som standard sammanslagna celler när radhöjden anpassas, så Aspose.Cells fungerar enligt MS Excels standard. Vänligen ställ in denna typ för att ändra hur den automatiska anpassningen av radhöjd för sammanslagna celler sker.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setAutoFitWrappedTextType(int value) {#setAutoFitWrappedTextType-int-}
```
public void setAutoFitWrappedTextType(int value)
```


Ställer in typen av automatisk anpassning av radbrutet text.

Se [AutoFitWrappedTextType](../../com.aspose.cells/autofitwrappedtexttype).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setDefaultEditLanguage(int value) {#setDefaultEditLanguage-int-}
```
public void setDefaultEditLanguage(int value)
```


Ställer in standardspråk för redigering.

Se [DefaultEditLanguage](../../com.aspose.cells/defaulteditlanguage).

**Remarks**

Det kan visa/rendera olika layouter för textparagraf när olika redigeringsspråk är inställda. Standard är [DefaultEditLanguage.AUTO](../../com.aspose.cells/defaulteditlanguage\#AUTO).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setForRendering(boolean value) {#setForRendering-boolean-}
```
public void setForRendering(boolean value)
```


Anger om anpassning för renderingsändamål.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setFormatStrategy(int value) {#setFormatStrategy-int-}
```
public void setFormatStrategy(int value)
```


Ställer in den formaterade strategin.

Se [CellValueFormatStrategy](../../com.aspose.cells/cellvalueformatstrategy).

**Remarks**

Standardvärdet är CellStyle för prestanda.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setIgnoreHidden(boolean value) {#setIgnoreHidden-boolean-}
```
public void setIgnoreHidden(boolean value)
```


Ignorerar dolda rader/kolumner.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setMaxRowHeight(double value) {#setMaxRowHeight-double-}
```
public void setMaxRowHeight(double value)
```


Ställer in den maximala radhöjden (i enheten Punkt) när rader automatiskt anpassas.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | double |  |

### setOnlyAuto(boolean value) {#setOnlyAuto-boolean-}
```
public void setOnlyAuto(boolean value)
```


Anger om endast rader vars höjd inte är anpassad ska anpassas.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

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

