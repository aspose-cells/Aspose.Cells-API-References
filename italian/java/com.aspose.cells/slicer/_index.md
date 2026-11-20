---
title: "Slicer"
second_title: "Riferimento API di Aspose.Cells per Java"
description: "descrizione riepilogativa della Vista Slicer"
type: docs
url: /it/java/com.aspose.cells/slicer/
---

**Inheritance:**
java.lang.Object
```
public class Slicer
```

descrizione riepilogativa della Vista Slicer

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
 
         pivot.calculateData();
 
         SlicerCollection slicers = sheet.getSlicers();
         int slicerIndex = slicers.add(pivot, "E12", "fruit");
         Slicer slicer = slicers.get(slicerIndex);
         slicer.setStyleType(SlicerStyleType.SLICER_STYLE_LIGHT_2);
 
         slicer.unselectItems(new String[] { "grape" });
         //do your business
         book.save("out.xlsx");
```
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [addPivotConnection(PivotTable pivot)](#addPivotConnection-com.aspose.cells.PivotTable-) | Aggiunge la connessione alla tabella pivot. |
| [clearFilter()](#clearFilter--) | Rimuovi filtri |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAlternativeText()](#getAlternativeText--) | Restituisce o imposta la stringa di testo descrittiva (alternativa) dell'oggetto Slicer. |
| [getCaption()](#getCaption--) | Restituisce o imposta la didascalia dello slicer specificato. |
| [getCaptionVisible()](#getCaptionVisible--) | Restituisce o imposta se l'intestazione che visualizza la didascalia dello slicer è visibile. |
| [getClass()](#getClass--) |  |
| [getColumnWidth()](#getColumnWidth--) | Restituisce o imposta la larghezza di ogni colonna nello slicer in unità di punti. |
| [getColumnWidthPixel()](#getColumnWidthPixel--) | Restituisce la larghezza di\u807deach colonna in\u807dlo slicer, in unità di\u807dpixel.\u807d |
| [getFirstItemIndex()](#getFirstItemIndex--) | Specifica l'indice basato su zero del primo elemento dello slicer. |
| [getHeight()](#getHeight--) | Restituisce o imposta l'altezza dello slicer specificato, in punti. |
| [getHeightPixel()](#getHeightPixel--) | Restituisce o imposta l'altezza dello slicer specificato, in pixel. |
| [getLeftPixel()](#getLeftPixel--) | Restituisce o imposta lo spostamento orizzontale della forma dello slicer dalla sua colonna sinistra, in pixel. |
| [getLockedAspectRatio()](#getLockedAspectRatio--) | Indica se il blocco del rapporto d'aspetto è abilitato. |
| [getLockedPosition()](#getLockedPosition--) | Indica se lo slicer specificato può essere spostato o ridimensionato tramite l'interfaccia utente. |
| [getName()](#getName--) | Restituisce o imposta il nome dello slicer specificato |
| [getNumberOfColumns()](#getNumberOfColumns--) | Restituisce o imposta il numero di colonne nello slicer. |
| [getParent()](#getParent--) | Restituisce l'oggetto [getWorksheet()](../../com.aspose.cells/slicer\#getWorksheet--) che contiene questo slicer. |
| [getPlacement()](#getPlacement--) | Rappresenta il modo in cui l'oggetto di disegno è collegato alle celle sottostanti. |
| [getRowHeight()](#getRowHeight--) | Restituisce o imposta l'altezza di ogni riga nello slicer specificato in unità di punti. |
| [getRowHeightPixel()](#getRowHeightPixel--) | Restituisce o imposta l'altezza di ogni riga nello slicer specificato, in unità di pixel. |
| [getShape()](#getShape--) | Restituisce l'oggetto Shape associato allo slicer specificato. |
| [getShowAllItems()](#getShowAllItems--) | Indica se mostrare tutti gli elementi anche se non ci sono dati o sono stati eliminati. |
| [getShowCaption()](#getShowCaption--) | Indica se l'intestazione dello slicer è visibile. |
| [getShowMissing()](#getShowMissing--) | Indica se mostrare gli elementi eliminati dalla fonte dati. |
| [getShowTypeOfItemsWithNoData()](#getShowTypeOfItemsWithNoData--) | Indica se mostrare gli elementi eliminati dalla fonte dati. |
| [getSlicerCache()](#getSlicerCache--) | Restituisce l'oggetto SlicerCache associato allo slicer. |
| [getSortOrderType()](#getSortOrderType--) | Indica il tipo di ordinamento degli elementi. |
| [getStyleType()](#getStyleType--) | Specifica il tipo di stile incorporato per lo slicer. |
| [getTitle()](#getTitle--) | Specifica il titolo dell'oggetto Slicer corrente. |
| [getTopPixel()](#getTopPixel--) | Restituisce o imposta lo spostamento verticale della forma dello slicer dalla sua riga superiore, in pixel. |
| [getWidth()](#getWidth--) | Restituisce o imposta la larghezza dello slicer specificato, in punti. |
| [getWidthPixel()](#getWidthPixel--) | Restituisce o imposta la larghezza dello slicer specificato, in pixel. |
| [getWorksheet()](#getWorksheet--) | Restituisce l'oggetto [getWorksheet()](../../com.aspose.cells/slicer\#getWorksheet--) che contiene questo slicer. |
| [hashCode()](#hashCode--) |  |
| [isLocked()](#isLocked--) | Indica se la forma dello slicer è bloccata. |
| [isPrintable()](#isPrintable--) | Indica se l'oggetto slicer è stampabile. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [refresh()](#refresh--) | Aggiornamento degli elementi dello slicer dalle tabelle pivot associate. |
| [removePivotConnection(PivotTable pivot)](#removePivotConnection-com.aspose.cells.PivotTable-) | Rimuove la connessione alla PivotTable. |
| [selectItems(String[] labels, boolean append)](#selectItems-java.lang.String---boolean-) | **Osservazioni** |
| [setAlternativeText(String value)](#setAlternativeText-java.lang.String-) | Restituisce o imposta la stringa di testo descrittiva (alternativa) dell'oggetto Slicer. |
| [setCaption(String value)](#setCaption-java.lang.String-) | Restituisce o imposta la didascalia dello slicer specificato. |
| [setCaptionVisible(boolean value)](#setCaptionVisible-boolean-) | Restituisce o imposta se l'intestazione che visualizza la didascalia dello slicer è visibile. |
| [setColumnWidth(double value)](#setColumnWidth-double-) | Restituisce o imposta la larghezza di ogni colonna nello slicer in unità di punti. |
| [setColumnWidthPixel(int value)](#setColumnWidthPixel-int-) | Imposta la larghezza di\u807deogni colonna in\u807dil slicer, in unità di\u807dpixel.\u807d |
| [setFirstItemIndex(int value)](#setFirstItemIndex-int-) | Specifica l'indice basato su zero del primo elemento dello slicer. |
| [setHeight(double value)](#setHeight-double-) | Restituisce o imposta l'altezza dello slicer specificato, in punti. |
| [setHeightPixel(int value)](#setHeightPixel-int-) | Restituisce o imposta l'altezza dello slicer specificato, in pixel. |
| [setLeftPixel(int value)](#setLeftPixel-int-) | Restituisce o imposta lo spostamento orizzontale della forma dello slicer dalla sua colonna sinistra, in pixel. |
| [setLocked(boolean value)](#setLocked-boolean-) | Indica se la forma dello slicer è bloccata. |
| [setLockedAspectRatio(boolean value)](#setLockedAspectRatio-boolean-) | Indica se il blocco del rapporto d'aspetto è abilitato. |
| [setLockedPosition(boolean value)](#setLockedPosition-boolean-) | Indica se lo slicer specificato può essere spostato o ridimensionato tramite l'interfaccia utente. |
| [setName(String value)](#setName-java.lang.String-) | Restituisce o imposta il nome dello slicer specificato |
| [setNumberOfColumns(int value)](#setNumberOfColumns-int-) | Restituisce o imposta il numero di colonne nello slicer. |
| [setPlacement(int value)](#setPlacement-int-) | Rappresenta il modo in cui l'oggetto di disegno è collegato alle celle sottostanti. |
| [setPrintable(boolean value)](#setPrintable-boolean-) | Indica se l'oggetto slicer è stampabile. |
| [setRowHeight(double value)](#setRowHeight-double-) | Restituisce o imposta l'altezza di ogni riga nello slicer specificato in unità di punti. |
| [setRowHeightPixel(int value)](#setRowHeightPixel-int-) | Restituisce o imposta l'altezza di ogni riga nello slicer specificato, in unità di pixel. |
| [setShowAllItems(boolean value)](#setShowAllItems-boolean-) | Indica se mostrare tutti gli elementi anche se non ci sono dati o sono stati eliminati. |
| [setShowCaption(boolean value)](#setShowCaption-boolean-) | Indica se l'intestazione dello slicer è visibile. |
| [setShowMissing(boolean value)](#setShowMissing-boolean-) | Indica se mostrare gli elementi eliminati dalla fonte dati. |
| [setShowTypeOfItemsWithNoData(int value)](#setShowTypeOfItemsWithNoData-int-) | Indica se mostrare gli elementi eliminati dalla fonte dati. |
| [setSortOrderType(int value)](#setSortOrderType-int-) | Indica il tipo di ordinamento degli elementi. |
| [setStyleType(int value)](#setStyleType-int-) | Specifica il tipo di stile incorporato per lo slicer. |
| [setTitle(String value)](#setTitle-java.lang.String-) | Specifica il titolo dell'oggetto Slicer corrente. |
| [setTopPixel(int value)](#setTopPixel-int-) | Restituisce o imposta lo spostamento verticale della forma dello slicer dalla sua riga superiore, in pixel. |
| [setWidth(double value)](#setWidth-double-) | Restituisce o imposta la larghezza dello slicer specificato, in punti. |
| [setWidthPixel(int value)](#setWidthPixel-int-) | Restituisce o imposta la larghezza dello slicer specificato, in pixel. |
| [toString()](#toString--) |  |
| [unselectItems(String[] labels)](#unselectItems-java.lang.String---) | Rimuovi le etichette di filtro selezionate. |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### addPivotConnection(PivotTable pivot) {#addPivotConnection-com.aspose.cells.PivotTable-}
```
public void addPivotConnection(PivotTable pivot)
```


Aggiunge la connessione alla tabella pivot.

**Example**

```
         slicer.addPivotConnection(pivot);
