---
title: Add
second_title: Aspose.Cells för .NET API-referens
description: Lägger till en ny PivotTable-cache till en PivotCaches-samling.
type: docs
weight: 20
url: /sv/net/aspose.cells.pivot/pivottablecollection/add/
---
## Add(string, string, string) {#add_4}

Lägger till en ny PivotTable-cache till en PivotCaches-samling.

```csharp
public int Add(string sourceData, string destCellName, string tableName)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| sourceData | String | Data för den nya PivotTable-cachen. |
| destCellName | String | Cellen i det övre vänstra hörnet av pivottabellrapportens målområde. |
| tableName | String | Namnet på den nya pivottabellsrapporten. |

### Returvärde

Det nya tillagda cacheindexet.

### Se även

* class [PivotTableCollection](../../pivottablecollection)
* namnutrymme [Aspose.Cells.Pivot](../../pivottablecollection)
* hopsättning [Aspose.Cells](../../../)

---

## Add(string, string, string, bool) {#add_5}

Lägger till en ny PivotTable-cache till en PivotCaches-samling.

```csharp
public int Add(string sourceData, string destCellName, string tableName, bool useSameSource)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| sourceData | String | Data för den nya PivotTable-cachen. |
| destCellName | String | Cellen i det övre vänstra hörnet av pivottabellrapportens målområde. |
| tableName | String | Namnet på den nya pivottabellsrapporten. |
| useSameSource | Boolean | Indikerar om samma datakälla används när en annan befintlig pivottabell har använt denna datakälla. Om egenskapen är true kommer den att spara minne. |

### Returvärde

Det nya tillagda cacheindexet.

### Se även

* class [PivotTableCollection](../../pivottablecollection)
* namnutrymme [Aspose.Cells.Pivot](../../pivottablecollection)
* hopsättning [Aspose.Cells](../../../)

---

## Add(string, int, int, string) {#add_2}

Lägger till en ny PivotTable-cache till en PivotCaches-samling.

```csharp
public int Add(string sourceData, int row, int column, string tableName)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| sourceData | String | Datacellintervallet för den nya pivottabellen.Exempel: Blad1!A1:C8 |
| row | Int32 | Radindex för cellen i det övre vänstra hörnet av pivottabellrapportens målområde. |
| column | Int32 | Kolumnindex för cellen i det övre vänstra hörnet av pivottabellrapportens målområde. |
| tableName | String | Namnet på den nya pivottabellsrapporten. |

### Returvärde

Det nya tillagda cacheindexet.

### Se även

* class [PivotTableCollection](../../pivottablecollection)
* namnutrymme [Aspose.Cells.Pivot](../../pivottablecollection)
* hopsättning [Aspose.Cells](../../../)

---

## Add(string, int, int, string, bool) {#add_3}

Lägger till en ny PivotTable-cache till en PivotCaches-samling.

```csharp
public int Add(string sourceData, int row, int column, string tableName, bool useSameSource)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| sourceData | String | Datacellintervallet för den nya pivottabellen.Exempel: Blad1!A1:C8 |
| row | Int32 | Radindex för cellen i det övre vänstra hörnet av pivottabellrapportens målområde. |
| column | Int32 | Kolumnindex för cellen i det övre vänstra hörnet av pivottabellrapportens målområde. |
| tableName | String | Namnet på den nya pivottabellsrapporten. |
| useSameSource | Boolean | Indikerar om samma datakälla används när en annan befintlig pivottabell har använt denna datakälla. Om egenskapen är true kommer den att spara minne. |

### Returvärde

Det nya tillagda cacheindexet.

### Se även

* class [PivotTableCollection](../../pivottablecollection)
* namnutrymme [Aspose.Cells.Pivot](../../pivottablecollection)
* hopsättning [Aspose.Cells](../../../)

---

## Add(PivotTable, string, string) {#add_1}

Lägger till ett nytt pivottabellobjekt till samlingen från en annan pivottabell.

