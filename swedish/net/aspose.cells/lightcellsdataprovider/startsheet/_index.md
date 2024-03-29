---
title: StartSheet
second_title: Aspose.Cells för .NET API-referens
description: Börjar spara ett kalkylblad.
type: docs
weight: 60
url: /sv/net/aspose.cells/lightcellsdataprovider/startsheet/
---
## LightCellsDataProvider.StartSheet method

Börjar spara ett kalkylblad.

```csharp
public bool StartSheet(int sheetIndex)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| sheetIndex | Int32 | index för aktuellt ark som ska sparas. |

### Returvärde

true om denna leverantör kommer att tillhandahålla data för det givna arket; false om ett visst ark ska använda sin normala datamodell (celler).

### Anmärkningar

Den kommer att anropas i början av att spara ett kalkylblad när en arbetsbok sparas. Om leverantören behöver hänvisa till

```csharp
sheetIndex
```

later i startRow(Row) eller startCell(Cell)-metoden, det vill säga om processen behöver veta vilket kalkylblad som bearbetas, ska implementeringen behålla

```csharp
sheetIndex
```

värde här.

### Se även

* interface [LightCellsDataProvider](../../lightcellsdataprovider)
* namnutrymme [Aspose.Cells](../../lightcellsdataprovider)
* hopsättning [Aspose.Cells](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