```

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| pivot | [PivotTable](../../com.aspose.cells/pivottable) | L'oggetto PivotTable |

### clearFilter() {#clearFilter--}
```
public void clearFilter()
```


Rimuovi filtri

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
### getAlternativeText() {#getAlternativeText--}
```
public String getAlternativeText()
```


Restituisce o imposta la stringa di testo descrittiva (alternativa) dell'oggetto Slicer.

**Remarks**

NOTA: Questo membro è ora obsoleto. Invece, si prega di utilizzare la proprietà [Shape.getAlternativeText()](../../com.aspose.cells/shape\#getAlternativeText--). Questa proprietà sarà rimossa tra 12 mesi a partire da gennaio 2026. Aspose si scusa per qualsiasi inconveniente tu possa aver riscontrato.

**Example**

```
         slicer.removePivotConnection(pivot);
```

**Returns:**
java.lang.String
### getCaption() {#getCaption--}
```
public String getCaption()
```


Restituisce o imposta la didascalia dello slicer specificato.

**Example**

```
         slicer.setCaption("slicer caption");
```

**Returns:**
java.lang.String
### getCaptionVisible() {#getCaptionVisible--}
```
public boolean getCaptionVisible()
```


Restituisce o imposta se l'intestazione che visualizza la didascalia dello slicer è visibile. Il valore predefinito è true.

**Remarks**

NOTA: Questo membro è ora obsoleto. Invece, si prega di utilizzare la proprietà [getShowCaption()](../../com.aspose.cells/slicer\#getShowCaption--). Questa proprietà sarà rimossa tra 12 mesi a partire da gennaio 2026. Aspose si scusa per qualsiasi inconveniente tu possa aver riscontrato.

**Example**

```
         slicer.setCaption("slicer caption");
