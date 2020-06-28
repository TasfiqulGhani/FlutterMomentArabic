# Flutter moment in Arabic

Moment is very popular for parsing timestamp into human readable very good format .In flutter moment is available but there is no Arabic version.So if you want Moment in Arabic follow this.

## Step 1:

First install Moment in your flutter project .Follow this link for this 
https://pub.dev/packages/simple_moment.


## Step 2:

Now create a dart file and add these codes.

```bash


import 'package:simple_moment/simple_moment.dart';

class LocaleAr implements ILocaleData {
  String get seconds => '1 ثانية';

  String get aMinute => 'دقيقة';
  String get minutes => '%i دقيقة';

  String get anHour => '1 ساعة';
  String get hours => '%i ساعة';

  String get aDay => '1 يوم';
  String get days => '%i يوم';

  String get aMonth => '1 شهر';
  String get months => '%i شهر';

  String get aYear => ' 1 سنه';
  String get years => '%i سنه';

  String get futureIdentifier => 'خلال';
  String get pastIdentifier => 'قبل';

  IdentifierPosition get futurePosition => IdentifierPosition.prepend;
  IdentifierPosition get pastPosition => IdentifierPosition.prepend;
}

```

## Step 3 :

Now just set the LacaleAr with your moment .

```python
moment.locale(LocaleAr())
```



## Full Code


```python

 var =new Moment.now(); 
 moment.locale(LocaleAr()).from(datetime);
```



## Thats IT !
For major changes, please open an issue first to discuss what you would like to change.
