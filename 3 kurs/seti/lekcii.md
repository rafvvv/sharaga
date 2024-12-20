```markdown
# Конспект №13
	Конструктивное исполнение коммутаторов

# Осн. типы конструктивного исполнения коммутаторов

1. Коммутаторы с фиксированным количеством портов
Описание: наиболее простой тип коммутаторов, представляющий собой отдельный корпус со
всеми необходимыми элементами, количество и тип портов обычно фиксированы.
+: Просты в использовании, недороги, компактны
-: Ограниченная гибкость конфигурации, сложно масштабировать
Применение: Используются для создания небольших сетей, рабочих групп

2. Модульные коммутаторы
Описание: Коммутаторы, в которых слоты позволяют устанавливать
различные модули, расширяющие функциональность устройства. Модули
могут быть сетевыми интерфейсами, модулями питания, модулями
управления и т.д.
+: Высокая гибкость конфигурации, возможность
масштабирования
-: Более высокая стоимость, повышенная сложность настройки
Применение: Используются в крупных сетях, где требуется высокая
производительность и возможность расширения

3. Стековые коммутаторы
Описание: Несколько коммутаторов объединяются в единую логическую
систему, управляемую как одно устройство.
+: Позволяют создавать большие сети с высокой пропускной
способностью, упрощают управление
-: Ограничения на тип коммутаторов, которые можно
объединять в стек
Применение: Используются для создания крупных сетей, требующих
высокой масштабируемости

# Факторы, влияющие на конструктивное исполнение
Количество портов, Тип портов, Пропускная способность, lvl надежности,
Функциональность, Управление

# Ключевые компоненты коммутатора
Процессор, Память, Коммутационная матрица, Порты

# Выбор коммутатора
Размер сети, Требования к пропускной способности, Функциональность, Бюджет
```

```markdown
# Конспект №14
	Общие принципы сетевого дизайна

Сетевой дизайн – это процесс планирования и проектирования компьютерной
сети с учетом требований бизнеса, технических характеристик и будущих
потребностей организации.

# Осн принципы сетевого дизайна

Модульность, Масштабируемость, Надежность, Безопасность, Производительность, 
Управляемость, Простота

# Этапы проектирования сети

1. Анализ требований
2. Разработка топологии
3. Планирование адресации
4. Выбор оборудования
5. Разработка плана безопасности
6. Документирование
7. Тестирование

# Факторы, влияющие на сетевой дизайн

Размер сети: Количество устройств и пользователей.
Тип сети: Локальная сеть (LAN), глобальная сеть (WAN), беспроводная
сеть (WLAN).
Приложения: Какие приложения будут использоваться в сети (почта, веб-
сервисы, VoIP и т.д.).
Бюджет: Финансовые ограничения.
Требования к безопасности: Уровень безопасности, необходимый для
защиты данных.

---
примеры топологий сетей
Звезда, Кольцо, Шина, Гибридная } подробнее в # Конспект №8

# Современные тенденции в сетевом дизайне

- Виртуализация сетей: Создание виртуальных сетей на физической инфраструктуре.
- SDN (Software-Defined Networking): Программное управление сетью.
- NFV (Network Functions Virtualization): Виртуализация сетевых функций.
- Безопасность: Усиление безопасности сетей за счет использования новых технологий и решений.
```

```markdown
# Конспект №15
	Технология PoweroverEthernet

Power over Ethernet (PoE) — это технология, позволяющая передавать
электрическую энергию по стандартным витым парам Ethernet наряду с данными.

Это означает, что сетевые устройства, такие как IP-телефоны, точки доступа 
Wi-Fi, IP-камеры и другие, могут получать питание непосредственно через сетевой
кабель, без необходимости в отдельной электрической розетке.

Технология PoE основана на стандартах IEEE 802.3af, 802.3at и 802.3bt, которые
определяют различные уровни мощности, которые могут быть переданы по
сетевому кабелю

Устройства, которые питаются по PoE, называются Powered Device (PD), а 
устройства, которые подают питание, называются Power Sourcing
Equipment (PSE).

# Процесс передачи питания:
1. PSE определяет, подключено ли к порту устройство, совместимое с PoE.
2. PSE начинает подавать питание на порт.
3. PD определяет тип питания и начинает потреблять необходимую мощность.

# Преимущества PoE
Упрощение установки, Гибкость размещения устройств, Экономичность, 
Централизованное управление

# Типы PoE
Type 1 (802.3af): Обеспечивает мощность до 15.4 Вт на порт.
Type 2 (802.3at): до 30 Вт на порт.
Type 3 (802.3bt): до 60 Вт на порт.
Type 4 (802.3bt): до 100 Вт на порт.

# Применение PoE
IP-телефония, Беспроводные сети, Системы видеонаблюдения, Сетевые устройства

# Ограничения PoE
Длина кабеля, Потребляемая мощность, Стоимость оборудования
```

