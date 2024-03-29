---
title: IsGatherString
second_title: Aspose.Cells för .NET API-referens
description: Kontrollerar om det aktuella strängvärdet för cellen måste samlas in i en global pool.
type: docs
weight: 10
url: /sv/net/aspose.cells/lightcellsdataprovider/isgatherstring/
---
## LightCellsDataProvider.IsGatherString method

Kontrollerar om det aktuella strängvärdet för cellen måste samlas in i en global pool.

```csharp
public bool IsGatherString()
```

### Returvärde

true om strängvärdet måste samlas in i en global pool för den resulterande filen.

### Anmärkningar

Att samla in strängvärden kommer bara att dra fördel när det finns många dubblerade strängvärden för cellerna som tillhandahålls av denna implementering. I den här situationen kommer insamlingssträngen att spara mycket minne och generera mindre resulterande fil. Om det finns många strängvärden för de tillhandahållna cellerna av LightCellsDataProvider men få av dem är samma, att samla strängar kommer att kosta mer minne och tid och har ingen fördel för den resulterande filen.

### Se även

* interface [LightCellsDataProvider](../../lightcellsdataprovider)
* namnutrymme [Aspose.Cells](../../lightcellsdataprovider)
* hopsättning [Aspose.Cells](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