```

**Returns:**
boolean
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getColumnWidth() {#getColumnWidth--}
```
public double getColumnWidth()
```


Restituisce o imposta la larghezza di ogni colonna nello slicer in unità di punti.

**Example**

```
         slicer.setColumnWidth(80);
```

**Returns:**
double
### getColumnWidthPixel() {#getColumnWidthPixel--}
```
public int getColumnWidthPixel()
```


Restituisce la larghezza di\u807deach colonna in\u807dlo slicer, in unità di\u807dpixel.\u807d

**Example**

```
         slicer.setColumnWidthPixel(120);
```

**Returns:**
int
### getFirstItemIndex() {#getFirstItemIndex--}
```
public int getFirstItemIndex()
```


Specifica l'indice basato su zero del primo elemento dello slicer.

**Returns:**
int
### getHeight() {#getHeight--}
```
public double getHeight()
```


Restituisce o imposta l'altezza dello slicer specificato, in punti.

**Remarks**

NOTA: Questo membro è ora obsoleto. Invece, si prega di utilizzare la proprietà Shape.HeightPt. Questa proprietà sarà rimossa tra 12 mesi a partire da maggio 2025. Aspose si scusa per qualsiasi inconveniente tu possa aver riscontrato.

**Example**

```
         slicer.setNumberOfColumns(1);
