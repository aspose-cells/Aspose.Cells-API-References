---
title: "Sınıf DiscreteGroupItem"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Pivot.DiscreteGroupItem sınıfı. Özel gruplanmış alanın bir öğesini temsil eder"
type: docs
url: /tr/net/aspose.cells.pivot/discretegroupitem/
---
## DiscreteGroupItem class

Özel gruplandırılmış alanın bir öğesini temsil eder.

```csharp
public class DiscreteGroupItem
```

## Yapıcılar

| Ad | Açıklama |
| --- | --- |
| [DiscreteGroupItem](discretegroupitem/#constructor)(string, int[]) | Pivot alanının özel grup öğesinin yapıcı yöntemi. |
| [DiscreteGroupItem](discretegroupitem/#constructor_1)(string, string[]) | Pivot alanının özel grup öğesinin yapıcı yöntemi. |

### Örnekler

```csharp

[C#]
Workbook book = new Workbook();
Worksheet sheet = book.Worksheets[0];
Cells cells = sheet.Cells;
cells[0, 0].Value = "product";
cells[1, 0].Value = "grape";
cells[2, 0].Value = "carrot";
cells[3, 0].Value = "potato";
cells[4, 0].Value = "cherry";

//Tarih stilini oluştur.
Style dateStyle = new CellsFactory().CreateStyle();
dateStyle.Custom = "m/d/yyyy";
cells[0, 1].Value = "date";
cells[1, 1].Value = new DateTime(2021, 2, 5);
cells[2, 1].Value = new DateTime(2022, 3, 8);
cells[3, 1].Value = new DateTime(2023, 4, 10);
cells[4, 1].Value = new DateTime(2024, 5, 16);
//Tarih stilini ayarla.
cells[1, 1].SetStyle(dateStyle);
cells[2, 1].SetStyle(dateStyle);
cells[3, 1].SetStyle(dateStyle);
cells[4, 1].SetStyle(dateStyle);

cells[0, 2].Value = "amount";
cells[1, 2].Value = 50;
cells[2, 2].Value = 60;
cells[3, 2].Value = 70;
cells[4, 2].Value = 80;

PivotTableCollection pivots = sheet.PivotTables;
//Bir PivotTable ekle.
PivotTable pivot = pivots.Add("=Sheet1!A1:C5", "A12");

pivot.AddFieldToArea(PivotFieldType.Row, "product");
pivot.AddFieldToArea(PivotFieldType.Column, "date");
pivot.AddFieldToArea(PivotFieldType.Data, "amount");
pivot.PivotTableStyleType = PivotTableStyleType.PivotTableStyleMedium10;

//Meyve ve sebzeye göre grupla
DiscreteGroupItem fruit = new DiscreteGroupItem("fruit", new int[] { 0, 3 });
DiscreteGroupItem vegetable = new DiscreteGroupItem("vegetable", new int[] { 1, 2 });
PivotFieldGroupOptions groupOptions = new PivotFieldGroupOptions();
groupOptions.DiscreteGroupItems = new DiscreteGroupItem[] { fruit, vegetable };
pivot.RowFields[0].Group(groupOptions);
pivot.CalculateData();

//işinizi yapın

book.Save("DiscreteGroup.xlsx");

[Visual Basic]

Dim book As New Workbook()
Dim sheet As Worksheet = book.Worksheets(0)
Dim cells As Cells = sheet.Cells
cells(0, 0).Value = "product"
cells(1, 0).Value = "grape"
cells(2, 0).Value = "carrot"
cells(3, 0).Value = "potato"
cells(4, 0).Value = "cherry"

'Create date style
Dim dateStyle As Style = New CellsFactory().CreateStyle()
dateStyle.Custom = "m/d/yyyy"
cells(0, 1).Value = "date"
cells(1, 1).Value = New DateTime(2021, 2, 5)
cells(2, 1).Value = New DateTime(2022, 3, 8)
cells(3, 1).Value = New DateTime(2023, 4, 10)
cells(4, 1).Value = New DateTime(2024, 5, 16)
'Set date style
cells(1, 1).SetStyle(dateStyle)
cells(2, 1).SetStyle(dateStyle)
cells(3, 1).SetStyle(dateStyle)
cells(4, 1).SetStyle(dateStyle)

cells(0, 2).Value = "amount"
cells(1, 2).Value = 50
cells(2, 2).Value = 60
cells(3, 2).Value = 70
cells(4, 2).Value = 80

Dim pivots As PivotTableCollection = sheet.PivotTables
'Add a PivotTable
Dim pivot As PivotTable = pivots.Add("=Sheet1!A1:C5", "A12")

pivot.AddFieldToArea(PivotFieldType.Row, "product")
pivot.AddFieldToArea(PivotFieldType.Column, "date")
pivot.AddFieldToArea(PivotFieldType.Data, "amount")
pivot.PivotTableStyleType = PivotTableStyleType.PivotTableStyleMedium10

'Group by fruit and vegetable
Dim fruit As New DiscreteGroupItem("fruit", New Integer() {0, 3})
Dim vegetable As New DiscreteGroupItem("vegetable", New Integer() {1, 2})
Dim groupOptions As New PivotFieldGroupOptions()
groupOptions.DiscreteGroupItems = New DiscreteGroupItem() {fruit, vegetable}
pivot.RowFields(0).Group(groupOptions)
pivot.CalculateData()

'do your business

book.Save("DiscreteGroup.xlsx")
```

### Ayrıca Bakınız

* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)