```csharp
public int Add(PivotTable pivotTable, string destCellName, string tableName)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| pivotTable | PivotTable | Källpivottabellen. |
| destCellName | String | Cellen i det övre vänstra hörnet av pivottabellrapportens målområde. |
| tableName | String | Namnet på den nya pivottabellsrapporten. |

### Returvärde

Det nya tillagda pivottabellindexet.

### Se även

* class [PivotTable](../../pivottable)
* class [PivotTableCollection](../../pivottablecollection)
* namnutrymme [Aspose.Cells.Pivot](../../pivottablecollection)
* hopsättning [Aspose.Cells](../../../)

---

## Add(PivotTable, int, int, string) {#add}

Lägger till ett nytt pivottabellobjekt till samlingen från en annan pivottabell.

```csharp
public int Add(PivotTable pivotTable, int row, int column, string tableName)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| pivotTable | PivotTable | Källpivottabellen. |
| row | Int32 | Radindex för cellen i det övre vänstra hörnet av pivottabellrapportens målområde. |
| column | Int32 | Kolumnindex för cellen i det övre vänstra hörnet av pivottabellrapportens målområde. |
| tableName | String | Namnet på den nya pivottabellsrapporten. |

### Returvärde

Det nya tillagda pivottabellindexet.

### Se även

* class [PivotTable](../../pivottable)
* class [PivotTableCollection](../../pivottablecollection)
* namnutrymme [Aspose.Cells.Pivot](../../pivottablecollection)
* hopsättning [Aspose.Cells](../../../)

---

## Add(string[], bool, PivotPageFields, string, string) {#add_7}

Lägger till ett nytt pivottabellobjekt till samlingen med flera konsolideringsintervall som datakälla.

```csharp
public int Add(string[] sourceData, bool isAutoPage, PivotPageFields pageFields, 
    string destCellName, string tableName)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| sourceData | String[] | De flera konsolideringsintervallen, som {"Sheet1!A1:C8","Sheet2!A1:B8"} |
| isAutoPage | Boolean | Huruvida automatiskt skapa ett enda sidfält. Om sant, kommer följande param pageFields att ignoreras. |
| pageFields | PivotPageFields | Pivotsidans fältobjekt. |
| destCellName | String | destCellName Namnet på den nya pivottabellsrapporten. |
| tableName | String | namnet på den nya pivottabellsrapporten. |

### Returvärde

Det nya tillagda pivottabellindexet.

### Se även

* class [PivotPageFields](../../pivotpagefields)
* class [PivotTableCollection](../../pivottablecollection)
* namnutrymme [Aspose.Cells.Pivot](../../pivottablecollection)
* hopsättning [Aspose.Cells](../../../)

---

## Add(string[], bool, PivotPageFields, int, int, string) {#add_6}

Lägger till ett nytt pivottabellobjekt till samlingen med flera konsolideringsintervall som datakälla.

```csharp
public int Add(string[] sourceData, bool isAutoPage, PivotPageFields pageFields, int row, 
    int column, string tableName)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| sourceData | String[] | De flera konsolideringsintervallen, som {"Sheet1!A1:C8","Sheet2!A1:B8"} |
| isAutoPage | Boolean | Huruvida automatiskt skapa ett enda sidfält. Om sant, kommer följande param pageFields att ignoreras |
| pageFields | PivotPageFields | Pivotsidans fältobjekt. |
| row | Int32 | Radindex för cellen i det övre vänstra hörnet av pivottabellrapportens målområde. |
| column | Int32 | Kolumnindex för cellen i det övre vänstra hörnet av pivottabellrapportens målområde. |
| tableName | String | Namnet på den nya pivottabellsrapporten. |

### Returvärde

Det nya tillagda pivottabellindexet.

### Se även

* class [PivotPageFields](../../pivotpagefields)
* class [PivotTableCollection](../../pivottablecollection)
* namnutrymme [Aspose.Cells.Pivot](../../pivottablecollection)
* hopsättning [Aspose.Cells](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
