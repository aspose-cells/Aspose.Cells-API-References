---
title: FontSetting.TextOptions
second_title: Aspose.Cells for .NET API Reference
description: FontSetting property. Returns the text options
type: docs
url: /net/aspose.cells/fontsetting/textoptions/
---
## FontSetting.TextOptions property

Returns the text options.

```csharp
public TextOptions TextOptions { get; }
```

### Examples

```csharp
// Called: _cell.Characters(s2, _STR_4.Length).TextOptions.IsBold = true;
[Test]
        public void Property_TextOptions()
        {
            Workbook wb = new Workbook();

            var _cell = wb.Worksheets["Sheet1"].Cells[13, 1];

            var _STR_1 = "　お客さまにお支払いいただきました水道料金等について，重複納付による過誤納金が発生しましたので，次のとおり充当させていただきます。" + Environment.NewLine;
            var _STR_2_1 = "　充当後の差引額は，今後，新たに発生する";
            var _STR_2_2 = "令和99年99.99" + "月分";
            var _STR_2_3 = "に充当させていただきます。" + Environment.NewLine;
            var _STR_3 = "　また，充当後に差額が発生する場合は，納付書を送付いたしますので，お支払いをお願いいたします。" + Environment.NewLine;
            var _STR_4 = "　なお，以前送付しました下記【充当先の明細】にある納付書については，廃棄いただきますようお願いいたします。" + Environment.NewLine;
            var _STR_5 = "　ご不明な点などがございましたら，下記までご連絡ください。";
            string str = _STR_1 + _STR_2_1 + _STR_2_2 + _STR_2_3 + _STR_3 + _STR_4 + _STR_5;
            int s1 = (_STR_1.Length + _STR_2_1.Length);

            int s2 = (_STR_1.Length + _STR_2_1.Length + _STR_2_2.Length + +_STR_2_3.Length + +_STR_3.Length);

            _cell.Value = _STR_1 + _STR_2_1 + _STR_2_2 + _STR_2_3 + _STR_3 + _STR_4 + _STR_5;

            _cell.Characters(s1, _STR_2_2.Length).TextOptions.IsBold = true;
            _cell.Characters(s1, _STR_2_2.Length).TextOptions.IsItalic = true;
            _cell.Characters(s2, _STR_4.Length).TextOptions.IsBold = true;
            _cell.Characters(s2, _STR_4.Length).TextOptions.IsItalic = true;
            wb = Util.ReSave(wb, SaveFormat.Xlsx);
            Assert.IsFalse(_cell.Characters(s1 - 1, _STR_2_2.Length).TextOptions.IsBold);
            Assert.IsTrue(_cell.Characters(s1, _STR_2_2.Length).TextOptions.IsBold);
        }
```

### See Also

* class [TextOptions](../../../aspose.cells.drawing.texts/textoptions/)
* class [FontSetting](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


