---
title: PivotItem.IsHidden
second_title: Aspose.Cells for .NET API Reference
description: PivotItem property. Gets and Sets whether the pivot item is hidden
type: docs
url: /net/aspose.cells.pivot/pivotitem/ishidden/
---
## PivotItem.IsHidden property

Gets and Sets whether the pivot item is hidden.

```csharp
public bool IsHidden { get; set; }
```

### Examples

```csharp
// Called: _Ret += &amp;quot;Name: &amp;quot; + _PivotItem.Name + &amp;quot; - Hidden: &amp;quot; + _PivotItem.IsHidden.ToString() + Environment.NewLine;
public static void Property_IsHidden(ref Aspose.Cells.Worksheet _sheetActiva,
                                                ref PivotTable _PivotTable,
                                                ref PivotField _PivotField,
                                                List&lt;string&gt; _lstStrValue,
                                                bool _bolKeySensitive = false,
                                                bool _bolRefreshData = true)
        {
            bool _bolOcultarBlancos = false; //SC: Ya hay otra ffunción para ocultar los blancos, no hace falta
            _PivotField.IsMultipleItemSelectionAllowed = true;
            //PivotItemCollection items = _PivotField.PivotItems;
            PivotItem _PivotItem;
            string _strItemActualPivotField;
            //foreach (string _strValue in _lstStrValue)
            //{

            //foreach (string item in items) //NF: No co ntiene Interface getenumrator
            //{            
            //}

            //_PivotTable.RefreshData();
            //_PivotTable.CalculateData();

            for (int i = 0; i &lt; _PivotField.PivotItems.Count; i++)
            {
                _PivotItem = _PivotField.PivotItems[i];
                _strItemActualPivotField = (_PivotItem.Value == null ? &quot;&quot; : _PivotItem.Value.ToString());

                if (_bolOcultarBlancos &amp;&amp; string.IsNullOrWhiteSpace(_strItemActualPivotField)) //Si es el valor blank
                {
                    _PivotItem.IsHidden = true;  //Ocultarlo
                }
                else if (!_lstStrValue.Contains(_strItemActualPivotField))
                {
                    //Chapuza (no encontré otra y XG ya está nervioso). Si solo viene uno y es todos o all no filtrar pq. sino no muestra nada en el Excel 
                    if (_lstStrValue.Count == 1 &amp;&amp; GetEsValorTodosNET44514(_lstStrValue[0])) { /*Nada*/}
                    else
                    {
                        _PivotItem.IsHidden = true;
                        //if (_PivotItem.Name == @&quot;2015/16&quot;) { /*_PivotItemTest = _PivotItem; */ var aa = 1; }
                    }
                }
            }
            //}

            //ALERT!!! BUG
            string _strOK = GetCheckValuePivotFieldNET44514(ref _sheetActiva);

            string _Ret = &quot;--------&quot; + _PivotField.Name + Environment.NewLine;

            for (int i = 0; i &lt; _PivotField.PivotItems.Count; i++)
            {
                _PivotItem = _PivotField.PivotItems[i];
                _strItemActualPivotField = (_PivotItem.Value == null ? &quot;&quot; : _PivotItem.Value.ToString());

                _Ret += &quot;Name: &quot; + _PivotItem.Name + &quot; - Hidden: &quot; + _PivotItem.IsHidden.ToString() + Environment.NewLine;
            }
            //Console.WriteLine(_Ret);

            if (_bolRefreshData)
            {
                _PivotTable.RefreshData(); //SC: Bug! en cuanto hago esto UtilAspose.GetCheckValuePivotField(ref _sheetActiva) no vale igual q antes y debería
                _PivotTable.CalculateData();
            }

            string _strKO = GetCheckValuePivotFieldNET44514(ref _sheetActiva);

            Console.WriteLine(&quot;==============================&quot;);
            string _Ret2 = &quot;--------&quot; + _PivotField.Name + Environment.NewLine;

            for (int i = 0; i &lt; _PivotField.PivotItems.Count; i++)
            {
                _PivotItem = _PivotField.PivotItems[i];
                _strItemActualPivotField = (_PivotItem.Value == null ? &quot;&quot; : _PivotItem.Value.ToString());

                _Ret2 += &quot;Name: &quot; + _PivotItem.Name + &quot; - Hidden: &quot; + _PivotItem.IsHidden.ToString() + Environment.NewLine;
            }
            //Console.WriteLine(_Ret2);
            Assert.AreEqual(_Ret, _Ret2);
        }
```

### See Also

* class [PivotItem](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


