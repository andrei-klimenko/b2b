## Add ssh pub keys

Добавление публичных ключей происходит в ansible playbook [ssh.yaml](ssh.yaml) , публичные ключи лежат в директории ssh в файле authorized_keys (Если нужно добавить юзера и для него ключи то можно раскомментировать нужны блок)

![ssh.yaml](/assets/ssh.png)

## Check ssh

** Я предположил, что подразумевается что нужно проверить ssh connections (w -h) и получил все файлы публичные ключи в authorized_keys

Проверка ssh access и отправка сформированного сообщения на smtp сервер происходит в файле [check_ssh_access.yaml](check_ssh_access.yaml)

![ssh_check_access.yaml](/assets/ssh_access_check.png)

