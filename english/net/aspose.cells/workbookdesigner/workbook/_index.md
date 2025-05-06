---
title: WorkbookDesigner.Workbook
second_title: Aspose.Cells for .NET API Reference
description: WorkbookDesigner property. Gets and sets the Workbook object
type: docs
url: /net/aspose.cells/workbookdesigner/workbook/
---
## WorkbookDesigner.Workbook property

Gets and sets the `Workbook` object.

```csharp
public Workbook Workbook { get; set; }
```

### Examples

```csharp
// Called: workbookDesigner.Workbook.Save(outfn);
[Test]
        // http://www.aspose.com/community/forums/thread/280643.aspx
        // set license very slow
        public void Property_Workbook()
        {
            Console.WriteLine(&quot;Property_Workbook()&quot;);
            string infn = path + @&quot;LicSlow/TestExcelTemplateSheet.xlsx&quot;;
            string outfn = Constants.destPath + @&quot;TestExcelTemplateSheet_out.xlsx&quot;;

            DateTime startDate = DateTime.Now;
            Console.WriteLine(&quot;Start date: &quot; + startDate.ToString());

            //string _templateLocation = @&quot;D:\Mydocs\Aspose\Aspose_Cells\Aspose.Cells.lic&quot;;
            //using (Stream licenseStream = File.OpenRead(_templateLocation))
            //{
            //    if (licenseStream == null)
            //    {
            //        throw new Exception(&quot;Can not find licence file in &apos;&quot; + _templateLocation + &quot;&apos; location.&quot;);
            //    }
            //    License _license = new License();
            //    _license.SetLicense(licenseStream);
            //}

            WorkbookDesigner workbookDesigner = new WorkbookDesigner();
            workbookDesigner.Workbook = new Workbook(new MemoryStream(File.ReadAllBytes(infn)));

            workbookDesigner.Workbook.Save(outfn);

            DateTime endDate = DateTime.Now;
            Console.WriteLine(&quot;End date: &quot; + endDate.ToString());

            Console.WriteLine(&quot;All Done - &quot; + endDate.Subtract(startDate).ToString());
        }
```

### See Also

* class [Workbook](../../workbook/)
* class [WorkbookDesigner](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