```

**Returns:**
double
### getHeightPixel() {#getHeightPixel--}
```
public int getHeightPixel()
```


Restituisce o imposta l'altezza dello slicer specificato, in pixel.

**Remarks**

NOTA: Questo membro è ora obsoleto. Invece, si prega di utilizzare la proprietà Shape.Height. Questa proprietà sarà rimossa 12 mesi dopo da maggio 2025. Aspose si scusa per qualsiasi inconveniente tu possa aver sperimentato.

**Example**

```
         slicer.setNumberOfColumns(1);
```

**Returns:**
int
### getLeftPixel() {#getLeftPixel--}
```
public int getLeftPixel()
```


Restituisce o imposta lo spostamento orizzontale della forma dello slicer dalla sua colonna sinistra, in pixel.

**Remarks**

NOTA: Questo membro è ora obsoleto. Invece, si prega di utilizzare la proprietà Shape.Left. Questa proprietà sarà rimossa 12 mesi dopo da maggio 2025. Aspose si scusa per qualsiasi inconveniente tu possa aver sperimentato.

**Example**

```
         slicer.setNumberOfColumns(1);
```

**Returns:**
int
### getLockedAspectRatio() {#getLockedAspectRatio--}
```
public boolean getLockedAspectRatio()
```


Indica se il blocco del rapporto d'aspetto è abilitato.

**Remarks**

NOTA: Questo membro è ora obsoleto. Invece, si prega di utilizzare il metodo [Shape.isAspectRatioLocked()](../../com.aspose.cells/shape\#isAspectRatioLocked--). Questa proprietà sarà rimossa tra 12 mesi a partire da gennaio 2026. Aspose si scusa per qualsiasi inconveniente tu possa aver riscontrato.

**Example**

```
         slicer.removePivotConnection(pivot);
```

**Returns:**
boolean
### getLockedPosition() {#getLockedPosition--}
```
public boolean getLockedPosition()
```


Indica se lo slicer specificato può essere spostato o ridimensionato tramite l'interfaccia utente.

**Example**

```
         slicer.setLockedPosition(false);
```

**Returns:**
boolean
### getName() {#getName--}
```
public String getName()
```


Restituisce o imposta il nome dello slicer specificato

**Example**

```
         slicer.setName("slicer name");
```

**Returns:**
java.lang.String
### getNumberOfColumns() {#getNumberOfColumns--}
```
public int getNumberOfColumns()
```


Restituisce o imposta il numero di colonne nello slicer. Il valore predefinito è 1.

**Example**

```
         slicer.setNumberOfColumns(1);
```

**Returns:**
int
### getParent() {#getParent--}
```
public Worksheet getParent()
```


Restituisce l'oggetto [getWorksheet()](../../com.aspose.cells/slicer\#getWorksheet--) che contiene questo slicer. Sola lettura.

**Remarks**

NOTA: Questo membro è ora obsoleto. Invece, si prega di utilizzare la proprietà [getWorksheet()](../../com.aspose.cells/slicer\#getWorksheet--). Questa proprietà sarà rimossa tra 12 mesi a partire da gennaio 2026. Aspose si scusa per qualsiasi inconveniente tu possa aver riscontrato.

**Example**

```
         SlicerCache slicerCache = slicer.getSlicerCache();
```

**Returns:**
[Worksheet](../../com.aspose.cells/worksheet)
### getPlacement() {#getPlacement--}
```
public int getPlacement()
```


Rappresenta il modo in cui l'oggetto di disegno è collegato alle celle sottostanti. La proprietà controlla il posizionamento di un oggetto su un foglio di lavoro.

Vedi [PlacementType](../../com.aspose.cells/placementtype).

**Remarks**

NOTA: Questo membro è ora obsoleto. Invece, si prega di utilizzare la proprietà [Shape.getPlacement()](../../com.aspose.cells/shape\#getPlacement--). Questa proprietà sarà rimossa tra 12 mesi a partire da gennaio 2026. Aspose si scusa per qualsiasi inconveniente tu possa aver riscontrato.

**Example**

```
         slicer.removePivotConnection(pivot);
```

**Returns:**
int
### getRowHeight() {#getRowHeight--}
```
public double getRowHeight()
```


Restituisce o imposta l'altezza di ogni riga nello slicer specificato in unità di punti.

**Example**

```
         slicer.setRowHeight(20);
```

**Returns:**
double
### getRowHeightPixel() {#getRowHeightPixel--}
```
public int getRowHeightPixel()
```


Restituisce o imposta l'altezza di ogni riga nello slicer specificato, in unità di pixel.

**Example**

```
         slicer.setRowHeightPixel(30);
