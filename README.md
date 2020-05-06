# OctoberCMS-AZ

Tercüme aşamasındadır 

az klasörleri ilgili yerlere elave olunladırı

modules/system/lang/  klasöründe bütün dillerin lang.php faylında locale kısmına az eklenmelidir


```shell
 'locale' => [
        'az' => 'Azərbaycan dili',

        ]
```


  
modules/backend/models/Preference.php  aşağıdakı kimi düzenlenmelidir

```shell
 public function getLocaleOptions()
    {
        $localeOptions = [
            'az'    => [Lang::get('system::lang.locale.az'),    'flag-az'],

        ]
```