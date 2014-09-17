INSTALL

activate virtualenv and install requirements.

```
pip install -r req.txt
./manage.py syncdb
./manage.py migrate --all
./manage.py runserver
```

Enjoy!


config format for dynamic_models is xml
cat apps/dynamic_models/config.xml

```
<?xml version="1.0" encoding="UTF-8"?>
<root>
  <model name="users" title="Пользователи">
    <field id="name" type="char" title="Имя" />
    <field id="paycheck" type="int" title="Зарплата" />
  </model>
  <model name="rooms" title="Комнаты">
    <field id="department" type="char" title="Отдел" />
    <field id="spots" type="int" title="Вместимость" />
  </model>
  <model name="officies" title="Офисы">
    <field id="address" type="char" title="Адрес" />
    <field id="description" type="text" title="Описание" />
  </model>
</root>
```
