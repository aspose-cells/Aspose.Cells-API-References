---
title: "PivotArea.SelectField"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PivotArea method. Wählt ein Feld im Bereich als Gebiet aus"
type: docs
url: /de/net/aspose.cells.pivot/pivotarea/selectfield/
---
## SelectField(PivotFieldType, string) {#selectfield_1}

Wählen Sie ein Feld im Bereich als Bereich aus.

```csharp
public void SelectField(PivotFieldType axisType, string fieldName)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| axisType | PivotFieldType | Der Regionstyp. |
| fieldName | String | Der Name des Pivotfelds. |

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotAreaMethodSelectFieldWithPivotFieldTypeStringDemo
    {
        public static void Run()
        {
            // Erstelle eine Arbeitsmappe
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Füge Beispieldaten für die Pivot‑Tabelle hinzu
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Product");
            worksheet.Cells["C1"].PutValue("Sales");
            worksheet.Cells["A2"].PutValue("Electronics");
            worksheet.Cells["B2"].PutValue("Laptop");
            worksheet.Cells["C2"].PutValue(1200);
            worksheet.Cells["A3"].PutValue("Electronics");
            worksheet.Cells["B3"].PutValue("Phone");
            worksheet.Cells["C3"].PutValue(800);
            worksheet.Cells["A4"].PutValue("Clothing");
            worksheet.Cells["B4"].PutValue("Shirt");
            worksheet.Cells["C4"].PutValue(50);

            // PivotTable hinzufügen
            PivotTableCollection pivotTables = worksheet.PivotTables;
            int pivotIndex = pivotTables.Add("A1:C4", "E3", "PivotTable1");
            PivotTable pivotTable = pivotTables[pivotIndex];

            // Fügt Felder zu Pivot-Bereichen hinzu.
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Category");
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Bedingte Formatierung erstellen
            PivotConditionalFormat pcf = pivotTable.ConditionalFormats[pivotTable.ConditionalFormats.Add()];
            pcf.ScopeType = PivotConditionFormatScopeType.Field;

            // Demonstriere SelectField mit PivotFieldType und Zeichenkettenparametern
            PivotArea pivotArea = new PivotArea(pivotTable);
            pivotArea.SelectField(PivotFieldType.Data, "Sales");
            pivotArea.SelectField(PivotFieldType.Row, "Category");
            pcf.PivotAreas.Add(pivotArea);

            // Speichere die Arbeitsmappe
            workbook.Save("PivotAreaSelectFieldDemo.xlsx");
        }
    }
}
```

### Siehe auch

* enum [PivotFieldType](../../pivotfieldtype/)
* class [PivotArea](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## SelectField(PivotFieldType, PivotField) {#selectfield}

Wählen Sie ein Feld im Bereich als Bereich aus.

```csharp
public void SelectField(PivotFieldType axisType, PivotField field)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| axisType | PivotFieldType | Der Regionstyp. |
| Feld | PivotField | Das Pivotfeld. |

### Beispiele

```csharp
using System;
using System.IO;
using System.Text;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotAreaMethodSelectFieldWithPivotFieldTypePivotFieldDemo
    {
        public static void Run()
        {
            byte[] SrcDataByteArray = Encoding.ASCII.GetBytes(
@"City,Product,Sales
Paris,Cream,2300
Paris,Lotion,1600
Tunis,Cream,900
Tunis,Lotion,1400
Tunis,Cream,3090
Tunis,Lotion,6000
Paris,Cream,4320");

            using (MemoryStream dataStream = new MemoryStream(SrcDataByteArray))
            {
                Workbook wb = new Workbook(dataStream, new LoadOptions(LoadFormat.Csv));
                Worksheet sheet = wb.Worksheets[0];
                
                PivotTableCollection pivotTables = sheet.PivotTables;
                int pivotIndex = pivotTables.Add("=A1:C8", "F3", "MyPivotTable");
                PivotTable pivotTable = pivotTables[pivotIndex];

                pivotTable.AddFieldToArea(PivotFieldType.Column, 0);
                pivotTable.AddFieldToArea(PivotFieldType.Row, 1);
                pivotTable.AddFieldToArea(PivotFieldType.Data, 2);

                int formatIndex = pivotTable.ConditionalFormats.Add();
                PivotConditionalFormat pivotFormat = pivotTable.ConditionalFormats[formatIndex];
                pivotFormat.ScopeType = PivotConditionFormatScopeType.Data;

                PivotArea pivotArea = new PivotArea(pivotTable);
                pivotArea.SelectField(PivotFieldType.Data, pivotTable.DataFields[0]);
                pivotFormat.PivotAreas.Add(pivotArea);

                int conditionIndex = pivotFormat.FormatConditions.AddCondition(
                    FormatConditionType.CellValue, 
                    OperatorType.GreaterThan, 
                    "1", 
                    null);
                pivotFormat.FormatConditions[conditionIndex].Style.BackgroundColor = System.Drawing.ColorTranslator.FromHtml("#e39e9e");

                wb.Save("output.xlsx");
            }
        }
    }
}
```

### Siehe auch

* enum [PivotFieldType](../../pivotfieldtype/)
* class [PivotField](../../pivotfield/)
* class [PivotArea](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


