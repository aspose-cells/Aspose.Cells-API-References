---
title: PaginatedSaveOptions.AllColumnsInOnePagePerSheet
second_title: Aspose.Cells for .NET API Reference
description: PaginatedSaveOptions property. If AllColumnsInOnePagePerSheet is true  all column content of one sheet will output to only one page in result. The width of paper size of pagesetup will be ignored and the other settings of pagesetup will still take effect
type: docs
url: /net/aspose.cells/paginatedsaveoptions/allcolumnsinonepagepersheet/
---
## PaginatedSaveOptions.AllColumnsInOnePagePerSheet property

If AllColumnsInOnePagePerSheet is true , all column content of one sheet will output to only one page in result. The width of paper size of pagesetup will be ignored, and the other settings of pagesetup will still take effect.

```csharp
public bool AllColumnsInOnePagePerSheet { get; set; }
```

### Examples

```csharp
// Called: opts.AllColumnsInOnePagePerSheet = true;
private void Property_AllColumnsInOnePagePerSheet(string filePath, string filename, SaveFormat format)
        {
            string[] osNames = new string[5];
            osNames[0] = &quot;Windows&quot;;
            osNames[1] = &quot;Solaris&quot;;
            osNames[2] = &quot;Ubuntu&quot;;
            osNames[3] = &quot;OSX&quot;;
            osNames[4] = &quot;Fedora&quot;;

            string[] moduleNames = new string[3];
            for (int i = 0; i &lt; 3; i++)
                moduleNames[i] = RandomString(5) + &quot; &quot; + RandomString(10);


            DataTable data = new DataTable();
            data.Columns.Add(new DataColumn(&quot;Vulnerability&quot;));
            data.Columns.Add(new DataColumn(&quot;Module Name&quot;));
            data.Columns.Add(new DataColumn(&quot;Entity Name&quot;));
            data.Columns.Add(new DataColumn(&quot;CVSS Score&quot;));
            data.Columns.Add(new DataColumn(&quot;OS Name&quot;));
            data.Columns.Add(new DataColumn(&quot;OS Version&quot;));

            Random rand = new Random();

            for (int i = 0; i &lt; 100; i++)
            {
                int randNumber = rand.Next(100, 300);
                int randCVSS = rand.Next(1, 10);
                int randIp = rand.Next(2, 20);
                int randVersion = rand.Next(1, 10);
                int randOSName = rand.Next(0, 5);
                int randModuleName = rand.Next(0, 3);
                DataRow row = data.NewRow();

                row[&quot;Vulnerability&quot;] = &quot;CVE-2013-&quot; + randNumber.ToString();
                row[&quot;Module Name&quot;] = moduleNames[randModuleName];
                row[&quot;Entity Name&quot;] = &quot;/192.168.22.&quot; + randIp.ToString();
                row[&quot;CVSS Score&quot;] = randCVSS;
                row[&quot;OS Name&quot;] = osNames[randOSName];
                row[&quot;OS Version&quot;] = randVersion;

                data.Rows.Add(row);
            }


            Workbook wb_b = new Workbook(filePath + @&quot;test.xlsx&quot;);

            Cells cellsp = wb_b.Worksheets[&quot;Most Exploited Vulns&quot;].Cells;
            cellsp[&quot;C24&quot;].Formula = &quot;=SUM(C29:C39)&quot;;
            wb_b.CalculateFormula();
            string prefixStr = cellsp[&quot;C24&quot;].StringValue;

            Worksheet sheet = wb_b.Worksheets[&quot;_mev_data&quot;];

            sheet.ListObjects[&quot;tbl_host_vulns_info&quot;].Resize(0, 0, 100, 5, true);
            sheet.Cells.ClearContents(1, 1, 13, 6);

            sheet.Cells.ImportData(data, 1, 0, new ImportTableOptions()
            {
                IsFieldNameShown = false,
                InsertRows = false,
                ConvertNumericData = true,
                TotalRows = 100,
                TotalColumns = 6,
                DateFormat = &quot;mm/dd/yy hh:mm AM/PM&quot;
            });

            foreach (PivotTable ptable in sheet.PivotTables)
            {
                ptable.ClearData();

                string[] ds = new string[1];
                ds[0] = &quot;_mev_data!A1:F101&quot;;
                ptable.ChangeDataSource(ds);

                ptable.CalculateRange();

                ptable.RefreshData();
                ptable.CalculateData();
            }

            sheet = wb_b.Worksheets[&quot;Most Exploited Vulns&quot;];
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
                filename += &quot;.pdf&quot;;
                wb_b.Save(Constants.PivotTableDestPath + @&quot;NET43744_&quot; + filename, opts);
                wb_b.Save(Constants.PivotTableDestPath + @&quot;NET43744_&quot; + &quot;outputpdf.xlsx&quot;);

                Cells cells = wb_b.Worksheets[&quot;Most Exploited Vulns&quot;].Cells;
                cells[&quot;C24&quot;].Formula = &quot;=SUM(C29:C39)&quot;;
                wb_b.CalculateFormula();
                Console.WriteLine(cells[&quot;C24&quot;].StringValue + &quot;   &quot; + prefixStr);
                Assert.AreNotEqual(cells[&quot;C24&quot;].StringValue, prefixStr);
            }
            else
            {
                filename += &quot;.xlsx&quot;;
                wb_b.Save(Constants.PivotTableDestPath + @&quot;NET43744_&quot; + filename);
            }

        }
```

### See Also

* class [PaginatedSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


