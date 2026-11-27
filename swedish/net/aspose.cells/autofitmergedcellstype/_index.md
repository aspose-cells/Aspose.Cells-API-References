---
title: "Enum AutoFitMergedCellsType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.AutoFitMergedCellsType‑enum. Representerar typen av automatiskt anpassade sammanslagna celler"
type: docs
url: /sv/net/aspose.cells/autofitmergedcellstype/
---
## AutoFitMergedCellsType enumeration

Representerar typen av automatisk anpassning av sammanslagna celler.

```csharp
public enum AutoFitMergedCellsType
```

### Värden

| Namn | Värde | Beskrivning |
| --- | --- | --- |
| None | `0` | Ignorera sammanslagna celler. |
| FirstLine | `1` | Expanderar endast höjden på den första raden. |
| LastLine | `2` | Expanderar endast höjden på den sista raden. |
| EachLine | `3` | Expanderar höjden på varje rad. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;

    public class AutoFitMergedCellsTypeDemo
    {
        public static void AutoFitMergedCellsTypeExample()
        {
            //Instansierar ett Workbook‑objekt
            Workbook workbook = new Workbook();
            //Hämtar referensen till det nyss tillagda kalkylbladet
            Worksheet sheet1 = workbook.Worksheets[0];

            // Skapa ett område A1:B2
            Range range = sheet1.Cells.CreateRange(0, 0, 2, 2);

            // Sammanfoga cellerna
            range.Merge();

            // Infoga värde i den sammanslagna cellen A1
            sheet1.Cells[0, 0].Value = "This is test text for autofit merged cells type demo This is test text for autofit merged cells type demo";

            // Skapa ett stilobjekt
            Style style = sheet1.Cells[0, 0].GetStyle();

            // Aktivera radbrytning av text
            style.IsTextWrapped = true;

            // Tillämpa stilen på cellen
            sheet1.Cells[0, 0].SetStyle(style);

            // Skapa ett objekt för AutoFitterOptions
            AutoFitterOptions options = new AutoFitterOptions();

            // Expanderar endast höjden på den första raden.
            options.AutoFitMergedCellsType = AutoFitMergedCellsType.FirstLine;

            // Autofit-rader i bladet(inklusive de sammanslagna cellerna)
            sheet1.AutoFitRows(options);


            int index = workbook.Worksheets.Add();
            Worksheet sheet2 = workbook.Worksheets[index];
            sheet2.Name = "Sheet2";
            // Skapa ett område A1:B2
            Range range2 = sheet2.Cells.CreateRange(0, 0, 2, 2);

            // Sammanfoga cellerna
            range2.Merge();

            // Infoga värde i den sammanslagna cellen A1
            sheet2.Cells[0, 0].Value = "This is test text for autofit merged cells type demo This is test text for autofit merged cells type demo";

            // Skapa ett stilobjekt
            Style style2 = sheet2.Cells[0, 0].GetStyle();

            // Aktivera radbrytning av text
            style2.IsTextWrapped = true;

            // Tillämpa stilen på cellen
            sheet2.Cells[0, 0].SetStyle(style);

            // Skapa ett objekt för AutoFitterOptions
            AutoFitterOptions options2 = new AutoFitterOptions();

            // Expanderar endast höjden på den sista raden.
            options2.AutoFitMergedCellsType = AutoFitMergedCellsType.LastLine;

            // Autofit-rader i bladet(inklusive de sammanslagna cellerna)
            sheet2.AutoFitRows(options2);


            index = workbook.Worksheets.Add();
            Worksheet sheet3 = workbook.Worksheets[index];
            sheet3.Name = "Sheet3";
            // Skapa ett område A1:B2
            Range range3 = sheet3.Cells.CreateRange(0, 0, 2, 2);

            // Sammanfoga cellerna
            range3.Merge();

            // Infoga värde i den sammanslagna cellen A1
            sheet3.Cells[0, 0].Value = "This is test text for autofit merged cells type demo This is test text for autofit merged cells type demo";

            // Skapa ett stilobjekt
            Style style3 = sheet3.Cells[0, 0].GetStyle();

            // Aktivera radbrytning av text
            style3.IsTextWrapped = true;

            // Tillämpa stilen på cellen
            sheet3.Cells[0, 0].SetStyle(style);

            // Skapa ett objekt för AutoFitterOptions
            AutoFitterOptions options3 = new AutoFitterOptions();

            // Utökar endast höjden på varje rad.
            options3.AutoFitMergedCellsType = AutoFitMergedCellsType.EachLine;

            // Autofit-rader i bladet(inklusive de sammanslagna cellerna)
            sheet3.AutoFitRows(options3);


            index = workbook.Worksheets.Add();
            Worksheet sheet4 = workbook.Worksheets[index];
            sheet4.Name = "Sheet4";
            // Skapa ett område A1:B2
            Range range4 = sheet4.Cells.CreateRange(0, 0, 2, 2);

            // Sammanfoga cellerna
            range4.Merge();

            // Infoga värde i den sammanslagna cellen A1
            sheet4.Cells[0, 0].Value = "This is test text for autofit merged cells type demo This is test text for autofit merged cells type demo";

            // Skapa ett stilobjekt
            Style style4 = sheet4.Cells[0, 0].GetStyle();

            // Aktivera radbrytning av text
            style4.IsTextWrapped = true;

            // Tillämpa stilen på cellen
            sheet4.Cells[0, 0].SetStyle(style);

            // Skapa ett objekt för AutoFitterOptions
            AutoFitterOptions options4 = new AutoFitterOptions();

            // Ignorera sammanslagna celler.
            options4.AutoFitMergedCellsType = AutoFitMergedCellsType.None;

            // Autofit-rader i bladet(utan de sammanslagna cellerna)
            sheet4.AutoFitRows(options4);

            // Spara arbetsboken
            workbook.Save("AutoFitMergedCellsTypeExample.xlsx");

            return;
        }
    }
}
```

### Se även

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


