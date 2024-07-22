# Проект Kittygram

## Суть данного репозитория заключается в получении навыков деплоя проекта на сервер(DevOps). В ходе деплоя были приобретены навыки:

1. Подключения к *VPS*. :heavy_check_mark:
2. Обновления пакетов сервера. :heavy_check_mark:
3. Генерации *SSH-ключей*. :heavy_check_mark:
4. Клонирования проекта с личного аккаунта *GitHub* на *VPS*. :heavy_check_mark:
5. Установки на сервер интерпретатора *Python* и дополнительных утилит. :heavy_check_mark:
6. Запуска бэкенд приложения (*Django*). :heavy_check_mark:
7. Запуска фронтенд приложения (*React*). :heavy_check_mark:
8. Установки, настройки и запуска WSGI-сервера (*Gunicorn*). :heavy_check_mark:
9. Установки, настройки и запуска SGI- и обратного прокси-сервера (*Nginx*). :heavy_check_mark:
10. Получения и внедрения в проект доменного имени. :heavy_check_mark:
11. Получения *SSL-сертификата*. :heavy_check_mark:
12. Сокрытия *SECRET_KEY* бэкенда *Django* в файле *.env*

## Создание собственного *SECRET_KEY* для *Django*.

1. Генерируем *SECRET_KEY* на данном ресурсе:
   <br>[Djecrety](https://djecrety.ir/)
2. Создаем файл *.env* в корневой директории где располагается файл *manage.py*
   ```bash
   touch .env
   ```
3. Открываем файл *.env* в редакторе *nano*.
   ```bash
   nano .env
   ```
   И создаем переменную *DJANGO_SECRET_KEY*, для которой присваиваем значение сгенерированного вами ключа:
   ```bash
   DJANGO_SECRET_KEY='ваш_секретный_ключ'
   ```

<br>**Это первый спринт из курса "Управление проектом на удалённом сервере Ver.2.0" от Яндекс.Практикум*