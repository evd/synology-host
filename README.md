# Хостинги для Synology Download Station
На данный момент только LostFilm.TV. Позволяет автоматически скачивать релизы через RSS.

# Установка
* Скачать последнюю версию "lostfilm.host" со страницы [релизов](https://github.com/evd/synology-hosts/releases)
* Зайти в "Настройки" Download Station, затем в раздел "Хостинг файлов", далее нажать "Добавить" и выбрать скачанный файл, подтвердить добавление.
* В редактировании указать "Имя пользователя" и "Пароль", получить их можно на сайте, а именно:
    - "Имя пользователя" можно узнать в настройках (Мой ID, формат ХХХХХХ)
    - "Пароль" в открывшемся окне (выбор качества) при скачивании любого релиза кликнув по usess слева внизу рядом со значком RSS.
* В "Каналы RSS" добавить "http://insearch.site/rssdd.xml" (актуальный URL в окне выбора качества при скачивании любого релиза)
* Для автоматиеского скачивания добавить в фильтр загрузки по каждому сериалу:
  - Название - Любое
  - Совпадения - Stranger Things*1080p (скачивать только в качестве 1080p)
  - Не совпадает - E999 (не скачивать когда выйдет сезон целиком)
  - Анализ с помощью регулярных выражений - по умолчанию

# Hosts for Synology Download Station
At the moment only LostFilm.TV. Allows automatic download of releases via RSS.

# Install
* Download the latest version of "lostfilm.host" from the [releases](https://github.com/evd/synology-hosts/releases) page
* Go to "Settings" of Download Station, then to the "File hosting" section, then click "Add" and select the downloaded file, confirm the addition.
* In the editing, specify the "Username" and "Password", you can get them on the website, namely:
    - "Username" can be found in the settings (My ID, format ХХХХХХ)
    - "Password" in the opened window (quality selection) when downloading any release by clicking on uses at the bottom left next to the RSS icon.
* In "RSS Channels" add "http://insearch.site/rssdd.xml" (current URL in the quality selection window when downloading any release)
* For automatic downloading, add to the download filter for each series:
    - Title - Any
    - Matches - Stranger Things*1080p (download only in 1080p quality)
    - Does not match - E999 (do not download when the entire season is released)
    - Analysis using regular expressions - by default
    
# Build
Run build.sh script

# Debug
1. Copy env.example.php to env.php
2. Setup credentials in env.php
3. Run php test.php
