---
title: "Enum AutoFitMergedCellsType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.AutoFitMergedCellsType-Enum. Stellt den Typ des automatischen Anpassens zusammengeführter Zellen dar"
type: docs
url: /de/net/aspose.cells/autofitmergedcellstype/
---
## AutoFitMergedCellsType enumeration

Stellt den Typ des automatischen Anpassens zusammengeführter Zellen dar.

```csharp
public enum AutoFitMergedCellsType
```

### Werte

| Name | Wert | Beschreibung |
| --- | --- | --- |
| None | `0` | Zusammengeführte Zellen ignorieren. |
| FirstLine | `1` | Erweitert nur die Höhe der ersten Zeile. |
| LastLine | `2` | Erweitert nur die Höhe der letzten Zeile. |
| EachLine | `3` | Erweitert die Höhe jeder Zeile. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;

    public class AutoFitMergedCellsTypeDemo
    {
        public static void AutoFitMergedCellsTypeExample()
        {
            //Instanziieren eines Workbook-Objekts
            Workbook workbook = new Workbook();
            //Abrufen der Referenz des neu hinzugefügten Arbeitsblatts
            Worksheet sheet1 = workbook.Worksheets[0];

            // Erstelle einen Bereich A1:B2
            Range range = sheet1.Cells.CreateRange(0, 0, 2, 2);

            // Zellen zusammenführen
            range.Merge();

            // Wert in die zusammengeführte Zelle A1 einfügen
            sheet1.Cells[0, 0].Value = "This is test text for autofit merged cells type demo This is test text for autofit merged cells type demo";

            // Erstellen Sie ein Stilobjekt
            Style style = sheet1.Cells[0, 0].GetStyle();

            // Zeilenumbruch aktivieren
            style.IsTextWrapped = true;

            // Wenden Sie den Stil auf die Zelle an
            sheet1.Cells[0, 0].SetStyle(style);

            // Ein Objekt für AutoFitterOptions erstellen
            AutoFitterOptions options = new AutoFitterOptions();

            // Erweitert nur die Höhe der ersten Zeile.
            options.AutoFitMergedCellsType = AutoFitMergedCellsType.FirstLine;

            // Zeilen im Blatt automatisch anpassen (einschließlich der zusammengeführten Zellen)
            sheet1.AutoFitRows(options);


            int index = workbook.Worksheets.Add();
            Worksheet sheet2 = workbook.Worksheets[index];
            sheet2.Name = "Sheet2";
            // Erstelle einen Bereich A1:B2
            Range range2 = sheet2.Cells.CreateRange(0, 0, 2, 2);

            // Zellen zusammenführen
            range2.Merge();

            // Wert in die zusammengeführte Zelle A1 einfügen
            sheet2.Cells[0, 0].Value = "This is test text for autofit merged cells type demo This is test text for autofit merged cells type demo";

            // Erstellen Sie ein Stilobjekt
            Style style2 = sheet2.Cells[0, 0].GetStyle();

            // Zeilenumbruch aktivieren
            style2.IsTextWrapped = true;

            // Wenden Sie den Stil auf die Zelle an
            sheet2.Cells[0, 0].SetStyle(style);

            // Ein Objekt für AutoFitterOptions erstellen
            AutoFitterOptions options2 = new AutoFitterOptions();

            // Erweitert nur die Höhe der letzten Zeile.
            options2.AutoFitMergedCellsType = AutoFitMergedCellsType.LastLine;

            // Zeilen im Blatt automatisch anpassen (einschließlich der zusammengeführten Zellen)
            sheet2.AutoFitRows(options2);


            index = workbook.Worksheets.Add();
            Worksheet sheet3 = workbook.Worksheets[index];
            sheet3.Name = "Sheet3";
            // Erstelle einen Bereich A1:B2
            Range range3 = sheet3.Cells.CreateRange(0, 0, 2, 2);

            // Zellen zusammenführen
            range3.Merge();

            // Wert in die zusammengeführte Zelle A1 einfügen
            sheet3.Cells[0, 0].Value = "This is test text for autofit merged cells type demo This is test text for autofit merged cells type demo";

            // Erstellen Sie ein Stilobjekt
            Style style3 = sheet3.Cells[0, 0].GetStyle();

            // Zeilenumbruch aktivieren
            style3.IsTextWrapped = true;

            // Wenden Sie den Stil auf die Zelle an
            sheet3.Cells[0, 0].SetStyle(style);

            // Ein Objekt für AutoFitterOptions erstellen
            AutoFitterOptions options3 = new AutoFitterOptions();

            // Erweitert nur die Höhe jeder Zeile.
            options3.AutoFitMergedCellsType = AutoFitMergedCellsType.EachLine;

            // Zeilen im Blatt automatisch anpassen (einschließlich der zusammengeführten Zellen)
            sheet3.AutoFitRows(options3);


            index = workbook.Worksheets.Add();
            Worksheet sheet4 = workbook.Worksheets[index];
            sheet4.Name = "Sheet4";
            // Erstelle einen Bereich A1:B2
            Range range4 = sheet4.Cells.CreateRange(0, 0, 2, 2);

            // Zellen zusammenführen
            range4.Merge();

            // Wert in die zusammengeführte Zelle A1 einfügen
            sheet4.Cells[0, 0].Value = "This is test text for autofit merged cells type demo This is test text for autofit merged cells type demo";

            // Erstellen Sie ein Stilobjekt
            Style style4 = sheet4.Cells[0, 0].GetStyle();

            // Zeilenumbruch aktivieren
            style4.IsTextWrapped = true;

            // Wenden Sie den Stil auf die Zelle an
            sheet4.Cells[0, 0].SetStyle(style);

            // Ein Objekt für AutoFitterOptions erstellen
            AutoFitterOptions options4 = new AutoFitterOptions();

            // Zusammengeführte Zellen ignorieren.
            options4.AutoFitMergedCellsType = AutoFitMergedCellsType.None;

            // Zeilen im Blatt automatisch anpassen (ohne die zusammengeführten Zellen)
            sheet4.AutoFitRows(options4);

            // Speichere die Arbeitsmappe
            workbook.Save("AutoFitMergedCellsTypeExample.xlsx");

            return;
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


