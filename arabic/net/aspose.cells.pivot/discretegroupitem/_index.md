---
title: "الفئة DiscreteGroupItem"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "Aspose.Cells.Pivot.DiscreteGroupItem فئة. يمثل عنصرًا لحقل مجموعة مخصص"
type: docs
url: /ar/net/aspose.cells.pivot/discretegroupitem/
---
## DiscreteGroupItem class

يمثل عنصرًا من حقل مجموعة مخصص.

```csharp
public class DiscreteGroupItem
```

## المنشئات

| الاسم | الوصف |
| --- | --- |
| [DiscreteGroupItem](discretegroupitem/#constructor)(string, int[]) | المُنشئ الخاص بعنصر مجموعة مخصص لحقل المحور. |
| [DiscreteGroupItem](discretegroupitem/#constructor_1)(string, string[]) | المُنشئ الخاص بعنصر مجموعة مخصص لحقل المحور. |

### أمثلة

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

//إنشاء نمط تاريخ
Style dateStyle = new CellsFactory().CreateStyle();
dateStyle.Custom = "m/d/yyyy";
cells[0, 1].Value = "date";
cells[1, 1].Value = new DateTime(2021, 2, 5);
cells[2, 1].Value = new DateTime(2022, 3, 8);
cells[3, 1].Value = new DateTime(2023, 4, 10);
cells[4, 1].Value = new DateTime(2024, 5, 16);
//ضبط نمط التاريخ
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
//إضافة PivotTable
PivotTable pivot = pivots.Add("=Sheet1!A1:C5", "A12");

pivot.AddFieldToArea(PivotFieldType.Row, "product");
pivot.AddFieldToArea(PivotFieldType.Column, "date");
pivot.AddFieldToArea(PivotFieldType.Data, "amount");
pivot.PivotTableStyleType = PivotTableStyleType.PivotTableStyleMedium10;

//تجميع حسب الفواكه والخضروات
DiscreteGroupItem fruit = new DiscreteGroupItem("fruit", new int[] { 0, 3 });
DiscreteGroupItem vegetable = new DiscreteGroupItem("vegetable", new int[] { 1, 2 });
PivotFieldGroupOptions groupOptions = new PivotFieldGroupOptions();
groupOptions.DiscreteGroupItems = new DiscreteGroupItem[] { fruit, vegetable };
pivot.RowFields[0].Group(groupOptions);
pivot.CalculateData();

//قم بأعمالك

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

### انظر أيضًا

* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)


