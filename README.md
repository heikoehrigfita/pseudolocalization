# pseudolocalization

The task is to transform a localization file to another.

The structure of the source file contains key-value pairs is as follows:

```
shoes.type.categories.w.loafers = Loafers
shoes.type.categories.w.pumps = Pumps
shoes.type.categories.w.sneakers = Sneakers
shoes.type.categories.w.other = Other
shoes.type.categories.w.snow\ boots = Snow boots
shoes.type.categories.w.sandals = Sandals
results.info_primary = <p>This recommendation is based on the size that <b>people like you</b> bought, and whether they returned it.</p><p>Based on the purchases of over {{noOfShoppers}} similar shoppers, there is <b>a <span class='uclw_percentage_span'>{{{percentage}}}</span> chance</b> that you will be happy with <span class='uclw_nowrap'>size {{size}}</span>.</p>
```

## Task

Create a new file so that the key-value structure persist but the values are translated two a pseudo-language:
``` 
shoes.type.categories.m.loafers = Ŀǿǿȧȧƒḗḗřş
shoes.type.categories.m.oxfords = ǾǾẋƒǿǿřḓş
shoes.type.categories.m.sneakers = Şƞḗḗȧȧķḗḗřş
shoes.type.categories.m.other = ǾǾŧħḗḗř
shoes.type.categories.m.snow\ boots = Şƞǿǿẇ ƀǿǿǿǿŧş
shoes.type.categories.m.sandals = Şȧȧƞḓȧȧŀş
results.info_primary = <p>Ŧħīş řḗḗƈǿǿḿḿḗḗƞḓȧȧŧīǿǿƞ īş ƀȧȧşḗḗḓ ǿǿƞ ŧħḗḗ şīẑḗḗ ŧħȧȧŧ <b>ƥḗḗǿǿƥŀḗḗ ŀīķḗḗ ẏǿǿŭŭ</b> ƀǿǿŭŭɠħŧ, ȧȧƞḓ ẇħḗḗŧħḗḗř ŧħḗḗẏ řḗḗŧŭŭřƞḗḗḓ īŧ.</p><p>Ɓȧȧşḗḗḓ ǿǿƞ ŧħḗḗ ƥŭŭřƈħȧȧşḗḗş ǿǿƒ ǿǿṽḗḗř {{noOfShoppers}} şīḿīŀȧȧř şħǿǿƥƥḗḗřş, ŧħḗḗřḗḗ īş <b>ȧȧ <span class='uclw_percentage_span'>{{{percentage}}}</span> ƈħȧȧƞƈḗḗ</b> ŧħȧȧŧ ẏǿǿŭŭ ẇīŀŀ ƀḗḗ ħȧȧƥƥẏ ẇīŧħ <span class='uclw_nowrap'>şīẑḗḗ {{size}}</span>.</p>
```

The rules are as follows: One Latin consonant (b,c,d,f ..)  form the values in source file is mapped to one consonant of the pseudo-language (ƀ,ƈ,ḓ,ƒ, .. ), one Latin vowel (a,e,i,...) is mapped to two vowels of the language file (ȧ,ḗ,ī, ...)

