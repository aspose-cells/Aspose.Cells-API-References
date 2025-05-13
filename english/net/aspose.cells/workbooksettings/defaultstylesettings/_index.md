---
title: WorkbookSettings.DefaultStyleSettings
second_title: Aspose.Cells for .NET API Reference
description: WorkbookSettings property. Gets the settings for default values of stylerelated properties for this workbook
type: docs
url: /net/aspose.cells/workbooksettings/defaultstylesettings/
---
## WorkbookSettings.DefaultStyleSettings property

Gets the settings for default values of style-related properties for this workbook.

```csharp
public DefaultStyleSettings DefaultStyleSettings { get; }
```

### Examples

```csharp
// Called: wb.Settings.DefaultStyleSettings.BuiltInPreference = true;
public void WorkbookSettings_Property_DefaultStyleSettings()
{
    //CELLSNET-53482
    //en-CA: CELLSNET-55529
    string ptn = "BuiltInFormat_";
    string[] files = Directory.GetFiles(Constants.sourcePath + "Style", ptn + "*.xlsx");
    if (files == null || files.Length < 1)
    {
        Assert.Fail("Cannot find template files " + ptn + "*.xlsx");
    }
    StringBuilder sb = null;
    foreach (string path in files)
    {
        int v = path.IndexOf(ptn);
        Console.Write("FormattingTest.LocaleBuiltIn: " + path.Substring(v) + "...");
        if (v < 0)
        {
            Console.WriteLine("Ignored");
            continue;
        }
        Workbook wb = new Workbook(path);
        wb.Settings.DefaultStyleSettings.BuiltInPreference = true;
        v += ptn.Length;
        bool addFile = true;
        string cn = path.Substring(v, path.Length - 5 - v).Replace('_', '-');
        try
        {
            wb.Settings.CultureInfo = new CultureInfo(cn);
        }
        catch (Exception e)
        {
            if (sb == null)
            {
                sb = new StringBuilder(1024);
            }
            else
            {
                sb.Append('\n');
            }
            sb.Append(path);
            sb.Append("\n  Failed to set CultureInfo: ");
            sb.Append(cn);
            sb.Append("; ");
            Util.GetExceptoinInfo(e, sb);
            addFile = false;
            continue;
        }
        Cells cells = wb.Worksheets[0].Cells;
        v = cells.MaxDataRow;
        for (int i = 0; i <= v; i++)
        {
            for (int j = 0; j < 6; j += 3)
            {
                Cell c = cells.CheckCell(i, j + 2);
                if (c != null && c.StringValue == "x")
                {
                    continue;
                }
                string d = cells[i, j].StringValue;
                string s = cells[i, j + 1].StringValue;
                if (d != s && !s.StartsWith("###"))
                {
                    if (addFile)
                    {
                        if (sb == null)
                        {
                            sb = new StringBuilder(1024);
                        }
                        else
                        {
                            sb.Append('\n');
                        }
                        sb.Append(path);
                        addFile = false;
                    }
                    sb.Append("\n  ");
                    sb.Append((char)('A' + j));
                    sb.Append(i + 1);
                    sb.Append("(Style.Number=");
                    sb.Append(cells[i, 0].GetStyle(false).Number);
                    sb.Append("): expected [");
                    sb.Append(s);
                    sb.Append("] but was [");
                    sb.Append(d);
                    sb.Append(']');
                }
            }
        }
        Console.WriteLine("Finished");
    }
    if (sb != null)
    {
        Assert.Fail(sb.ToString());
    }
}
```

### See Also

* class [DefaultStyleSettings](../../defaultstylesettings/)
* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