```markdown
# Конспект №16
	Сетевой уровень. Протокол IP версии 4. Общие функции классовой и бесклассовой адресации. Выделение адресов

Сетевой lvl (lvl 3) в модели OSI отвечает за маршрутизацию пакетов
данных между различными сетями. Он определяет логические адреса устройств
(IP-адреса) и выбирает оптимальные пути для передачи данных.

# Протокол IPv4
IPv4 (Internet Protocol version 4) — это основной протокол, используемый
для передачи данных в Интернете.
Адрес IPv4: Представляет собой 32-битное число, которое записывается в
виде четырех десятичных чисел в диапазоне от 0 до 255, разделенных
точками (например, 192.168.1.1).

---
Функции IPv4:
Адресация, Маршрутизация, Фрагментация и сборка, Время жизни (TTL)

Классовая IP адресация - это метод IP-адресации, который не позволяет рационально использовать ограниченный ресурс уникальных IP-адресов, т.к. не возможно использование различных масок подсетей.

Бесклассовая IP адресация (Classless Inter- Domain Routing - CIDR) - это метод IP-адресации, кот. позволяет рационально управлять пространством IP адресов.

- Классовая адресация:
Деление адресного пространства: IP-адреса делились на пять классов (A,
B, C, D, E) в зависимости от значения первых битов. Каждый класс имел
определенный диапазон адресов и количество доступных сетей и хостов.
Проблемы: Неэффективное использование адресного пространства,
особенно для небольших сетей.

- Бесклассовая адресация (CIDR):
Маска подсети: Введена маска подсети, которая определяет количество
битов, отвечающих за сетевой адрес, и количество битов, отвечающих за
адрес хоста.
Гибкость: Позволяет более гибко делить адресное пространство, создавая
сети различного размера.
Преимущества:
	Более эффективное использование адресного пространства.
	Возможность создавать сети различного размера.
	Упрощение маршрутизации.

# Выделение адресов
- Статическое выделение: Администратор вручную назначает IP-адрес
каждому устройству.
- Динамическое выделение: Сервер DHCP автоматически назначает IP-
адреса устройствам при их подключении к сети.
- Методы выделения в CIDR:
	- Субнетирование: Деление сети на более мелкие подсети
	- Безклассовая междоменная маршрутизация (CIDR): Использование масок подсети
	переменной длины для гибкого деления адресного пространства.
	- NAT (Network Address Translation): Перевод частных IP-адресов в
	публичные для выхода в Интернет.

# Сравнение классовой и бесклассовой адресации
```

|Характеристика|Классовая адресация|Бесклассовая адресация (CIDR)|
|-|-|-|
|Гибкость|Низкая|Высокая|
|Эффективность использования адресов|Низкая|Высокая|
|Управление сетью|Сложно|Более просто|
|Современное использование|Практически не используется|Широко используется|

.
---
.

```markdown
# Конспект №24
	Протокол Spanning Tree Protocol (STP). Уязвимости протокола STP
STP (Spanning Tree Protocol) - это сетевой протокол, работающий на канальном
уровне (2-й уровень модели OSI). Его основная задача - предотвращение циклов в
топологии сети Ethernet, которые могут привести к нестабильности и потере
data.

# Как работает STP?
1. Выбор корневого моста
2. Расчет стоимости пути
3. Выбор портов

# Состояния портов в STP
- Blocking
- Listening
- Learning
- Forwarding

+: Предотвращение циклов, Автоматическое восстановление,Стандартный протокол
-: Задержка при конвергенции, Сложность конфигурации, Влияние на производительность

# Модернизации STP
RSTP (Rapid Spanning Tree Protocol): Ускоряет процесс конвергенции
MSTP (Multiple Spanning Tree Protocol): Позволяет создавать несколько
экземпляров STP для разных VLAN
PVST+ (Per-VLAN Spanning Tree Plus): Разработан Cisco для создания
отдельных экземпляров STP для каждой VLAN

# Уязвимости протокола STP
Атаки на BPDU
Уязвимости в конфигурации
	Неправильная настройка Bridge ID
	Слабые пароли
Проблемы с аутентификацией

Способы защиты от атак на STP
BPDU Guard, Root Guard, BPDU Filter, Secure STP, VLAN Pruning, Сильные пароли, Регулярное обновление ПО, Сегментация сети, Мониторинг сети

# Примеры атак на STP
• Yersinia: Фреймворк, позволяющий проводить различные атаки на STP,
включая флуд BPDU, перехват ролей коммутаторов и другие.
• Rootkit: Злоумышленник может установить rootkit на коммутатор для
скрытного выполнения вредоносных действий.
```


```markdown
# Конспект №25
	Обзор адресации сетевого уровня.

Адресация сетевого уровня – это фундаментальный механизм, позволяющий
устройствам в компьютерной сети идентифицировать друг друга и определять
маршруты для передачи data.
- IP-адрес: Числовой идентификатор устр-ва в сети, используемый протоколом IP
- Сетевая маска: Определяет, какая часть IP-адреса относится к сети, а какая – к хосту в этой сети.
- Подсеть: Логическое подразделение сети, используемое для управления трафиком и повышения эффективности маршрутизации.
- Маршрутизатор: Устройство, которое направляет пакеты данных между различными сетями на основе их IP-адресов.

---
IPv4: Состоит из 32 бит, обычно записывается в виде четырех десятичных
чисел, разделенных точками (например, 192.168.1.100).
IPv6: Состоит из 128 бит и записывается в шестнадцатеричном виде, разделенным
двоеточиями (например, 2001:0db8:85a3:0000:0000:8a2e:0370:7334).

DHCP (Dynamic Host Configuration Protocol): Протокол, позволяющий
автоматически настраивать сетевые параметры устр-в, включая IP- адреса.
+: Упрощение администрирования, Гибкость, Эффективное использование IP-адресов

# IPV6
+: Большое адресное пространство, Улучшенная маршрутизация, Поддержка новых сервисов

# NAT
-: Проблемы с некоторыми приложениями, Сложности с сетевой адресацией
NAT – это технология, которая позволяет множеству устройств в частной сети
использовать один или несколько публичных IP-адресов для доступа в Интернет.

# Типы NAT
Статический NAT
Динамический NAT
NAPT (Network Address Port Translation): Разновидность динамического NAT


```



