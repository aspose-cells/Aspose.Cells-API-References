---
title: PivotTable.ClearData
second_title: Aspose.Cells for .NET API Reference
description: PivotTable method. Clear PivotTables data and formatting
type: docs
url: /net/aspose.cells.pivot/pivottable/cleardata/
---
## PivotTable.ClearData method

Clear PivotTable's data and formatting

```csharp
public void ClearData()
```

### Remarks

If this method is not called before you add or delete PivotField, Maybe the PivotTable data is not corrected

### Examples

```csharp
// Called: ptable.ClearData();
private void Method_ClearData(string filePath, string filename, SaveFormat format)
        {
            string[] osNames = new string[5];
            osNames[0] = "Windows";
            osNames[1] = "Solaris";
            osNames[2] = "Ubuntu";
            osNames[3] = "OSX";
            osNames[4] = "Fedora";

            string[] moduleNames = new string[3];
            for (int i = 0; i < 3; i++)
                moduleNames[i] = RandomString(5) + " " + RandomString(10);


            DataTable data = new DataTable();
            data.Columns.Add(new DataColumn("Vulnerability"));
            data.Columns.Add(new DataColumn("Module Name"));
            data.Columns.Add(new DataColumn("Entity Name"));
            data.Columns.Add(new DataColumn("CVSS Score"));
            data.Columns.Add(new DataColumn("OS Name"));
            data.Columns.Add(new DataColumn("OS Version"));

            Random rand = new Random();

            for (int i = 0; i < 100; i++)
            {
                int randNumber = rand.Next(100, 300);
                int randCVSS = rand.Next(1, 10);
                int randIp = rand.Next(2, 20);
                int randVersion = rand.Next(1, 10);
                int randOSName = rand.Next(0, 5);
                int randModuleName = rand.Next(0, 3);
                DataRow row = data.NewRow();

                row["Vulnerability"] = "CVE-2013-" + randNumber.ToString();
                row["Module Name"] = moduleNames[randModuleName];
                row["Entity Name"] = "/192.168.22." + randIp.ToString();
                row["CVSS Score"] = randCVSS;
                row["OS Name"] = osNames[randOSName];
                row["OS Version"] = randVersion;

                data.Rows.Add(row);
            }


            Workbook wb_b = new Workbook(filePath + @"test.xlsx");

            Cells cellsp = wb_b.Worksheets["Most Exploited Vulns"].Cells;
            cellsp["C24"].Formula = "=SUM(C29:C39)";
            wb_b.CalculateFormula();
            string prefixStr = cellsp["C24"].StringValue;

            Worksheet sheet = wb_b.Worksheets["_mev_data"];

            sheet.ListObjects["tbl_host_vulns_info"].Resize(0, 0, 100, 5, true);
            sheet.Cells.ClearContents(1, 1, 13, 6);

            sheet.Cells.ImportData(data, 1, 0, new ImportTableOptions()
            {
                IsFieldNameShown = false,
                InsertRows = false,
                ConvertNumericData = true,
                TotalRows = 100,
                TotalColumns = 6,
                DateFormat = "mm/dd/yy hh:mm AM/PM"
            });

            foreach (PivotTable ptable in sheet.PivotTables)
            {
                ptable.ClearData();

                string[] ds = new string[1];
                ds[0] = "_mev_data!A1:F101";
                ptable.ChangeDataSource(ds);

                ptable.CalculateRange();

                ptable.RefreshData();
                ptable.CalculateData();
            }

            sheet = wb_b.Worksheets["Most Exploited Vulns"];
            foreach (PivotTable ptable in sheet.PivotTables)
            {
                ptable.RefreshData();
                ptable.CalculateData();
            }

            foreach (Chart c in sheet.Charts)
            {
                c.Calculate();
                c.RefreshPivotData();
            }

            if (format.Equals(SaveFormat.Pdf))
            {
                PdfSaveOptions opts = new PdfSaveOptions();
                //opts.RefreshChartCache = true;
                opts.AllColumnsInOnePagePerSheet = true;
                filename += ".pdf";
                wb_b.Save(Constants.PivotTableDestPath + @"NET43744_" + filename, opts);
                wb_b.Save(Constants.PivotTableDestPath + @"NET43744_" + "outputpdf.xlsx");

                Cells cells = wb_b.Worksheets["Most Exploited Vulns"].Cells;
                cells["C24"].Formula = "=SUM(C29:C39)";
                wb_b.CalculateFormula();
                Console.WriteLine(cells["C24"].StringValue + "   " + prefixStr);
                Assert.AreNotEqual(cells["C24"].StringValue, prefixStr);
            }
            else
            {
                filename += ".xlsx";
                wb_b.Save(Constants.PivotTableDestPath + @"NET43744_" + filename);
            }

        }
```

### See Also

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


