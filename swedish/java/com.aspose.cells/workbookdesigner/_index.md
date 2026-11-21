---
title: "WorkbookDesigner"
second_title: "Aspose.Cells för Java API-referens"
description: "Inkapslar objektet som representerar ett designark."
type: docs
url: /sv/java/com.aspose.cells/workbookdesigner/
---

**Inheritance:**
java.lang.Object
```
public class WorkbookDesigner
```

Inkapslar objektet som representerar ett designark.

**Example**

```
         //Create WorkbookDesigner object.
         WorkbookDesigner wd = new WorkbookDesigner();
         //Open the template file (which contains smart markers).
         wd.setWorkbook(new Workbook("SmartMarker_Designer.xls"));
 
         //Initialize your data from data source
         //DataSet ds = new DataSet();
 
 
         //Set the datatable as the data source.
         //wd.SetDataSource(dt);
         //Process the smart markers to fill the data into the worksheets.
         wd.process(true);
         //Save the excel file.
         wd.getWorkbook().save("outSmartMarker_Designer.xls");
```
## Konstruktörer

| Konstruktör | Beskrivning |
| --- | --- |
| [WorkbookDesigner()](#WorkbookDesigner--) | Initierar en ny instans av klassen [WorkbookDesigner](../../com.aspose.cells/workbookdesigner). |
| [WorkbookDesigner(Workbook workbook)](#WorkbookDesigner-com.aspose.cells.Workbook-) | Initierar en ny instans av klassen [WorkbookDesigner](../../com.aspose.cells/workbookdesigner). |
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [clearDataSource()](#clearDataSource--) | Rensar alla datakällor. |
| [containsVariables()](#containsVariables--) | Anger om det första kalkylbladet innehåller anpassade variabler. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getCalculateFormula()](#getCalculateFormula--) | Anger om formler ska beräknas. |
| [getCallBack()](#getCallBack--) | Hämtar återuppringningsgränssnitt för bearbetning av smartmarker. |
| [getClass()](#getClass--) |  |
| [getEnableHeaderFooterMarkers()](#getEnableHeaderFooterMarkers--) | Anger om sidhuvud/sidfot innehåller smart markers och ska bearbetas tillsammans. |
| [getLineByLine()](#getLineByLine--) | Anger om smart marker bearbetas rad för rad. |
| [getRepeatFormulasWithSubtotal()](#getRepeatFormulasWithSubtotal--) | Anger om formler ska upprepas med subtotalrad. |
| [getSmartMarkers()](#getSmartMarkers--) | Returnerar en samling av smart markers i ett kalkylblad. |
| [getSortDataSource()](#getSortDataSource--) | Anger om datakällan ska sorteras. |
| [getUpdateEmptyStringAsNull()](#getUpdateEmptyStringAsNull--) | Om TRUE, Null kommer att infogas om värdet är ""; |
| [getUpdateReference()](#getUpdateReference--) | Indikerar om referenser i andra arbetsblad kommer att uppdateras. |
| [getVariablesWorksheetName()](#getVariablesWorksheetName--) | Hämtar namnet på kalkylbladet som innehåller variabler smart marker. |
| [getWorkbook()](#getWorkbook--) | Hämtar objektet [getWorkbook()](../../com.aspose.cells/workbookdesigner\#getWorkbook--). |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [process()](#process--) | Bearbetar smart markers och fyller i värdena för datakällan. |
| [process(boolean isPreserved)](#process-boolean-) | Bearbetar smart markers och fyller i värdena för datakällan. |
| [process(Range range, boolean isPreserved)](#process-com.aspose.cells.Range-boolean-) | Bearbetar smart markers och fyller i värdena för datakällan. |
| [process(int sheetIndex, boolean isPreserved)](#process-int-boolean-) | Bearbetar smart markers och fyller i värdena för datakällan. |
| [setCalculateFormula(boolean value)](#setCalculateFormula-boolean-) | Anger om formler ska beräknas. |
| [setCallBack(ISmartMarkerCallBack value)](#setCallBack-com.aspose.cells.ISmartMarkerCallBack-) | Ställer in återuppringningsgränssnittet för bearbetning av smartmarker. |
| [setContainsVariables(boolean value)](#setContainsVariables-boolean-) | Anger om det första kalkylbladet innehåller anpassade variabler. |
| [setDataSource(String dataSource, ICellsDataTable cellsDataTable)](#setDataSource-java.lang.String-com.aspose.cells.ICellsDataTable-) | Ställer in datakällan för ett [ICellsDataTable](../../com.aspose.cells/icellsdatatable)-objekt. |
| [setDataSource(String variable, Object data)](#setDataSource-java.lang.String-java.lang.Object-) | Ställer in databindning till en variabel. |
| [setDataSource(String dataSource, ResultSet rs)](#setDataSource-java.lang.String-java.sql.ResultSet-) | Ställ in datakällan. |
| [setDataSource(String dataSource, ResultSet rs, int rowCount)](#setDataSource-java.lang.String-java.sql.ResultSet-int-) | Ställ in datakällan. |
| [setDataSource(ResultSet rs)](#setDataSource-java.sql.ResultSet-) | Ställ in datakällan. |
| [setEnableHeaderFooterMarkers(boolean value)](#setEnableHeaderFooterMarkers-boolean-) | Anger om sidhuvud/sidfot innehåller smart markers och ska bearbetas tillsammans. |
| [setJsonDataSource(String name, String json)](#setJsonDataSource-java.lang.String-java.lang.String-) | Ställ in JSON-strängvärdet som datakälla för smarta markörer. |
| [setLineByLine(boolean value)](#setLineByLine-boolean-) | Anger om smart marker bearbetas rad för rad. |
| [setRepeatFormulasWithSubtotal(boolean value)](#setRepeatFormulasWithSubtotal-boolean-) | Anger om formler ska upprepas med subtotalrad. |
| [setSortDataSource(boolean value)](#setSortDataSource-boolean-) | Anger om datakällan ska sorteras. |
| [setUpdateEmptyStringAsNull(boolean value)](#setUpdateEmptyStringAsNull-boolean-) | Om TRUE, Null kommer att infogas om värdet är ""; |
| [setUpdateReference(boolean value)](#setUpdateReference-boolean-) | Indikerar om referenser i andra arbetsblad kommer att uppdateras. |
| [setVariablesWorksheetName(String value)](#setVariablesWorksheetName-java.lang.String-) | Ställer in namnet på kalkylbladet som innehåller variabler för smart marker. |
| [setWorkbook(Workbook value)](#setWorkbook-com.aspose.cells.Workbook-) | Ställer in [getWorkbook()](../../com.aspose.cells/workbookdesigner\#getWorkbook--)-objektet. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### WorkbookDesigner() {#WorkbookDesigner--}
```
public WorkbookDesigner()
```


Initierar en ny instans av klassen [WorkbookDesigner](../../com.aspose.cells/workbookdesigner).

### WorkbookDesigner(Workbook workbook) {#WorkbookDesigner-com.aspose.cells.Workbook-}
```
public WorkbookDesigner(Workbook workbook)
```


Initierar en ny instans av klassen [WorkbookDesigner](../../com.aspose.cells/workbookdesigner).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| workbook | [Workbook](../../com.aspose.cells/workbook) | Mall-arbetsboksfilen. |

### clearDataSource() {#clearDataSource--}
```
public void clearDataSource()
```


Rensar alla datakällor.

### containsVariables() {#containsVariables--}
```
public boolean containsVariables()
```


Anger om det första kalkylbladet innehåller anpassade variabler.

**Remarks**

OBS: Detta medlem är nu föråldrat. Använd istället WorkbookDesigner.VariablesWorksheetName-egenskapen. Denna egenskap kommer att tas bort 3 månader senare, från och med september 2025. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Returns:**
boolean
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
### getCalculateFormula() {#getCalculateFormula--}
```
public boolean getCalculateFormula()
```


Anger om formler ska beräknas.

**Returns:**
boolean
### getCallBack() {#getCallBack--}
```
public ISmartMarkerCallBack getCallBack()
```


Hämtar återuppringningsgränssnitt för bearbetning av smartmarker.

**Returns:**
[ISmartMarkerCallBack](../../com.aspose.cells/ismartmarkercallback)
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getEnableHeaderFooterMarkers() {#getEnableHeaderFooterMarkers--}
```
public boolean getEnableHeaderFooterMarkers()
```


Anger om sidhuvud/sidfot innehåller smart markers och ska bearbetas tillsammans.

**Returns:**
boolean
### getLineByLine() {#getLineByLine--}
```
public boolean getLineByLine()
```


Anger om smart marker bearbetas rad för rad.

**Remarks**

OBS: Denna klass är nu föråldrad. Använd istället range smart markers. Denna egenskap kommer att tas bort 12 månader senare, från och med juli 2025. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Returns:**
boolean
### getRepeatFormulasWithSubtotal() {#getRepeatFormulasWithSubtotal--}
```
public boolean getRepeatFormulasWithSubtotal()
```


Anger om formler ska upprepas med subtotalrad.

**Returns:**
boolean
### getSmartMarkers() {#getSmartMarkers--}
```
public String[] getSmartMarkers()
```


Returnerar en samling av smart markers i ett kalkylblad.

**Remarks**

En strängarray skapas vid varje anrop. Arrayen sorteras och duplicerade värden tas bort.

**Returns:**
java.lang.String[] - En samling av smarta markörer
### getSortDataSource() {#getSortDataSource--}
```
public boolean getSortDataSource()
```


Anger om datakällan ska sorteras.

**Remarks**

OBS: Denna egenskap är nu föråldrad. Denna egenskap kommer att tas bort 12 månader senare, från och med oktober 2026. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt. JSON-datakälla sorteras om smart marker innehåller stigande och fallande parametrar.

**Returns:**
boolean
### getUpdateEmptyStringAsNull() {#getUpdateEmptyStringAsNull--}
```
public boolean getUpdateEmptyStringAsNull()
```


Om TRUE, Null kommer att infogas om värdet är "";

**Returns:**
boolean
### getUpdateReference() {#getUpdateReference--}
```
public boolean getUpdateReference()
```


Indikerar om referenser i andra arbetsblad kommer att uppdateras.

**Returns:**
boolean
### getVariablesWorksheetName() {#getVariablesWorksheetName--}
```
public String getVariablesWorksheetName()
```


Hämtar namnet på kalkylbladet som innehåller variabler smart marker.

**Returns:**
java.lang.String
### getWorkbook() {#getWorkbook--}
```
public Workbook getWorkbook()
```


Hämtar objektet [getWorkbook()](../../com.aspose.cells/workbookdesigner\#getWorkbook--).

**Returns:**
[Workbook](../../com.aspose.cells/workbook)
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




### process() {#process--}
```
public void process()
```


Bearbetar smart markers och fyller i värdena för datakällan.

### process(boolean isPreserved) {#process-boolean-}
```
public void process(boolean isPreserved)
```


Bearbetar smart markers och fyller i värdena för datakällan.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| isPreserved | boolean | Sant om den oigenkända smarta markören bevaras. |

### process(Range range, boolean isPreserved) {#process-com.aspose.cells.Range-boolean-}
```
public void process(Range range, boolean isPreserved)
```


Bearbetar smart markers och fyller i värdena för datakällan.

**Remarks**

OBS: Denna klass är nu föråldrad. Använd istället Range smart markers. Denna egenskap kommer att tas bort 12 månader senare, från och med juli 2025. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| range | [Range](../../com.aspose.cells/range) | Det område som ska bearbetas |
| isPreserved | boolean | Sant om den oigenkända smarta markören bevaras. |

### process(int sheetIndex, boolean isPreserved) {#process-int-boolean-}
```
public void process(int sheetIndex, boolean isPreserved)
```


Bearbetar smart markers och fyller i värdena för datakällan.

**Remarks**

Denna metod fungerar på kalkylbladsnivå.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| sheetIndex | int | Kalkylbladsindex. |
| isPreserved | boolean | Sant om den oigenkända smarta markören bevaras. |

### setCalculateFormula(boolean value) {#setCalculateFormula-boolean-}
```
public void setCalculateFormula(boolean value)
```


Anger om formler ska beräknas.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setCallBack(ISmartMarkerCallBack value) {#setCallBack-com.aspose.cells.ISmartMarkerCallBack-}
```
public void setCallBack(ISmartMarkerCallBack value)
```


Ställer in återuppringningsgränssnittet för bearbetning av smartmarker.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [ISmartMarkerCallBack](../../com.aspose.cells/ismartmarkercallback) |  |

### setContainsVariables(boolean value) {#setContainsVariables-boolean-}
```
public void setContainsVariables(boolean value)
```


Anger om det första kalkylbladet innehåller anpassade variabler.

**Remarks**

OBS: Detta medlem är nu föråldrat. Använd istället WorkbookDesigner.VariablesWorksheetName-egenskapen. Denna egenskap kommer att tas bort 3 månader senare, från och med september 2025. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setDataSource(String dataSource, ICellsDataTable cellsDataTable) {#setDataSource-java.lang.String-com.aspose.cells.ICellsDataTable-}
```
public void setDataSource(String dataSource, ICellsDataTable cellsDataTable)
```


Ställer in datakällan för ett [ICellsDataTable](../../com.aspose.cells/icellsdatatable)-objekt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| dataSource | java.lang.String | Namnet på datakällan. |
| cellsDataTable | [ICellsDataTable](../../com.aspose.cells/icellsdatatable) | datatabell. |

### setDataSource(String variable, Object data) {#setDataSource-java.lang.String-java.lang.Object-}
```
public void setDataSource(String variable, Object data)
```


Ställer in databindning till en variabel.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| variabel | java.lang.String | Variabelnamn skapat med smart marker. |
| data | java.lang.Object | Källdata. |

### setDataSource(String dataSource, ResultSet rs) {#setDataSource-java.lang.String-java.sql.ResultSet-}
```
public void setDataSource(String dataSource, ResultSet rs)
```


Ställ in datakällan.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| dataSource | java.lang.String | Namnet på datakällan. |
| rs | java.sql.ResultSet | Resultatmängden. |

### setDataSource(String dataSource, ResultSet rs, int rowCount) {#setDataSource-java.lang.String-java.sql.ResultSet-int-}
```
public void setDataSource(String dataSource, ResultSet rs, int rowCount)
```


Ställ in datakällan.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| dataSource | java.lang.String | Namnet på datakällan. |
| rs | java.sql.ResultSet | Resultatmängden. |
| rowCount | int | Datamängdens antal för det givna resultatsetet. Det bör vara det exakta radantalet eller -1; Om resultatsetet är endast framåtriktat bör användaren ange det exakta radantalet här, annars kan smarten kanske inte bearbetas korrekt när smartmarkörens "noadd" inte är inställd. |

### setDataSource(ResultSet rs) {#setDataSource-java.sql.ResultSet-}
```
public void setDataSource(ResultSet rs)
```


Ställ in datakällan.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| rs | java.sql.ResultSet | Resultatmängden. |

### setEnableHeaderFooterMarkers(boolean value) {#setEnableHeaderFooterMarkers-boolean-}
```
public void setEnableHeaderFooterMarkers(boolean value)
```


Anger om sidhuvud/sidfot innehåller smart markers och ska bearbetas tillsammans.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setJsonDataSource(String name, String json) {#setJsonDataSource-java.lang.String-java.lang.String-}
```
public void setJsonDataSource(String name, String json)
```


Ställ in JSON-strängvärdet som datakälla för smarta markörer.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| name | java.lang.String | Namnet på tabellen. Om värdet i JSON representerar ett objekt kan det vara null. |
| json | java.lang.String | Värdet på JSON-strängen. |

### setLineByLine(boolean value) {#setLineByLine-boolean-}
```
public void setLineByLine(boolean value)
```


Anger om smart marker bearbetas rad för rad.

**Remarks**

OBS: Denna klass är nu föråldrad. Använd istället range smart markers. Denna egenskap kommer att tas bort 12 månader senare, från och med juli 2025. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setRepeatFormulasWithSubtotal(boolean value) {#setRepeatFormulasWithSubtotal-boolean-}
```
public void setRepeatFormulasWithSubtotal(boolean value)
```


Anger om formler ska upprepas med subtotalrad.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setSortDataSource(boolean value) {#setSortDataSource-boolean-}
```
public void setSortDataSource(boolean value)
```


Anger om datakällan ska sorteras.

**Remarks**

OBS: Denna egenskap är nu föråldrad. Denna egenskap kommer att tas bort 12 månader senare, från och med oktober 2026. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt. JSON-datakälla sorteras om smart marker innehåller stigande och fallande parametrar.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setUpdateEmptyStringAsNull(boolean value) {#setUpdateEmptyStringAsNull-boolean-}
```
public void setUpdateEmptyStringAsNull(boolean value)
```


Om TRUE, Null kommer att infogas om värdet är "";

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setUpdateReference(boolean value) {#setUpdateReference-boolean-}
```
public void setUpdateReference(boolean value)
```


Indikerar om referenser i andra arbetsblad kommer att uppdateras.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setVariablesWorksheetName(String value) {#setVariablesWorksheetName-java.lang.String-}
```
public void setVariablesWorksheetName(String value)
```


Ställer in namnet på kalkylbladet som innehåller variabler för smart marker.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setWorkbook(Workbook value) {#setWorkbook-com.aspose.cells.Workbook-}
```
public void setWorkbook(Workbook value)
```


Ställer in [getWorkbook()](../../com.aspose.cells/workbookdesigner\#getWorkbook--)-objektet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [Workbook](../../com.aspose.cells/workbook) |  |

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

