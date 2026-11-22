---
title: "PivotCache.SourceCellArea"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية PivotCache. تُرجع نطاق مصدر البيانات باستخدام SourceSheet"
type: docs
url: /ar/net/aspose.cells.gridweb.data/pivotcache/sourcecellarea/
---
## PivotCache.SourceCellArea property

يرجع نطاق مصدر البيانات باستخدام SourceSheet.

```csharp
public WebCellArea SourceCellArea { get; }
```

### أمثلة

```csharp

 [C#]

 //يغيّر نطاق مصدر البيانات
 //القيمة الأصلية: StartRow=0;StartColumn=0;EndRow=10;EndColumn=4;
 PivotTable table = GridWeb1.WebWorksheets.PivotTables["myPivotTable"];
 //يضيف بيانات صفين
 table.PivotCache.SourceCellArea.EndRow = 12;

 [VB]

 'Changes data source range
 'Original value: StartRow=0;StartColumn=0;EndRow=10;EndColumn=4;
 Dim table As PivotTable =  GridWeb1.WebWorksheets.PivotTables("myPivotTable")
  'Adds 2 row data
 table.PivotCache.SourceCellArea.EndRow = 12
```

### انظر أيضًا

* class [WebCellArea](../../webcellarea/)
* class [PivotCache](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)


