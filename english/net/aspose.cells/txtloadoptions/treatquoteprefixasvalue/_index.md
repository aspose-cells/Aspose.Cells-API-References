---
title: TxtLoadOptions.TreatQuotePrefixAsValue
second_title: Aspose.Cells for .NET API Reference
description: TxtLoadOptions property. Indicates whether the leading single quote sign should be taken as part of the value of one cell. Default is true. If it is false the leading single quote will be removed from corresponding cells value and QuotePrefix will be set as true for the cell
type: docs
url: /net/aspose.cells/txtloadoptions/treatquoteprefixasvalue/
---
## TxtLoadOptions.TreatQuotePrefixAsValue property

Indicates whether the leading single quote sign should be taken as part of the value of one cell. Default is true. If it is false, the leading single quote will be removed from corresponding cell's value and [`QuotePrefix`](../../style/quoteprefix/) will be set as true for the cell.

```csharp
public bool TreatQuotePrefixAsValue { get; set; }
```

### Examples

```csharp
// Called: tlo.TreatQuotePrefixAsValue = !tso.ExportQuotePrefix;
private void TxtLoadOptions_Property_TreatQuotePrefixAsValue(Workbook wb, TxtSaveOptions tso, string csvTxt)
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
            TxtLoadOptions_Property_TreatQuotePrefixAsValue(wb, tso, tlo, csvTxt);
        }
```

### See Also

* class [TxtLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


