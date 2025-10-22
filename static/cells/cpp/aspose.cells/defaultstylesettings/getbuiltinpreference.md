##Aspose::Cells::DefaultStyleSettings::GetBuiltInPreference method
'Aspose::Cells::DefaultStyleSettings::GetBuiltInPreference method. Indicates whether property for number format is preferable when the style defines both built-in number and custom pattern. Default value is false, that means by default custom pattern will be used to format values as long as it is not empty for one style in C++.'
## DefaultStyleSettings::GetBuiltInPreference method
Indicates whether property for number format is preferable when the style defines both built-in number and custom pattern. Default value is false, that means by default custom pattern will be used to format values as long as it is not empty for one style.
```cpp
bool Aspose::Cells::DefaultStyleSettings::GetBuiltInPreference()
```
## Remarks
When loading workbook from existing template file, maybe both built-in number and custom pattern are defined for one style. This property determine whether we should use the built-in number or the custom pattern when formatting values with the style.
## See Also
* Class [Vector](../../vector/)
* Class [DefaultStyleSettings](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
