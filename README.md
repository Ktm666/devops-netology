1. Опишите основные преимущества применения на практике IaaC-паттернов.
Какой из принципов IaaC является основополагающим?

  -Приимуществами IaaC на практике является увелечение процессов автоматизации и разворачивание инфраструктуры, что приведет к увелечению скорости работ и снижение трудозотрат.
Так же можно отметить такие преимущества масштабируемости, надежности и стабильности, а так же простой процесс описание документации, а так же увелечение безопастности за счет ручного труда.

  -Главным приципом является создание и настройка инфраструктуры аналогично процессу разработки ПО


2. Чем Ansible выгодно отличается от других систем управление конфигурациями?
Какой, на ваш взгляд, метод работы систем конфигурации более надёжный — push или pull?

  -Главное отличие заключается в том, что он использует уже существующую ssh инфрастрктуру, а аналоги потребуют установки дополнительного окружения

  -Pull, потому что отсутствует точка отказа и данные для доступа


3. `dmitry@HP:~/Загрузки$ vboxmanage -v
6.1.48_Ubuntur159471
dmitry@HP:~/Загрузки$ vagrant -v
Vagrant 2.3.4
dmitry@HP:~/Загрузки$ terraform -v
Terraform v1.5.7
on linux_amd64

Your version of Terraform is out of date! The latest version
is 1.7.2. You can update by downloading from https://www.terraform.io/downloads.html
dmitry@HP:~/Загрузки$ ansible --version
ansible [core 2.15.9]
config file = /etc/ansible/ansible.cfg
configured module search path = ['/home/dmitry/.ansible/plugins/modules', '/usr/share/ansible/plugins/modules']
ansible python module location = /usr/lib/python3/dist-packages/ansible
ansible collection location = /home/dmitry/.ansible/collections:/usr/share/ansible/collections
executable location = /usr/bin/ansible
python version = 3.10.12 (main, Jun 11 2023, 05:26:28) [GCC 11.4.0] (/usr/bin/python3)
jinja version = 3.0.3
libyaml = True`
