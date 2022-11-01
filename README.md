# 5.1-Vitrualisation
Задание 1
Паравиртуализация - гипервизону необходима ОС, гипервизор модифицирует ядро гостевой ОС для разделения дотупа к аппартаным сердствам физического сервера
Полная виртуализация - не требуется установливать ОС на хосте, т.к. гипервизор берет на себя роль ОС, гостевые ВМ получают доступ напрямую
Витруализация уровня ОС - гипервизору необходима ОС, запуск ВМ возможен только с такой же ОС как и ядро хостовой ОС

Основные отличия 
- возможность создавать ВМ с различными ОС (полная и паравиртуализация), возможность создавать ВМ только с ОС как у хостовой машины
- скорость инициализации (Витруализация уровня ОС имеют меньшее время инициализации)
- Виртуализацтя уровня ОС не нужен гипервизор эту функцию на себя берет ядро ОС хоста

Задание 2
Высоконагруженная база данных, чувствительная к отказу - физический сервер (более высокий отклик системы, меньше вероятных узлов отключения (например могут быть проблемы не только с физическим состояние а еще и с гипервизором)
Различные web-приложения. - виртуализация уровня ОС (требуется меньше ресурсов, выше скорость, нет жестких требований к аппаратным ресурсам)
Windows системы для использования бухгалтерским отделом. - паравиртуализация (возможность добавление ресурсов ВМ, удобно делать резервные копии, можно клонировать всю ВМ)
Системы, выполняющие высокопроизводительные расчеты на GPU. - физический сервер (более эффективное использованию аппаратных ресурсов, высокая скорость работы)

Задание 3

Сценарий 1
Hyper-V так как имеет самую тесную интеграцию с MS Windows, а также плжходит под все требования
Сценарий 2
Стоит выбрать Xen та как из open source он более стабилен чем KVM, при решении задач с интенсивным водов-выводом

Сценарий 3
Стоит выбрать бесплатный Hyper-V так как имеет самую тесную интеграцию с MS Windows
Сценарий 4
Считаю что больше всего подойдет KVM. Плюсы KVM недорогой и лояльный к аппаратным ресурсам, оптимален для создания бюджетных виртуальных сред.

Задача 4

Возможные проблемы и недостатки гетерогенной среды виртуализации:
- сложность администрирования;
- необходимое наличие высококвалифицированных специалистов;
- повышенный риск отказа и недоступности;
- высокая стоимость обслуживания;
Для минимизации рисков необходимы высококвалифицированные специалисты для поддержки всей системы, а также финансирование - лицензии, программные и аппратные ресурсы, обучение сотрудников и т.д.
Я бы предпочел работать в единой среде. Небольшие выгоды в цене и производительности при использовании разных ведут
к большим издержкам в сфере обслуживания, а также поддержки работоспособности и не всегда оправданы.

