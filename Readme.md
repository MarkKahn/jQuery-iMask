# jQuery iMask Plugin

  A jQuery input masking plugin.

## Including

  Include either `jquery-imask.js` or `jquery-imask-min.js` from the dist directory

## Demos

  http://zyklus.github.com/jQuery-iMask/

## Example

```js
$('#input').iMask({
    type : 'number'
});

$('#input').iMask({
      type : 'fixed'
    , mask : '99/99/99'
})
```

## Options

```
type             (number|fixed)
mask             Mask using 9,a,x notation.  9=Numeric; a=Alpha; x=AlphaNumeric
maskEmptyChr     [ Default = ' ' ]
validNumbers     [ Default = '1234567890' ]
validAlphas      [ Default = 'abcdefghijklmnopqrstuvwxyz' ]
validAlphaNums   [ Default = 'abcdefghijklmnopqrstuvwxyz1234567890' ]
groupDigits      [ Default = 3 ]  # of digits before a numeric seperator ( e.g. "3" yields 1,000,000 )
decDigits        [ Default = 2 ]  # of digits to show after decimal place
currencySymbol
groupSymbol      [ Default = ',' ]
decSymbol        [ Default = '.' ]
showMask         [ Default = true ]  Show mask while editing
stripMask        [ Default = false ] Remove mask when done editing
sanity           Provide a function that acts as a sanity check.
                 return `false` to prevent the keypress, return any other value to replace the pre-masked input value.

number           Override options for when validating numbers only
number.stripMask [ Default = false ]
number.showMask  [ Default = false ]
```

## Events

```
onValid
onInvalid
```


## Features
- Static Masking
   - Mask numbers, letters
   - Customize list of valid numbers & letters
   - Special symbols are displayed but un-selectable
   - Optionally only show the mask while user is entering
- Numeric Masking
    - Control currency symbol, decimal & thousands seperator, # of digits
- Events
    - onValid
    - onInvalid

## Browser Compatibility

  iMask is tested in Chrome, Firefox, Safari & IE.  It should work in any browser.  If there are any issues, please report them.

The core code for the iMask plugin was originally created for MooTools by Fabio Zendhi Nagao (http://zendold.lojcomm.com.br/imask/)
