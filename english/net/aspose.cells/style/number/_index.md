---
title: Style.Number
second_title: Aspose.Cells for .NET API Reference
description: Style property. Gets or sets the display format of numbers and dates. The formatting patterns are different for different regions
type: docs
url: /net/aspose.cells/style/number/
---
## Style.Number property

Gets or sets the display format of numbers and dates. The formatting patterns are different for different regions.

```csharp
public int Number { get; set; }
```

### Remarks

For example, the formatting patterns represented by numbers for en_US region:

| **Value** | **Type** | **Format String** |
| --- | --- | --- |
| 0 | General | `General` |
| 1 | Decimal | `0` |
| 2 | Decimal | `0.00` |
| 3 | Decimal | `#,##0` |
| 4 | Decimal | `#,##0.00` |
| 5 | Currency | `$#,##0_);($#,##0)` |
| 6 | Currency | `$#,##0_);[Red]($#,##0)` |
| 7 | Currency | `$#,##0.00_);($#,##0.00)` |
| 8 | Currency | `$#,##0.00_);[Red]($#,##0.00)` |
| 9 | Percentage | `0%` |
| 10 | Percentage | `0.00%` |
| 11 | Scientific | `0.00E+00` |
| 12 | Fraction | `# ?/?` |
| 13 | Fraction | `# ??/??` |
| 14 | Date | `m/d/yyyy` |
| 15 | Date | `d-mmm-yy` |
| 16 | Date | `d-mmm` |
| 17 | Date | `mmm-yy` |
| 18 | Time | `h:mm AM/PM` |
| 19 | Time | `h:mm:ss AM/PM` |
| 20 | Time | `h:mm` |
| 21 | Time | `h:mm:ss` |
| 22 | Time | `m/d/yyyy h:mm` |
| 37 | Accounting | `#,##0_);(#,##0)` |
| 38 | Accounting | `#,##0_);[Red](#,##0)` |
| 39 | Accounting | `#,##0.00_);(#,##0.00)` |
| 40 | Accounting | `#,##0.00_);[Red](#,##0.00)` |
| 41 | Accounting | `_(* #,##0_);_(* (#,##0);_(* "-"_);_(@_)` |
| 42 | Currency | `_($* #,##0_);_($* (#,##0);_($* "-"_);_(@_)` |
| 43 | Accounting | `_(* #,##0.00_);_(* (#,##0.00);_(* "-"??_);_(@_)` |
| 44 | Currency | `_($* #,##0.00_);_($* (#,##0.00);_($* "-"??_);_(@_)` |
| 45 | Time | `mm:ss` |
| 46 | Time | `[h]:mm:ss` |
| 47 | Time | `mm:ss.0` |
| 48 | Scientific | `##0.0E+0` |
| 49 | Text | `@` |

### Examples

