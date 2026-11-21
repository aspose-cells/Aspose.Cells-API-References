---
title: "PivotTableCollection"
second_title: "Aspose.Cells för Java API-referens"
description: "Representerar samlingen av alla PivotTable‑objekt på det angivna kalkylbladet."
type: docs
url: /sv/java/com.aspose.cells/pivottablecollection/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.CollectionBase](../../com.aspose.cells/collectionbase)
```
public class PivotTableCollection extends CollectionBase
```

Representerar samlingen av alla PivotTable‑objekt på det angivna kalkylbladet.

**Example**

```
         Workbook book = new Workbook();
         Worksheet sheet = book.getWorksheets().get(0);
         Cells cells = sheet.getCells();
         cells.get(0, 0).setValue("fruit");
         cells.get(1, 0).setValue("grape");
         cells.get(2, 0).setValue("blueberry");
         cells.get(3, 0).setValue("kiwi");
         cells.get(4, 0).setValue("cherry");
         cells.get(5, 0).setValue("grape");
         cells.get(6, 0).setValue("blueberry");
         cells.get(7, 0).setValue("kiwi");
         cells.get(8, 0).setValue("cherry");
 
         cells.get(0, 1).setValue("year");
         cells.get(1, 1).setValue(2020);
         cells.get(2, 1).setValue(2020);
         cells.get(3, 1).setValue(2020);
         cells.get(4, 1).setValue(2020);
         cells.get(5, 1).setValue(2021);
         cells.get(6, 1).setValue(2021);
         cells.get(7, 1).setValue(2021);
         cells.get(8, 1).setValue(2021);
 
         cells.get(0, 2).setValue("amount");
         cells.get(1, 2).setValue(50);
         cells.get(2, 2).setValue(60);
         cells.get(3, 2).setValue(70);
         cells.get(4, 2).setValue(80);
         cells.get(5, 2).setValue(90);
         cells.get(6, 2).setValue(100);
         cells.get(7, 2).setValue(110);
         cells.get(8, 2).setValue(120);
 
         PivotTableCollection pivots = sheet.getPivotTables();
 
         PivotTable pivot = pivots.add("=Sheet1!A1:C9", "A12");
 
         pivot.addFieldToArea(PivotFieldType.ROW, "fruit");
         pivot.addFieldToArea(PivotFieldType.COLUMN, "year");
         pivot.addFieldToArea(PivotFieldType.DATA, "amount");
 
         pivot.setPivotTableStyleType(PivotTableStyleType.PIVOT_TABLE_STYLE_MEDIUM_10);
 
         //Change PivotField's attributes
         PivotField rowField = pivot.getRowFields().get(0);
         rowField.setDisplayName("custom display name");
 
         //Add PivotFilter
         PivotFilter filter = pivot.getRowFields().get(0).filterTop10(0, PivotFilterType.PERCENT, false, 2);
 
 
         //Add PivotFormatCondition
         int formatIndex = pivot.getConditionalFormats().add();
         PivotConditionalFormat pfc = pivot.getConditionalFormats().get(formatIndex);
         pfc.addCellArea(pivot.getDataBodyRange());
         FormatConditionCollection fcc = pfc.getFormatConditions();
         int ii = fcc.addCondition(FormatConditionType.CELL_VALUE, OperatorType.GREATER_OR_EQUAL, "100", null);
 
         FormatCondition fc = fcc.get(ii);
 
         fc.getStyle().setBackgroundColor(Color.getRed());
 
         pivot.calculateData();
 
         //do your business
 
         book.save("out.xlsx");
```
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [add(PivotTable pivotTable, int row, int column, String tableName)](#add-com.aspose.cells.PivotTable-int-int-java.lang.String-) | Lägger till en ny pivottabell baserad på en annan pivottabell. |
| [add(PivotTable pivotTable, String destCellName, String tableName)](#add-com.aspose.cells.PivotTable-java.lang.String-java.lang.String-) | Lägger till en ny pivottabell baserad på en annan pivottabell. |
| [add(Object o)](#add-java.lang.Object-) | Lägger till ett objekt i CollectionBase-instansen. |
| [add(String sourceData, int row, int column)](#add-java.lang.String-int-int-) | Lägger till en ny modern pivottabell (sedan Excel 2007) på den angivna arbetsbladets rad- och kolumnposition med standardalternativ. |
| [add(String sourceData, int row, int column, PivotTableCreateOptions options)](#add-java.lang.String-int-int-com.aspose.cells.PivotTableCreateOptions-) | Lägger till en ny pivottabell på den angivna arbetsbladets rad- och kolumnposition. |
| [add(String sourceData, int row, int column, String tableName)](#add-java.lang.String-int-int-java.lang.String-) | Lägger till en ny pivottabell med äldre Excel 97-2003 layout och stil. |
| [add(String sourceData, int row, int column, String tableName, boolean useSameSource)](#add-java.lang.String-int-int-java.lang.String-boolean-) | Lägger till en ny pivottabell med äldre Excel 97-2003 layout och stil. |
| [add(String sourceData, int row, int column, String tableName, boolean useSameSource, boolean isXlsClassic)](#add-java.lang.String-int-int-java.lang.String-boolean-boolean-) | Lägger till en ny pivottabell med äldre Excel 97-2003 layout och stil. |
| [add(String sourceData, String cellName)](#add-java.lang.String-java.lang.String-) | Lägger till en ny modern pivottabell (sedan Excel 2007) på den angivna arbetsbladets rad- och kolumnposition med standardalternativ. |
| [add(String sourceData, String cellName, PivotTableCreateOptions options)](#add-java.lang.String-java.lang.String-com.aspose.cells.PivotTableCreateOptions-) | Lägger till en ny modern pivottabell (sedan Excel 2007) på den angivna arbetsbladets rad- och kolumnposition med standardalternativ. |
| [add(String sourceData, String destCellName, String tableName)](#add-java.lang.String-java.lang.String-java.lang.String-) | Lägger till en ny pivottabell med äldre Excel 97-2003 layout och stil. |
| [add(String sourceData, String destCellName, String tableName, boolean useSameSource)](#add-java.lang.String-java.lang.String-java.lang.String-boolean-) | Lägger till en ny pivottabell med äldre Excel 97-2003 layout och stil. |
| [add(String sourceData, String cell, String tableName, boolean useSameSource, boolean isXlsClassic)](#add-java.lang.String-java.lang.String-java.lang.String-boolean-boolean-) | Lägger till en ny pivottabell. |
| [add(String[] sourceData, boolean isAutoPage, PivotPageFields pageFields, int row, int column, String tableName)](#add-java.lang.String---boolean-com.aspose.cells.PivotPageFields-int-int-java.lang.String-) | Lägger till ett nytt pivottabellobjekt i samlingen med flera konsolideringsområden som datakälla. |
| [add(String[] sourceData, boolean isAutoPage, PivotPageFields pageFields, String destCellName, String tableName)](#add-java.lang.String---boolean-com.aspose.cells.PivotPageFields-java.lang.String-java.lang.String-) | Lägger till ett nytt pivottabellobjekt i samlingen med flera konsolideringsområden som datakälla. |
| [clear()](#clear--) | Rensar alla pivottabeller. |
| [contains(Object o)](#contains-java.lang.Object-) | Returnerar om instansen innehåller detta objekt |
| [dispose()](#dispose--) | Utför applikationsdefinierade uppgifter som är relaterade till att frigöra, släppa eller återställa ohanterade resurser. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | Hämtar pivottabellsrapporten efter index. |
| [get(int row, int column)](#get-int-int-) | Hämtar den [PivotTable](../../com.aspose.cells/pivottable) som finns i cellen. |
| [get(String name)](#get-java.lang.String-) | Hämtar PivotTable-rapporten efter pivottabellens namn. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | Hämtar antalet element som finns i CollectionBase-instansen. |
| [hashCode()](#hashCode--) |  |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | Bestämmer indexet för ett specifikt objekt i CollectionBase-instansen. |
| [iterator()](#iterator--) | Returnerar en enumerator som itererar genom CollectionBase-instansen. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [remove(PivotTable pivotTable)](#remove-com.aspose.cells.PivotTable-) | Tar bort den angivna PivotTable och raderar PivotTable-data. |
| [remove(PivotTable pivotTable, boolean keepData)](#remove-com.aspose.cells.PivotTable-boolean-) | Tar bort den angivna PivotTable. |
| [removeAt(int index)](#removeAt-int-) | Tar bort PivotTable på det angivna indexet och raderar PivotTable-data. |
| [removeAt(int index, boolean keepData)](#removeAt-int-boolean-) | Tar bort PivotTable på det angivna indexet. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### add(PivotTable pivotTable, int row, int column, String tableName) {#add-com.aspose.cells.PivotTable-int-int-java.lang.String-}
```
public int add(PivotTable pivotTable, int row, int column, String tableName)
```


Lägger till en ny pivottabell baserad på en annan pivottabell.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| pivotTable | [PivotTable](../../com.aspose.cells/pivottable) | Käll‑PivotTable. |
| rad | int | Radindex för cellen i det övre vänstra hörnet av PivotTable‑rapportens destinationsområde. |
| kolumn | int | Kolumnindex för cellen i det övre vänstra hörnet av PivotTable‑rapportens destinationsområde. |
| tableName | java.lang.String | Namnet på den nya PivotTable‑rapporten. |

**Returns:**
int – Det nyss tillagda PivotTable‑indexet.
### add(PivotTable pivotTable, String destCellName, String tableName) {#add-com.aspose.cells.PivotTable-java.lang.String-java.lang.String-}
```
public int add(PivotTable pivotTable, String destCellName, String tableName)
```


Lägger till en ny pivottabell baserad på en annan pivottabell.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| pivotTable | [PivotTable](../../com.aspose.cells/pivottable) | Käll‑PivotTable. |
| destCellName | java.lang.String | Cellen i det övre vänstra hörnet av PivotTable‑rapportens destinationsområde. |
| tableName | java.lang.String | Namnet på den nya PivotTable‑rapporten. |

**Returns:**
int – Det nyss tillagda PivotTable‑indexet.
### add(Object o) {#add-java.lang.Object-}
```
public int add(Object o)
```


Lägger till ett objekt i CollectionBase-instansen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| o | java.lang.Object | Objektet som ska läggas till i CollectionBase-instansen. |

**Returns:**
int - Positionen där det nya elementet infördes.
### add(String sourceData, int row, int column) {#add-java.lang.String-int-int-}
```
public PivotTable add(String sourceData, int row, int column)
```


Lägger till en ny modern pivottabell (sedan Excel 2007) på den angivna arbetsbladets rad- och kolumnposition med standardalternativ.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| sourceData | java.lang.String | Data‑cellområdet för den nya PivotTable. Exempel: Sheet1!A1:C8 |
| rad | int | Nollbaserat radindex för det övre vänstra hörnet av PivotTable‑destinationen. |
| kolumn | int | Nollbaserat kolumnindex för det övre vänstra hörnet av PivotTable‑destinationen. |

**Returns:**
[PivotTable](../../com.aspose.cells/pivottable) - The newly created PivotTable instance.
### add(String sourceData, int row, int column, PivotTableCreateOptions options) {#add-java.lang.String-int-int-com.aspose.cells.PivotTableCreateOptions-}
```
public PivotTable add(String sourceData, int row, int column, PivotTableCreateOptions options)
```


Lägger till en ny pivottabell på den angivna arbetsbladets rad- och kolumnposition.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| sourceData | java.lang.String | Data‑cellområdet för den nya PivotTable. Exempel: Sheet1!A1:C8 |
| rad | int | Nollbaserat radindex för det övre vänstra hörnet av PivotTable‑destinationen. |
| kolumn | int | Nollbaserat kolumnindex för det övre vänstra hörnet av PivotTable‑destinationen. |
| options | [PivotTableCreateOptions](../../com.aspose.cells/pivottablecreateoptions) | Alternativ för skapande av PivotTable. |

**Returns:**
[PivotTable](../../com.aspose.cells/pivottable) - The newly created PivotTable instance.
### add(String sourceData, int row, int column, String tableName) {#add-java.lang.String-int-int-java.lang.String-}
```
public int add(String sourceData, int row, int column, String tableName)
```


Lägger till en ny pivottabell med äldre Excel 97-2003 layout och stil.

**Remarks**

OBS: Denna metod är föråldrad. Den är ekvivalent med att anropa PivotTableCollection.Add(string, int, int, PivotTableCreateOptions) med `NewPivotTableOptions.IsXlsClassic = true`. Använd istället PivotTableCollection.Add(string, int, int, PivotTableCreateOptions)-överladdning. Denna metod kommer att tas bort 12 månader efter september 2026. Vi ber om ursäkt för eventuella besvär.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| sourceData | java.lang.String | Data‑cellområdet för den nya PivotTable. Exempel: Sheet1!A1:C8 |
| rad | int | Radindex för cellen i det övre vänstra hörnet av PivotTable‑rapportens destinationsområde. |
| kolumn | int | Kolumnindex för cellen i det övre vänstra hörnet av PivotTable‑rapportens destinationsområde. |
| tableName | java.lang.String | Namnet på den nya PivotTable‑rapporten. |

**Returns:**
int – Indexet i den här PivotTable‑listan.
### add(String sourceData, int row, int column, String tableName, boolean useSameSource) {#add-java.lang.String-int-int-java.lang.String-boolean-}
```
public int add(String sourceData, int row, int column, String tableName, boolean useSameSource)
```


Lägger till en ny pivottabell med äldre Excel 97-2003 layout och stil.

**Remarks**

OBS: Denna metod är föråldrad. Den är ekvivalent med att anropa PivotTableCollection.Add(string, int, int, PivotTableCreateOptions) med `NewPivotTableOptions.IsXlsClassic = true`. Använd istället PivotTableCollection.Add(string, int, int, PivotTableCreateOptions)-överladdning. Denna metod kommer att tas bort 12 månader efter september 2026. Vi ber om ursäkt för eventuella besvär.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| sourceData | java.lang.String | Data‑cellområdet för den nya PivotTable. Exempel: Sheet1!A1:C8 |
| rad | int | Radindex för cellen i det övre vänstra hörnet av PivotTable‑rapportens destinationsområde. |
| kolumn | int | Kolumnindex för cellen i det övre vänstra hörnet av PivotTable‑rapportens destinationsområde. |
| tableName | java.lang.String | Namnet på den nya PivotTable‑rapporten. |
| useSameSource | boolean | Anger om samma datakälla ska användas när en annan befintlig pivottabell har använt denna datakälla. Om egenskapen är sann sparas minne. |

**Returns:**
int – Det nyss tillagda cache‑indexet.
### add(String sourceData, int row, int column, String tableName, boolean useSameSource, boolean isXlsClassic) {#add-java.lang.String-int-int-java.lang.String-boolean-boolean-}
```
public int add(String sourceData, int row, int column, String tableName, boolean useSameSource, boolean isXlsClassic)
```


Lägger till en ny pivottabell med äldre Excel 97-2003 layout och stil.

**Remarks**

OBS: Denna metod är föråldrad. Den är ekvivalent med att anropa PivotTableCollection.Add(string, int, int, PivotTableCreateOptions) med `NewPivotTableOptions.IsXlsClassic = true`. Använd istället PivotTableCollection.Add(string, int, int, PivotTableCreateOptions)-överladdning. Denna metod kommer att tas bort 12 månader efter oktober 2026. Vi ber om ursäkt för eventuella besvär.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| sourceData | java.lang.String | Data‑cellområdet för den nya PivotTable. Exempel: Sheet1!A1:C8 |
| rad | int | Radindex för cellen i det övre vänstra hörnet av PivotTable‑rapportens destinationsområde. |
| kolumn | int | Kolumnindex för cellen i det övre vänstra hörnet av PivotTable‑rapportens destinationsområde. |
| tableName | java.lang.String | Namnet på den nya PivotTable‑rapporten. |
| useSameSource | boolean | Anger om samma datakälla ska användas när en annan befintlig pivottabell har använt denna datakälla. Om egenskapen är sann sparas minne. |
| isXlsClassic | boolean | Anger om en klassisk pivottabell för Excel 97-2003 ska läggas till. |

**Returns:**
int – Det nyss tillagda cache‑indexet.
### add(String sourceData, String cellName) {#add-java.lang.String-java.lang.String-}
```
public PivotTable add(String sourceData, String cellName)
```


Lägger till en ny modern pivottabell (sedan Excel 2007) på den angivna arbetsbladets rad- och kolumnposition med standardalternativ.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| sourceData | java.lang.String | Data‑cellområdet för den nya PivotTable. Exempel: Sheet1!A1:C8 |
| cellNamn | java.lang.String | Namnet på cellen i övre vänstra hörnet för pivottabellens destination. |

**Returns:**
[PivotTable](../../com.aspose.cells/pivottable) - The newly created PivotTable instance.
### add(String sourceData, String cellName, PivotTableCreateOptions options) {#add-java.lang.String-java.lang.String-com.aspose.cells.PivotTableCreateOptions-}
```
public PivotTable add(String sourceData, String cellName, PivotTableCreateOptions options)
```


Lägger till en ny modern pivottabell (sedan Excel 2007) på den angivna arbetsbladets rad- och kolumnposition med standardalternativ.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| sourceData | java.lang.String | Data‑cellområdet för den nya PivotTable. Exempel: Sheet1!A1:C8 |
| cellNamn | java.lang.String | Namnet på cellen i övre vänstra hörnet för pivottabellens destination. |
| options | [PivotTableCreateOptions](../../com.aspose.cells/pivottablecreateoptions) | Alternativen för att skapa pivottabell. |

**Returns:**
[PivotTable](../../com.aspose.cells/pivottable) - The newly created PivotTable instance.
### add(String sourceData, String destCellName, String tableName) {#add-java.lang.String-java.lang.String-java.lang.String-}
```
public int add(String sourceData, String destCellName, String tableName)
```


Lägger till en ny pivottabell med äldre Excel 97-2003 layout och stil.

**Remarks**

OBS: Denna metod är föråldrad. Den är ekvivalent med att anropa PivotTableCollection.Add(string, int, int, PivotTableCreateOptions) med `NewPivotTableOptions.IsXlsClassic = true`. Använd istället PivotTableCollection.Add(string, int, int, PivotTableCreateOptions)-överladdning. Denna metod kommer att tas bort 12 månader efter september 2026. Vi ber om ursäkt för eventuella besvär.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| sourceData | java.lang.String | Data för den nya pivottabellcachen. |
| destCellName | java.lang.String | Cellen i det övre vänstra hörnet av PivotTable‑rapportens destinationsområde. |
| tableName | java.lang.String | Namnet på den nya PivotTable‑rapporten. |

**Returns:**
int – Indexet i den här PivotTable‑listan.
### add(String sourceData, String destCellName, String tableName, boolean useSameSource) {#add-java.lang.String-java.lang.String-java.lang.String-boolean-}
```
public int add(String sourceData, String destCellName, String tableName, boolean useSameSource)
```


Lägger till en ny pivottabell med äldre Excel 97-2003 layout och stil.

**Remarks**

OBS: Denna metod är föråldrad. Den är ekvivalent med att anropa PivotTableCollection.Add(string, int, int, PivotTableCreateOptions) med `NewPivotTableOptions.IsXlsClassic = true`. Använd istället PivotTableCollection.Add(string, int, int, PivotTableCreateOptions)-överladdning. Denna metod kommer att tas bort 12 månader efter september 2026. Vi ber om ursäkt för eventuella besvär.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| sourceData | java.lang.String | Data för den nya pivottabellcachen. |
| destCellName | java.lang.String | Cellen i det övre vänstra hörnet av PivotTable‑rapportens destinationsområde. |
| tableName | java.lang.String | Namnet på den nya PivotTable‑rapporten. |
| useSameSource | boolean | Anger om samma datakälla ska användas när en annan befintlig pivottabell har använt denna datakälla. Om egenskapen är sann sparas minne. |

**Returns:**
int – Det nyss tillagda cache‑indexet.
### add(String sourceData, String cell, String tableName, boolean useSameSource, boolean isXlsClassic) {#add-java.lang.String-java.lang.String-java.lang.String-boolean-boolean-}
```
public int add(String sourceData, String cell, String tableName, boolean useSameSource, boolean isXlsClassic)
```


Lägger till en ny pivottabell.

**Remarks**

OBS: Denna metod är föråldrad. Den är ekvivalent med att anropa PivotTableCollection.Add(string, int, int, PivotTableCreateOptions) med `NewPivotTableOptions.IsXlsClassic = true`. Använd istället PivotTableCollection.Add(string, int, int, PivotTableCreateOptions)-överladdning. Denna metod kommer att tas bort 12 månader efter oktober 2026. Vi ber om ursäkt för eventuella besvär.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| sourceData | java.lang.String | Data‑cellområdet för den nya PivotTable. Exempel: Sheet1!A1:C8 |
| cell | java.lang.String | Cellen i det övre vänstra hörnet av PivotTable‑rapportens destinationsområde. |
| tableName | java.lang.String | Namnet på den nya PivotTable‑rapporten. |
| useSameSource | boolean | Anger om samma datakälla ska användas när en annan befintlig pivottabell har använt denna datakälla. Om egenskapen är sann sparas minne när samma datakälla har samlats i en pivottabellcache. |
| isXlsClassic | boolean | Anger om en klassisk pivottabell för Excel 97-2003 ska läggas till. |

**Returns:**
int – Det nyss tillagda cache‑indexet.
### add(String[] sourceData, boolean isAutoPage, PivotPageFields pageFields, int row, int column, String tableName) {#add-java.lang.String---boolean-com.aspose.cells.PivotPageFields-int-int-java.lang.String-}
```
public int add(String[] sourceData, boolean isAutoPage, PivotPageFields pageFields, int row, int column, String tableName)
```


Lägger till ett nytt pivottabellobjekt i samlingen med flera konsolideringsområden som datakälla.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| sourceData | java.lang.String[] | De flera konsolideringsområdena, till exempel \{"Sheet1!A1:C8","Sheet2!A1:B8"\} |
| isAutoPage | boolean | Om ett enskilt sidfält ska skapas automatiskt. Om sant kommer följande parameter pageFields att ignoreras. |
| pageFields | [PivotPageFields](../../com.aspose.cells/pivotpagefields) | Pivotsidfältets objekt. |
| rad | int | Radindex för cellen i det övre vänstra hörnet av PivotTable‑rapportens destinationsområde. |
| kolumn | int | Kolumnindex för cellen i det övre vänstra hörnet av PivotTable‑rapportens destinationsområde. |
| tableName | java.lang.String | Namnet på den nya PivotTable‑rapporten. |

**Returns:**
int – Det nyss tillagda PivotTable‑indexet.
### add(String[] sourceData, boolean isAutoPage, PivotPageFields pageFields, String destCellName, String tableName) {#add-java.lang.String---boolean-com.aspose.cells.PivotPageFields-java.lang.String-java.lang.String-}
```
public int add(String[] sourceData, boolean isAutoPage, PivotPageFields pageFields, String destCellName, String tableName)
```


Lägger till ett nytt pivottabellobjekt i samlingen med flera konsolideringsområden som datakälla.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| sourceData | java.lang.String[] | De flera konsolideringsområdena, till exempel \{"Sheet1!A1:C8","Sheet2!A1:B8"\} |
| isAutoPage | boolean | Om ett enskilt sidfält ska skapas automatiskt. Om sant kommer följande parameter pageFields att ignoreras. |
| pageFields | [PivotPageFields](../../com.aspose.cells/pivotpagefields) | Pivotsidfältets objekt. |
| destCellName | java.lang.String | destCellName Namnet på den nya pivottabellrapporten. |
| tableName | java.lang.String | namnet på den nya pivottabellrapporten. |

**Returns:**
int – Det nyss tillagda PivotTable‑indexet.
### clear() {#clear--}
```
public void clear()
```


Rensar alla pivottabeller.

### contains(Object o) {#contains-java.lang.Object-}
```
public boolean contains(Object o)
```


Returnerar om instansen innehåller detta objekt

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| o | java.lang.Object | testobjekt |

**Returns:**
boolean - Om instansen innehåller detta objekt
### dispose() {#dispose--}
```
public void dispose()
```


Utför applikationsdefinierade uppgifter som är relaterade till att frigöra, släppa eller återställa ohanterade resurser.

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
### get(int index) {#get-int-}
```
public PivotTable get(int index)
```


Hämtar pivottabellsrapporten efter index.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| index | int |  |

**Returns:**
[PivotTable](../../com.aspose.cells/pivottable)
### get(int row, int column) {#get-int-int-}
```
public PivotTable get(int row, int column)
```


Hämtar den [PivotTable](../../com.aspose.cells/pivottable) som finns i cellen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| rad | int |  |
| kolumn | int |  |

**Returns:**
[PivotTable](../../com.aspose.cells/pivottable)
### get(String name) {#get-java.lang.String-}
```
public PivotTable get(String name)
```


Hämtar PivotTable-rapporten efter pivottabellens namn.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| name | java.lang.String |  |

**Returns:**
[PivotTable](../../com.aspose.cells/pivottable)
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getCount() {#getCount--}
```
public int getCount()
```


Hämtar antalet element som finns i CollectionBase-instansen.

**Returns:**
int - Antalet element som finns i CollectionBase-instansen.
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### indexOf(Object o) {#indexOf-java.lang.Object-}
```
public int indexOf(Object o)
```


Bestämmer indexet för ett specifikt objekt i CollectionBase-instansen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| o | java.lang.Object | Bestämmer indexet för ett specifikt objekt i CollectionBase-instansen. |

**Returns:**
int - Indexet för värdet om det hittas i listan; annars -1.
### iterator() {#iterator--}
```
public Iterator iterator()
```


Returnerar en enumerator som itererar genom CollectionBase-instansen.

**Returns:**
java.util.Iterator - En iterator för CollectionBase-instansen.
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### remove(PivotTable pivotTable) {#remove-com.aspose.cells.PivotTable-}
```
public void remove(PivotTable pivotTable)
```


Tar bort den angivna PivotTable och raderar PivotTable-data.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| pivotTable | [PivotTable](../../com.aspose.cells/pivottable) | PivotTable-objekt |

### remove(PivotTable pivotTable, boolean keepData) {#remove-com.aspose.cells.PivotTable-boolean-}
```
public void remove(PivotTable pivotTable, boolean keepData)
```


Tar bort den angivna PivotTable.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| pivotTable | [PivotTable](../../com.aspose.cells/pivottable) | PivotTable-objekt |
| keepData | boolean | Om pivottabellens data ska behållas |

### removeAt(int index) {#removeAt-int-}
```
public void removeAt(int index)
```


Tar bort PivotTable på det angivna indexet och raderar PivotTable-data.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| index | int | positionsindexet i pivottabellsamlingen |

### removeAt(int index, boolean keepData) {#removeAt-int-boolean-}
```
public void removeAt(int index, boolean keepData)
```


Tar bort PivotTable på det angivna indexet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| index | int | positionsindexet i pivottabellsamlingen |
| keepData | boolean | Om pivottabellens data ska behållas |

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