```

**Returns:**
int
### getShape() {#getShape--}
```
public SlicerShape getShape()
```


Restituisce l'oggetto Shape associato allo slicer specificato. Sola lettura.

**Returns:**
[SlicerShape](../../com.aspose.cells/slicershape)
### getShowAllItems() {#getShowAllItems--}
```
public boolean getShowAllItems()
```


Indica se mostrare tutti gli elementi anche se non ci sono dati o sono stati eliminati. Il valore predefinito è true;

**Returns:**
boolean
### getShowCaption() {#getShowCaption--}
```
public boolean getShowCaption()
```


Indica se l'intestazione dello slicer è visibile. Il valore predefinito è true

**Example**

```
         slicer.setShowCaption(false);
```

**Returns:**
boolean
### getShowMissing() {#getShowMissing--}
```
public boolean getShowMissing()
```


Indica se mostrare gli elementi eliminati dalla fonte dati.

**Remarks**

Funziona solo quando [getShowAllItems()](../../com.aspose.cells/slicer\#getShowAllItems--) è true.

**Returns:**
boolean
### getShowTypeOfItemsWithNoData() {#getShowTypeOfItemsWithNoData--}
```
public int getShowTypeOfItemsWithNoData()
```


Indica se mostrare gli elementi eliminati dalla fonte dati.

Vedi [ItemsWithNoDataShowMode](../../com.aspose.cells/itemswithnodatashowmode).

**Remarks**

Funziona solo quando [getShowAllItems()](../../com.aspose.cells/slicer\#getShowAllItems--) è true.

**Returns:**
int
### getSlicerCache() {#getSlicerCache--}
```
public SlicerCache getSlicerCache()
```


Restituisce l'oggetto SlicerCache associato allo slicer. Sola lettura.

**Example**

```
         SlicerCache slicerCache = slicer.getSlicerCache();
```

**Returns:**
[SlicerCache](../../com.aspose.cells/slicercache)
### getSortOrderType() {#getSortOrderType--}
```
public int getSortOrderType()
```


Indica il tipo di ordinamento degli elementi.

Vedi [SortOrder](../../com.aspose.cells/sortorder).

**Returns:**
int
### getStyleType() {#getStyleType--}
```
public int getStyleType()
```


Specifica il tipo di stile slicer incorporato. Il tipo predefinito è SlicerStyleLight1.

Vedi [SlicerStyleType](../../com.aspose.cells/slicerstyletype).

**Example**

```
         slicer.setStyleType(SlicerStyleType.SLICER_STYLE_LIGHT_2);
```

**Returns:**
int
### getTitle() {#getTitle--}
```
public String getTitle()
```


Specifica il titolo dell'oggetto Slicer corrente.

**Remarks**

NOTA: Questo membro è ora obsoleto. Invece, si prega di utilizzare la proprietà [Shape.getTitle()](../../com.aspose.cells/shape\#getTitle--). Questa proprietà sarà rimossa tra 12 mesi a partire da gennaio 2026. Aspose si scusa per qualsiasi inconveniente tu possa aver riscontrato.

**Example**

```
         slicer.removePivotConnection(pivot);
```

**Returns:**
java.lang.String
### getTopPixel() {#getTopPixel--}
```
public int getTopPixel()
```


Restituisce o imposta lo spostamento verticale della forma dello slicer dalla sua riga superiore, in pixel.

**Remarks**

NOTA: Questo membro è ora obsoleto. Invece, si prega di utilizzare la proprietà Shape.Top. Questa proprietà sarà rimossa 12 mesi dopo da maggio 2025. Aspose si scusa per qualsiasi inconveniente tu possa aver sperimentato.

**Example**

```
         slicer.setNumberOfColumns(1);
```

**Returns:**
int
### getWidth() {#getWidth--}
```
public double getWidth()
```


Restituisce o imposta la larghezza dello slicer specificato, in punti.

**Remarks**

NOTA: Questo membro è ora obsoleto. Invece, si prega di utilizzare la proprietà Shape.WidthPt. Questa proprietà sarà rimossa tra 12 mesi a partire da maggio 2025. Aspose si scusa per qualsiasi inconveniente tu possa aver riscontrato.

**Example**

```
         slicer.setNumberOfColumns(1);
```

**Returns:**
double
### getWidthPixel() {#getWidthPixel--}
```
public int getWidthPixel()
```


Restituisce o imposta la larghezza dello slicer specificato, in pixel.

**Remarks**

NOTA: Questo membro è ora obsoleto. Invece, si prega di utilizzare la proprietà Shape.Width. Questa proprietà sarà rimossa 12 mesi dopo da maggio 2025. Aspose si scusa per qualsiasi inconveniente tu possa aver sperimentato.

**Example**

```
         slicer.setNumberOfColumns(1);