```csharp
// Called: style.Number = 47;
[Test]
        public void Property_Number()
        {
            caseName = &quot;testNumber_001&quot;;
            Workbook workbook = new Workbook();            
            Cells cells = workbook.Worksheets[0].Cells;

            Cell cell = cells[0, 0];
            cell.PutValue(12);
            Style style = cell.GetStyle();
            style.Number = 0;
            cell.SetStyle(style);            
            testAreEqual(12, cell.IntValue, caseName);

            cell = cells[1, 0];
            cell.PutValue(12);
            style = cell.GetStyle();
            style.Number = 1;
            cell.SetStyle(style);
            testAreEqual(12, cell.IntValue, caseName);

            cell = cells[2, 0];
            cell.PutValue(12);
            style = cell.GetStyle();
            style.Number = 2;
            cell.SetStyle(style);

            cell = cells[3, 0];
            cell.PutValue(12);
            style = cell.GetStyle();
            style.Number = 3;
            cell.SetStyle(style);

            cell = cells[4, 0];
            cell.PutValue(12);
            style = cell.GetStyle();
            style.Number = 4;
            cell.SetStyle(style);

            cell = cells[5, 0];
            cell.PutValue(12);
            style = cell.GetStyle();
            style.Number = 5;
            cell.SetStyle(style);

            cell = cells[6, 0];
            cell.PutValue(12);
            style = cells[6, 0].GetStyle();
            style.Number = 6;
            cells[6, 0].SetStyle(style);

            style = cells[7, 0].GetStyle();
            style.Number = 7;
            cells[7, 0].SetStyle(style);

            style = cells[8, 0].GetStyle();
            style.Number = 8;
            cells[8, 0].SetStyle(style);

            style = cells[9, 0].GetStyle();
            style.Number = 9;
            cells[9, 0].SetStyle(style);

            style = cells[10, 0].GetStyle();
            style.Number = 10;
            cells[10, 0].SetStyle(style);

            style = cells[11, 0].GetStyle();
            style.Number = 11;
            cells[11, 0].SetStyle(style);

            style = cells[12, 0].GetStyle();
            style.Number = 12;
            cells[12, 0].SetStyle(style);

            style = cells[13, 0].GetStyle();
            style.Number = 13;
            cells[13, 0].SetStyle(style);

            style = cells[14, 0].GetStyle();
            style.Number = 14;
            cells[14, 0].SetStyle(style);

            style = cells[15, 0].GetStyle();
            style.Number = 15;
            cells[15, 0].SetStyle(style);            

            style = cells[16, 0].GetStyle();
            style.Number = 16;
            cells[16, 0].SetStyle(style);           

            style = cells[17, 0].GetStyle();
            style.Number = 17;
            cells[17, 0].SetStyle(style);            

            style = cells[18, 0].GetStyle();
            style.Number = 18;
            cells[18, 0].SetStyle(style);            

            style = cells[19, 0].GetStyle();
            style.Number = 19;
            cells[19, 0].SetStyle(style);            

            style = cells[20, 0].GetStyle();
            style.Number = 20;
            cells[20, 0].SetStyle(style);
            

            style = cells[21, 0].GetStyle();
            style.Number = 21;
            cells[21, 0].SetStyle(style);            

            style = cells[22, 0].GetStyle();
            style.Number = 22;
            cells[22, 0].SetStyle(style);            

            style = cells[23, 0].GetStyle();
            style.Number = 37;
            cells[23, 0].SetStyle(style);          

            style = cells[24, 0].GetStyle();
            style.Number = 38;
            cells[24, 0].SetStyle(style);
            
            style = cells[25, 0].GetStyle();
            style.Number = 39;
            cells[25, 0].SetStyle(style);            

            style = cells[26, 0].GetStyle();
            style.Number = 40;
            cells[26, 0].SetStyle(style);            

            style = cells[27, 0].GetStyle();
            style.Number = 41;
            cells[27, 0].SetStyle(style);           

            style = cells[28, 0].GetStyle();
            style.Number = 42;
            cells[28, 0].SetStyle(style);            

            style = cells[29, 0].GetStyle();
            style.Number = 43;
            cells[29, 0].SetStyle(style);            

            style = cells[30, 0].GetStyle();
            style.Number = 44;
            cells[30, 0].SetStyle(style);            

            style = cells[31, 0].GetStyle();
            style.Number = 45;
            cells[31, 0].SetStyle(style);            

            style = cells[32, 0].GetStyle();
            style.Number = 46;
            cells[32, 0].SetStyle(style);            

            style = cells[33, 0].GetStyle();
            style.Number = 47;
            cells[33, 0].SetStyle(style);            

            style = cells[34, 0].GetStyle();
            style.Number = 48;
            cells[34, 0].SetStyle(style);            

            style = cells[35, 0].GetStyle();
            style.Number = 49;
            cells[35, 0].SetStyle(style);       
     
            checkNumber_001(workbook);
            workbook.Save(Constants.destPath + &quot;testNumber.xls&quot;);            
            workbook = new Workbook(Constants.destPath + &quot;testNumber.xls&quot;);
            checkNumber_001(workbook);
            workbook.Save(Constants.destPath + &quot;testNumber.xlsx&quot;);            
            workbook = new Workbook(Constants.destPath + &quot;testNumber.xlsx&quot;);
            checkNumber_001(workbook);
            workbook.Save(Constants.destPath + &quot;testNumber.xml&quot;, SaveFormat.SpreadsheetML );            
            workbook = new Workbook(Constants.destPath + &quot;testNumber.xml&quot;);
         //   checkNumber_001(workbook);
            workbook.Save(Constants.destPath + &quot;testNumber.xls&quot;);
        }
```

### See Also

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


