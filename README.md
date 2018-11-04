# GPS_display
Simple GPS displaying system

## RoadMap
- [x] Создать новый репозиторий Octonix/IPCam_monitor и выполнить форк к себе
- [ ] Исправить ошибку при которой сервис не работает в старых браузерах
- [ ] Сделать групповой просмотр снапшотов на стартовой странице с автообновлением

## Examples

    sqlite3 /var/www/net_octonix_sight/database/default.db "SELECT * FROM coordinates WHERE latitude='';"

    sqlite3 /var/www/net_octonix_sight/database/default.db "DELETE FROM coordinates WHERE latitude='';"

## Links
* http://wiki.mikrotik.com/wiki/Manual:System/GPS
* http://wiki.mikrotik.com/wiki/Manual:GPS-tracking

## License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details