```

**Returns:**
int
### getWorksheet() {#getWorksheet--}
```
public Worksheet getWorksheet()
```


Restituisce l'oggetto [getWorksheet()](../../com.aspose.cells/slicer\#getWorksheet--) che contiene questo slicer. Sola lettura.

**Example**

```
         Worksheet currSheet = slicer.getParent();
```

**Returns:**
[Worksheet](../../com.aspose.cells/worksheet)
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isLocked() {#isLocked--}
```
public boolean isLocked()
```


Indica se la forma dello slicer è bloccata.

**Remarks**

NOTA: Questo membro è ora obsoleto. Invece, si prega di utilizzare la proprietà [Shape.isLocked()](../../com.aspose.cells/shape\#isLocked--). Questa proprietà sarà rimossa tra 12 mesi a partire da gennaio 2026. Aspose si scusa per qualsiasi inconveniente tu possa aver riscontrato.

**Example**

```
         slicer.removePivotConnection(pivot);
```

**Returns:**
boolean
### isPrintable() {#isPrintable--}
```
public boolean isPrintable()
```


Indica se l'oggetto slicer è stampabile.

**Remarks**

NOTA: Questo membro è ora obsoleto. Invece, si prega di utilizzare la proprietà [Shape.isPrintable()](../../com.aspose.cells/shape\#isPrintable--). Questa proprietà sarà rimossa tra 12 mesi a partire da gennaio 2026. Aspose si scusa per qualsiasi inconveniente tu possa aver riscontrato.

**Example**

```
         slicer.removePivotConnection(pivot);
```

**Returns:**
boolean
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### refresh() {#refresh--}
```
public void refresh()
```


Aggiornamento degli elementi dello slicer dalle tabelle pivot associate.

**Example**

```
         slicer.refresh();
```

### removePivotConnection(PivotTable pivot) {#removePivotConnection-com.aspose.cells.PivotTable-}
```
public void removePivotConnection(PivotTable pivot)
```


Rimuove la connessione alla PivotTable.

**Example**

```
         slicer.removePivotConnection(pivot);
