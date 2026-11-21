---
title: "LightCellsDataHandler"
second_title: "Aspose.Cells för Java API-referens"
description: "Representerar cellernas datahanterare för att läsa stora kalkylbladsfiler i lättviktsläge."
type: docs
url: /sv/java/com.aspose.cells/lightcellsdatahandler/
---
```
public interface LightCellsDataHandler
```

Representerar cellernas datahanterare för att läsa stora kalkylbladsfiler i lättviktsläge.

**Remarks**

När en arbetsbok läses i detta läge, kommer [startSheet(Worksheet)](../../com.aspose.cells/lightcellsdatahandler\#startSheet-Worksheet-) att kontrolleras när varje kalkylblad i arbetsboken läses. För ett blad, om [startSheet(Worksheet)](../../com.aspose.cells/lightcellsdatahandler\#startSheet-Worksheet-) returnerar true, kommer all data och egenskaper för rader/celler i detta blad att kontrolleras och bearbetas av implementeringen av detta gränssnitt. För varje rad kommer [startRow(int)](../../com.aspose.cells/lightcellsdatahandler\#startRow-int-) att anropas för att kontrollera om den behöver bearbetas. Om en rad behöver bearbetas, läses först radens egenskaper och användaren kan komma åt dem via [processRow(Row)](../../com.aspose.cells/lightcellsdatahandler\#processRow-Row-). Om radens celler också behöver bearbetas, ska [processRow(Row)](../../com.aspose.cells/lightcellsdatahandler\#processRow-Row-) returnera true och sedan kommer [startCell(int)](../../com.aspose.cells/lightcellsdatahandler\#startCell-int-) att anropas för varje befintlig cell i raden för att kontrollera om en cell behöver bearbetas. Om en cell behöver bearbetas, kommer [processCell(Cell)](../../com.aspose.cells/lightcellsdatahandler\#processCell-Cell-) att anropas för att bearbeta cellen av implementeringen av detta gränssnitt.

Observera att användaren endast bör arbeta med värdena och egenskaperna för det aktuella Row/Cell-objektet som tillhandahålls av motsvarande metod. Eftersom cellernas data läses från mallfilen i strömmningsläge, kan de flesta andra objekt återställas/uppdateras senare efter att celldata har lästs in. Så när användaren arbetar med andra objekt i denna implementering, kan dessa operationer eventuellt inte påverka objekten som finns i arbetsboken. Ännu värre, dessa operationer kan orsaka inkonsekvent data i arbetsboken och sedan leda till oväntade problem eller undantag senare. Därför, för alla andra objekt såsom former, kolumnbredder och stilar, villkorsformatering, ...etc., vänligen arbeta inte med dem i några metoder i denna implementering. Hantera dem istället efter att arbetsboken har konstruerats.
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [processCell(Cell cell)](#processCell-com.aspose.cells.Cell-) | Startar bearbetning av en cell. |
| [processRow(Row row)](#processRow-com.aspose.cells.Row-) | Startar bearbetning av en rad. |
| [startCell(int columnIndex)](#startCell-int-) | Förbereder bearbetning av en cell. |
| [startRow(int rowIndex)](#startRow-int-) | Förbereder bearbetning av en rad. |
| [startSheet(Worksheet sheet)](#startSheet-com.aspose.cells.Worksheet-) | Startar bearbetning av ett kalkylblad. |
### processCell(Cell cell) {#processCell-com.aspose.cells.Cell-}
```
public abstract boolean processCell(Cell cell)
```


Startar bearbetning av en cell.

**Remarks**

Den kommer att anropas efter att en cells data har lästs.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| cell | [Cell](../../com.aspose.cells/cell) | Cellobjekt som för närvarande bearbetas |

**Returns:**
boolean – anger om denna cell ska behållas i cellmodellen för det aktuella bladet. Vanligtvis bör den vara false så att alla celler inte behålls i minnet efter att de har bearbetats, vilket sparar minne. För vissa speciella ändamål, såsom när användaren behöver komma åt vissa celler senare efter att hela arbetsboken har bearbetats, kan användaren låta denna metod returnera true för att behålla de speciella cellerna i Cells-modellen och komma åt dem senare via API:er som Cells[row, column]. Däremot kräver det att hålla celldata i Cells-modellen mer minne, och om alla celler behålls blir läsning av mallfilen i LightCells-läge samma som att läsa den på normalt sätt.
### processRow(Row row) {#processRow-com.aspose.cells.Row-}
```
public abstract boolean processRow(Row row)
```


Startar bearbetning av en rad.

**Remarks**

Den kommer att anropas efter att radens egenskaper såsom höjd, stil, ...etc. har lästs. Cellerna i denna rad har dock ännu inte lästs.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| row | [Row](../../com.aspose.cells/row) | Radobjekt som för närvarande bearbetas. |

**Returns:**
boolean - om cellerna i den här raden behöver bearbetas. false för att ignorera alla celler i den här raden.
### startCell(int columnIndex) {#startCell-int-}
```
public abstract boolean startCell(int columnIndex)
```


Förbereder bearbetning av en cell.

**Remarks**

Den kommer att anropas när en befintlig cell i den aktuella raden nås. Aktuell rad är raden för det senaste anropet av [processRow(Row)](../../com.aspose.cells/lightcellsdatahandler\\#processRow-Row-).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| columnIndex | int | kolumnindex för cellen som ska bearbetas |

**Returns:**
boolean - om den här cellen behöver bearbetas. false för att ignorera cellen och kontrollera nästa tills slutet av celldata i den aktuella raden nås
### startRow(int rowIndex) {#startRow-int-}
```
public abstract boolean startRow(int rowIndex)
```


Förbereder bearbetning av en rad.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| rowIndex | int | index för nästa rad som ska bearbetas |

**Returns:**
boolean - om den här raden (egenskaper eller celldata) behöver bearbetas. false för att ignorera denna rad och dess celler och kontrollera nästa rad.
### startSheet(Worksheet sheet) {#startSheet-com.aspose.cells.Worksheet-}
```
public abstract boolean startSheet(Worksheet sheet)
```


Startar bearbetning av ett kalkylblad.

**Remarks**

Den kommer att anropas innan celldata i ett kalkylblad läses.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| sheet | [Worksheet](../../com.aspose.cells/worksheet) | kalkylbladet för att läsa celldata. |

**Returns:**
boolean - om detta bladets celldata behöver bearbetas. false för att ignorera detta blad.
