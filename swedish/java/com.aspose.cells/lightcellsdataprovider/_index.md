---
title: "LightCellsDataProvider"
second_title: "Aspose.Cells för Java API-referens"
description: "Representerar dataleverantör för att spara stora kalkylbladsfiler i lättviktsläge."
type: docs
url: /sv/java/com.aspose.cells/lightcellsdataprovider/
---
```
public interface LightCellsDataProvider
```

Representerar dataleverantör för att spara stora kalkylbladsfiler i lättviktsläge.

**Remarks**

När du sparar en arbetsbok med detta läge, kommer [startSheet(int)](../../com.aspose.cells/lightcellsdataprovider\#startSheet-int-) att kontrolleras när varje kalkylblad i arbetsboken sparas. För ett blad, om [startSheet(int)](../../com.aspose.cells/lightcellsdataprovider\#startSheet-int-) returnerar true, kommer all data och egenskaper som ska sparas för rader/celler i detta blad att tillhandahållas av implementeringen av detta gränssnitt. Till att börja med kommer [nextRow()](../../com.aspose.cells/lightcellsdataprovider\#nextRow--) att anropas för att få nästa radindex som ska sparas. Om ett giltigt radindex returneras (radindexet måste vara i stigande ordning för raderna som ska sparas), kommer ett Row‑objekt som representerar denna rad att tillhandahållas av [startRow(Row)](../../com.aspose.cells/lightcellsdataprovider\#startRow-Row-) så att implementeringen kan sätta dess egenskaper. För en rad kommer [nextCell()](../../com.aspose.cells/lightcellsdataprovider\#nextCell--) att kontrolleras först. Om ett giltigt kolumnindex returneras (kolumnindexet måste vara i stigande ordning för alla celler i den aktuella raden), kommer ett Cell‑objekt som representerar denna cell att tillhandahållas av [startCell(Cell)](../../com.aspose.cells/lightcellsdataprovider\#startCell-Cell-) så att implementeringen kan sätta dess data och egenskaper. Efter [startCell(Cell)](../../com.aspose.cells/lightcellsdataprovider\#startCell-Cell-) sparas cellen direkt till den resulterande kalkylarksfilen. Därefter kontrolleras och bearbetas nästa cell.

Observera att användaren endast ska uppdatera värden och egenskaper för det aktuella Row/Cell‑objektet som tillhandahålls av motsvarande metod. Eftersom cellernas data skrivs till den resulterande filen i strömmad form, kan de flesta andra objekt redan ha skrivits till den resulterande filen, eller ha samlats och skrivit viss global data för dem. Så när användaren uppdaterar andra objekt medan celldata sparas, kan dessa operationer eventuellt inte påverka den sparade datan. Eller ännu värre, dessa operationer kan leda till inkonsekvent data som sparas till den resulterande filen och slutligen göra filen korrupt. Så för alla andra objekt såsom former, kolumnbredder och stilar, villkorsstyrd formatering, …etc., vänligen utför inga operationer på dem i någon metod i denna implementation. Hantera dem istället och justera dem till slutligt tillstånd innan du anropar metoden \"Save\" för Workbook.
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [isGatherString()](#isGatherString--) | Kontrollerar om det aktuella strängvärdet för cellen behöver samlas in i en global pool. |
| [nextCell()](#nextCell--) | Hämtar nästa cell som ska sparas. |
| [nextRow()](#nextRow--) | Hämtar nästa rad som ska sparas. |
| [startCell(Cell cell)](#startCell-com.aspose.cells.Cell-) | Påbörjar sparandet av data för en cell. |
| [startRow(Row row)](#startRow-com.aspose.cells.Row-) | Påbörjar sparandet av data för en rad. |
| [startSheet(int sheetIndex)](#startSheet-int-) | Påbörjar sparandet av ett kalkylblad. |
### isGatherString() {#isGatherString--}
```
public abstract boolean isGatherString()
```


Kontrollerar om det aktuella strängvärdet för cellen behöver samlas in i en global pool.

**Remarks**

Att samla in strängvärden ger fördelar endast när det finns många duplicerade strängvärden för cellerna som tillhandahålls av denna implementation. I detta fall sparar insamling av strängar mycket minne och genererar en mindre resulterande fil. Om det finns många strängvärden för cellerna som tillhandahålls av LightCellsDataProvider men få av dem är lika, kommer insamling av strängar att kräva mer minne och tid och har ingen fördel för den resulterande filen.

**Returns:**
boolean – true om strängvärdet behöver samlas in i en global pool för den resulterande filen.
### nextCell() {#nextCell--}
```
public abstract int nextCell()
```


Hämtar nästa cell som ska sparas.

**Remarks**

Den kommer att anropas i början av sparandet av en cell.

**Returns:**
int - kolumnindex för nästa cell som ska sparas. -1 betyder att slutet av den aktuella radens data har nåtts och ingen ytterligare cell i den aktuella raden ska sparas.
### nextRow() {#nextRow--}
```
public abstract int nextRow()
```


Hämtar nästa rad som ska sparas.

**Remarks**

Den kommer att anropas i början av att spara en rad och dess celldata(före [startRow(Row)](../../com.aspose.cells/lightcellsdataprovider\#startRow-Row-)).

**Returns:**
int - nästa radindex som ska sparas. -1 betyder att slutet av det aktuella bladets data har nåtts och ingen ytterligare rad i det aktuella bladet ska sparas.
### startCell(Cell cell) {#startCell-com.aspose.cells.Cell-}
```
public abstract void startCell(Cell cell)
```


Påbörjar sparandet av data för en cell.

**Remarks**

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| cell | [Cell](../../com.aspose.cells/cell) | Cell-objekt för implementering för att fylla data. Dess kolumnindex är det returnerade värdet från det senaste anropet av [nextCell()](../../com.aspose.cells/lightcellsdataprovider\#nextCell--). Om cellen har initierats i den interna cellmodellen kommer det befintliga cellobjektet att användas. Annars kommer ett tillfälligt Cell-objekt att användas för implementering för att fylla data. |

### startRow(Row row) {#startRow-com.aspose.cells.Row-}
```
public abstract void startRow(Row row)
```


Påbörjar sparandet av data för en rad.

**Remarks**

Den kommer att anropas i början av att spara en rad och dess celldata. Om den aktuella raden har vissa anpassade egenskaper såsom höjd, stil, ...etc., bör implementeringen sätta dessa egenskaper på det givna Row-objektet här.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| row | [Row](../../com.aspose.cells/row) | Row-objekt för implementering för att fylla data. Dess radindex är det returnerade värdet från det senaste anropet av [nextRow()](../../com.aspose.cells/lightcellsdataprovider\#nextRow--). Om raden har initierats i den interna cellmodellen kommer det befintliga radobjektet att användas. Annars kommer ett tillfälligt Row-objekt att användas för implementering för att fylla data. |

### startSheet(int sheetIndex) {#startSheet-int-}
```
public abstract boolean startSheet(int sheetIndex)
```


Påbörjar sparandet av ett kalkylblad.

**Remarks**

Den kommer att anropas i början av att spara ett arbetsblad under sparande av en arbetsbok. Om leverantören behöver referera till *`sheetIndex`* senare i startRow(Row)- eller startCell(Cell)-metoden, det vill säga om processen behöver veta vilket arbetsblad som bearbetas, bör implementeringen behålla *`sheetIndex`*-värdet här.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| sheetIndex | int | index för aktuellt blad som ska sparas. |

**Returns:**
boolean - true om denna leverantör kommer att tillhandahålla data för det angivna bladet; false om det angivna bladet ska använda sin normala datamodell (Cells).