```

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| pivot | [PivotTable](../../com.aspose.cells/pivottable) | L'oggetto PivotTable |

### selectItems(String[] labels, boolean append) {#selectItems-java.lang.String---boolean-}
```
public void selectItems(String[] labels, boolean append)
```


**Remarks**

Se desideri selezionare tutti gli elementi, si prega di utilizzare il metodo [clearFilter()](../../com.aspose.cells/slicer\#clearFilter--).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| etichette | java.lang.String[] | Etichette selezionate. |
| aggiungi | boolean | False indica che vengono selezionate solo queste etichette e deselezionate le altre. True indica che vengono mantenuti gli elementi selezionati in precedenza e selezionate queste etichette. |

### setAlternativeText(String value) {#setAlternativeText-java.lang.String-}
```
public void setAlternativeText(String value)
```


Restituisce o imposta la stringa di testo descrittiva (alternativa) dell'oggetto Slicer.

**Remarks**

NOTA: Questo membro è ora obsoleto. Invece, si prega di utilizzare la proprietà [Shape.getAlternativeText()](../../com.aspose.cells/shape\#getAlternativeText--). Questa proprietà sarà rimossa tra 12 mesi a partire da gennaio 2026. Aspose si scusa per qualsiasi inconveniente tu possa aver riscontrato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### setCaption(String value) {#setCaption-java.lang.String-}
```
public void setCaption(String value)
```


Restituisce o imposta la didascalia dello slicer specificato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### setCaptionVisible(boolean value) {#setCaptionVisible-boolean-}
```
public void setCaptionVisible(boolean value)
```


Restituisce o imposta se l'intestazione che visualizza la didascalia dello slicer è visibile. Il valore predefinito è true.

**Remarks**

NOTA: Questo membro è ora obsoleto. Invece, si prega di utilizzare la proprietà [getShowCaption()](../../com.aspose.cells/slicer\#getShowCaption--). Questa proprietà sarà rimossa tra 12 mesi a partire da gennaio 2026. Aspose si scusa per qualsiasi inconveniente tu possa aver riscontrato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setColumnWidth(double value) {#setColumnWidth-double-}
```
public void setColumnWidth(double value)
```


Restituisce o imposta la larghezza di ogni colonna nello slicer in unità di punti.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | double |  |

### setColumnWidthPixel(int value) {#setColumnWidthPixel-int-}
```
public void setColumnWidthPixel(int value)
```


Imposta la larghezza di\u807deogni colonna in\u807dil slicer, in unità di\u807dpixel.\u807d

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setFirstItemIndex(int value) {#setFirstItemIndex-int-}
```
public void setFirstItemIndex(int value)
```


Specifica l'indice basato su zero del primo elemento dello slicer.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setHeight(double value) {#setHeight-double-}
```
public void setHeight(double value)
```


Restituisce o imposta l'altezza dello slicer specificato, in punti.

**Remarks**

NOTA: Questo membro è ora obsoleto. Invece, si prega di utilizzare la proprietà Shape.HeightPt. Questa proprietà sarà rimossa tra 12 mesi a partire da maggio 2025. Aspose si scusa per qualsiasi inconveniente tu possa aver riscontrato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | double |  |

### setHeightPixel(int value) {#setHeightPixel-int-}
```
public void setHeightPixel(int value)
```


Restituisce o imposta l'altezza dello slicer specificato, in pixel.

**Remarks**

NOTA: Questo membro è ora obsoleto. Invece, si prega di utilizzare la proprietà Shape.Height. Questa proprietà sarà rimossa 12 mesi dopo da maggio 2025. Aspose si scusa per qualsiasi inconveniente tu possa aver sperimentato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setLeftPixel(int value) {#setLeftPixel-int-}
```
public void setLeftPixel(int value)
```


Restituisce o imposta lo spostamento orizzontale della forma dello slicer dalla sua colonna sinistra, in pixel.

**Remarks**

NOTA: Questo membro è ora obsoleto. Invece, si prega di utilizzare la proprietà Shape.Left. Questa proprietà sarà rimossa 12 mesi dopo da maggio 2025. Aspose si scusa per qualsiasi inconveniente tu possa aver sperimentato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setLocked(boolean value) {#setLocked-boolean-}
```
public void setLocked(boolean value)
```


Indica se la forma dello slicer è bloccata.

**Remarks**

NOTA: Questo membro è ora obsoleto. Invece, si prega di utilizzare la proprietà [Shape.isLocked()](../../com.aspose.cells/shape\#isLocked--). Questa proprietà sarà rimossa tra 12 mesi a partire da gennaio 2026. Aspose si scusa per qualsiasi inconveniente tu possa aver riscontrato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setLockedAspectRatio(boolean value) {#setLockedAspectRatio-boolean-}
```
public void setLockedAspectRatio(boolean value)
```


Indica se il blocco del rapporto d'aspetto è abilitato.

**Remarks**

NOTA: Questo membro è ora obsoleto. Invece, si prega di utilizzare il metodo [Shape.isAspectRatioLocked()](../../com.aspose.cells/shape\#isAspectRatioLocked--). Questa proprietà sarà rimossa tra 12 mesi a partire da gennaio 2026. Aspose si scusa per qualsiasi inconveniente tu possa aver riscontrato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setLockedPosition(boolean value) {#setLockedPosition-boolean-}
```
public void setLockedPosition(boolean value)
```


Indica se lo slicer specificato può essere spostato o ridimensionato tramite l'interfaccia utente.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setName(String value) {#setName-java.lang.String-}
```
public void setName(String value)
```


Restituisce o imposta il nome dello slicer specificato

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### setNumberOfColumns(int value) {#setNumberOfColumns-int-}
```
public void setNumberOfColumns(int value)
```


Restituisce o imposta il numero di colonne nello slicer. Il valore predefinito è 1.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setPlacement(int value) {#setPlacement-int-}
```
public void setPlacement(int value)
```


Rappresenta il modo in cui l'oggetto di disegno è collegato alle celle sottostanti. La proprietà controlla il posizionamento di un oggetto su un foglio di lavoro.

Vedi [PlacementType](../../com.aspose.cells/placementtype).

**Remarks**

NOTA: Questo membro è ora obsoleto. Invece, si prega di utilizzare la proprietà [Shape.getPlacement()](../../com.aspose.cells/shape\#getPlacement--). Questa proprietà sarà rimossa tra 12 mesi a partire da gennaio 2026. Aspose si scusa per qualsiasi inconveniente tu possa aver riscontrato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setPrintable(boolean value) {#setPrintable-boolean-}
```
public void setPrintable(boolean value)
```


Indica se l'oggetto slicer è stampabile.

**Remarks**

NOTA: Questo membro è ora obsoleto. Invece, si prega di utilizzare la proprietà [Shape.isPrintable()](../../com.aspose.cells/shape\#isPrintable--). Questa proprietà sarà rimossa tra 12 mesi a partire da gennaio 2026. Aspose si scusa per qualsiasi inconveniente tu possa aver riscontrato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setRowHeight(double value) {#setRowHeight-double-}
```
public void setRowHeight(double value)
```


Restituisce o imposta l'altezza di ogni riga nello slicer specificato in unità di punti.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | double |  |

### setRowHeightPixel(int value) {#setRowHeightPixel-int-}
```
public void setRowHeightPixel(int value)
```


Restituisce o imposta l'altezza di ogni riga nello slicer specificato, in unità di pixel.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setShowAllItems(boolean value) {#setShowAllItems-boolean-}
```
public void setShowAllItems(boolean value)
```


Indica se mostrare tutti gli elementi anche se non ci sono dati o sono stati eliminati. Il valore predefinito è true;

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setShowCaption(boolean value) {#setShowCaption-boolean-}
```
public void setShowCaption(boolean value)
```


Indica se l'intestazione dello slicer è visibile. Il valore predefinito è true

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setShowMissing(boolean value) {#setShowMissing-boolean-}
```
public void setShowMissing(boolean value)
```


Indica se mostrare gli elementi eliminati dalla fonte dati.

**Remarks**

Funziona solo quando [getShowAllItems()](../../com.aspose.cells/slicer\#getShowAllItems--) è true.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setShowTypeOfItemsWithNoData(int value) {#setShowTypeOfItemsWithNoData-int-}
```
public void setShowTypeOfItemsWithNoData(int value)
```


Indica se mostrare gli elementi eliminati dalla fonte dati.

Vedi [ItemsWithNoDataShowMode](../../com.aspose.cells/itemswithnodatashowmode).

**Remarks**

Funziona solo quando [getShowAllItems()](../../com.aspose.cells/slicer\#getShowAllItems--) è true.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setSortOrderType(int value) {#setSortOrderType-int-}
```
public void setSortOrderType(int value)
```


Indica il tipo di ordinamento degli elementi.

Vedi [SortOrder](../../com.aspose.cells/sortorder).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setStyleType(int value) {#setStyleType-int-}
```
public void setStyleType(int value)
```


Specifica il tipo di stile slicer incorporato. Il tipo predefinito è SlicerStyleLight1.

Vedi [SlicerStyleType](../../com.aspose.cells/slicerstyletype).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setTitle(String value) {#setTitle-java.lang.String-}
```
public void setTitle(String value)
```


Specifica il titolo dell'oggetto Slicer corrente.

**Remarks**

NOTA: Questo membro è ora obsoleto. Invece, si prega di utilizzare la proprietà [Shape.getTitle()](../../com.aspose.cells/shape\#getTitle--). Questa proprietà sarà rimossa tra 12 mesi a partire da gennaio 2026. Aspose si scusa per qualsiasi inconveniente tu possa aver riscontrato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### setTopPixel(int value) {#setTopPixel-int-}
```
public void setTopPixel(int value)
```


Restituisce o imposta lo spostamento verticale della forma dello slicer dalla sua riga superiore, in pixel.

**Remarks**

NOTA: Questo membro è ora obsoleto. Invece, si prega di utilizzare la proprietà Shape.Top. Questa proprietà sarà rimossa 12 mesi dopo da maggio 2025. Aspose si scusa per qualsiasi inconveniente tu possa aver sperimentato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setWidth(double value) {#setWidth-double-}
```
public void setWidth(double value)
```


Restituisce o imposta la larghezza dello slicer specificato, in punti.

**Remarks**

NOTA: Questo membro è ora obsoleto. Invece, si prega di utilizzare la proprietà Shape.WidthPt. Questa proprietà sarà rimossa tra 12 mesi a partire da maggio 2025. Aspose si scusa per qualsiasi inconveniente tu possa aver riscontrato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | double |  |

### setWidthPixel(int value) {#setWidthPixel-int-}
```
public void setWidthPixel(int value)
```


Restituisce o imposta la larghezza dello slicer specificato, in pixel.

**Remarks**

NOTA: Questo membro è ora obsoleto. Invece, si prega di utilizzare la proprietà Shape.Width. Questa proprietà sarà rimossa 12 mesi dopo da maggio 2025. Aspose si scusa per qualsiasi inconveniente tu possa aver sperimentato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### toString() {#toString--}
```
public String toString()
```




**Returns:**
java.lang.String
### unselectItems(String[] labels) {#unselectItems-java.lang.String---}
```
public void unselectItems(String[] labels)
```


Rimuovi le etichette di filtro selezionate.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| etichette | java.lang.String[] | Le etichette. |

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

