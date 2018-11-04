# GPS_display
Simple GPS displaying system

## RoadMap
- [x] Создать новый репозиторий Octonix/IPCam_monitor и выполнить форк к себе
- [ ] Исправить ошибку при которой сервис не работает в старых браузерах
- [ ] Сделать групповой просмотр снапшотов на стартовой странице с автообновлением

## Examples
#### Просмотреть все пустые записи в базе
    sqlite3 /var/www/net_octonix_sight/database/default.db "SELECT * FROM coordinates WHERE latitude='';"
#### Удалить все пустые записи в базе
    sqlite3 /var/www/net_octonix_sight/database/default.db "DELETE FROM coordinates WHERE latitude='';"
#### Войти в базу
    sqlite3 /var/www/net_octonix_sight/database/default.db
#### Внести запись в базу локально
    INSERT INTO "coordinates" VALUES('N 56 57 32.262','E 24 9 7.262','2018-10-20 23:15:01','2018-10-20 23:15:01');
#### Внести запись в базу через вызов CURL с устройства
    curl -X POST http://sight.octonix.net/index.php -H "Content-Type: application/json" --data '{"lat": "0" , "lon": "0"}'

## Links
* http://wiki.mikrotik.com/wiki/Manual:System/GPS
* http://wiki.mikrotik.com/wiki/Manual:GPS-tracking

## License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details

