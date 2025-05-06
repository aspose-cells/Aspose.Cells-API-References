---
title: AbstractTextLoadOptions.Encoding
second_title: Aspose.Cells for .NET API Reference
description: AbstractTextLoadOptions property. Gets and sets the default encoding. Only applies for csv file
type: docs
url: /net/aspose.cells/abstracttextloadoptions/encoding/
---
## AbstractTextLoadOptions.Encoding property

Gets and sets the default encoding. Only applies for csv file.

```csharp
public Encoding Encoding { get; set; }
```

### Examples

```csharp
// Called: tlo.Encoding = tso.Encoding;
private void Property_Encoding(Workbook wb, TxtSaveOptions tso, string csvTxt)
        {
            TxtLoadOptions tlo = new TxtLoadOptions();
            if (tso.SeparatorString != null)
            {
                tlo.SeparatorString = tso.SeparatorString;
            }
            else
            {
                tlo.Separator = tso.Separator;
            }
            tlo.Encoding = tso.Encoding;
            tlo.TreatQuotePrefixAsValue = !tso.ExportQuotePrefix;
            Property_Encoding(wb, tso, tlo, csvTxt);
        }
```

### See Also

* class [AbstractTextLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


