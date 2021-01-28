# User
1. login
1. password
1. loginAttempts
1. blocked


## Операция проверки доступа в учетную запись
Сверяет данные полученные из БД с __*введенными пользователями*__
возвращает true если пользовалю разрешен доступ, и false если нет

-[x] Проверка заключается в сверке __*пароля*__ для запрашиваемого логина с пришедшими из БД
-[x] У пользователя три попытки для ввода пароля
-[x] Если  пароль введен неправильно, количество __*попыток*__ уменьшается на 1
-[x] Если количество попыток закончилось, значит пользователь должен быть __*заблокирован*__
-[x] Если пользователь заблокирован, он не может войти в учетную запись
-[x] Если пароль введен правильно, то количество попыток должно быть восстановлено