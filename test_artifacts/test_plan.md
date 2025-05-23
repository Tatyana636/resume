# Тест-план мобильное приложение


|||
|-|--------|
| Мобильное приложение | Версия 1.0 |
| Мастер тест-план| Дата: 22.04.2025 |
|Идентификатор документа: 01||

|Дата |Версия| Изменения |Автор |
|-|-|-|-|
|20.04.2025|1.0| Первая мажорная и минорная версии плана тестирования |  |

<br>

# Главный план тестирования мобильного приложения

## 1. Введение

Документ описывает методы и подходы к тестированию, которые будут использоваться инженером по обеспечению качества отдела обеспечения качества, для тестирования мобильного приложения.

Проверка объекта тестирования — это деятельность, направленная на проверку работоспособности функций приложения в операционных системах Android и iOS.

1.1 Цель

Документ “Тест план” для проекта [...] (далее *“Продукт”*) преследует следующие цели:
- определить стратегии тестирования Продукта, которые планируется использовать;
- определить компоненты Продукта, которые должны быть протестированы;
- спланировать процесс тестирования и техническую поддержку тестирования;
- описать структуру и рамки тестирования, достаточные для достижения целей и решения задач;
- определить перечень инструментов, которые будут использоваться в процессе тестирования;
- определить этапы работ и основные вехи;
- определить обязанности, роли и ресурсы в процессе тестирования;
- определить критерии начала и окончания процесса тестирования;
- определить возможные риски при тестировании продукта и способы их избежать.

1.2 Общие сведения

*Продукт* предназначен для <...>.
Особенности:
- при разработке *Продукта* использовался <...>;
- в качестве решения для хранения данных, выводимых в приложение используется БД MySQL;
- в качестве решения для хранения временных данных локально используется база данных SQLite3;
- в качестве системы для сбора статистики по использованию мобильного приложения используется AppMetrica;
- *продукт* размещен в следующих маркетплейсах: AppStore, AppGallery, Google Play Market, NashStore.

1.3 Объем работ

Для обеспечения качества *Продукта* проводятся следующие виды тестирования: 
- ручное тестирование; 
- автоматизированное тестирование;
- дымовое тестирование; 
- системное интеграционное тестирование; 
- функциональное тестирование; 
- тестирование интерфейса;
- тестирование базы данных;
- тестирование безопасности;
- тестирование конфигурации;
- регрессионное тестирование; 
- тестирование уменьшения памяти и энергии;
- тестирование инсталляции;
- тестирование глобализации и локализации;
- тестирование документации;
- верификация;
- пост-релизное тестирование;
- тестирование производительности.

Подробный набор находится в детальном тест-плане.

Текущий подход к контролю качества подразумевает следующие вехи проекта:
- система готова к демонстрации заказчику;
- система готова к промышленной эксплуатации.
    
Такое разбиение предполагает продемонстрировать как можно более раннюю версию работающего прототипа заказчику с целью получения обратной связи.\
Для проверки готовности продукта используется План Приемочных Испытаний (ППИ). \
Для проверки готовности к промышленной эксплуатации используется полный набор запланированных тестов.\
Готовность определяется руководителем проекта на основании представленных ему руководителем или менеджером тестирования отчётов о полноте тестового покрытия и списка значимых расхождений, оформленных в виде ошибок в системе отслеживания ошибок.


## 2. Требования к тестированию

В приведенном ниже списке указаны те функциональные и нефункциональные требования, которые были определены в качестве целей для тестирования. Этот список представляет то, что будет тестироваться.
    
**Функциональные возможности:**
- *Пригодность.*
    
    Свойства и характеристики программного обеспечения, относящиеся к наличию и соответствию набора функций конкретным задачам. Примерами соответствия является состав функций, ориентированных на задачу, из входящих в него подфункций и объемы таблиц.
- *Правильность.* 
    
    Свойства и характеристики программного обеспечения, относящиеся к обеспечению правильности или соответствия результатов. Например, она включает необходимую степень точности вычисленных значений.
 - *Способность к взаимодействию.*
    
    Свойства и характеристики программного обеспечения, относящиеся к способности его взаимодействовать с конкретными системами.
- *Согласованность*. 
    
    Свойства и характеристики программного обеспечения, которые заставляют программу придерживаться соответствующих стандартов или соглашений, или положений законов, или подобных рекомендаций.
- *Защищенность.* 

    Свойства и характеристики программного обеспечения, относящиеся к его способности предотвращать несанкционированный доступ, случайный или преднамеренный, к программам и данным.

**Надёжность:**
- *Стабильность.* 
    
    Свойства и характеристики программного обеспечения, относящиеся к частоте отказов при ошибках в программном обеспечении.
- *Устойчивость к ошибкам.*

    Свойства и характеристики программного обеспечения, относящиеся к его способности поддерживать определенный уровень качества функционирования в случаях программных ошибок или нарушения определенного интерфейса.
- *Восстанавливаемость.*
    Свойства и характеристики программного обеспечения, относящиеся к его возможности восстанавливать уровень качества функционирования и восстанавливать данные, непосредственно поврежденные в случае отказа, а также к времени и усилиям, необходимым для этого.

**Практичность:**
- *Понятность.*
        
    Свойства и характеристики программного обеспечения, относящиеся к усилиям пользователя по пониманию общей логической концепции и ее применимости.

- *Обучаемость.* 

    Свойства и характеристики программного обеспечения, относящиеся к усилиям пользователя по обучению его применению (например, оперативному управлению, вводу, выводу).
- *Простота использования.*
    Свойства и характеристики программного обеспечения, относящиеся к усилиям пользователя, по эксплуатации и оперативному управлению.

- *Эффективность*:

    Характер изменения во времени. Свойства и характеристики программного обеспечения, 
        относящиеся к временам отклика и обработки и к скоростям выполнения его функций.

- *Характер изменения ресурсов.*

    Свойства и характеристики программного обеспечения, относящиеся к объему используемых ресурсов и продолжительности такого использования при выполнении функции.

**Сопровождение:**
- *Анализируемость.*
    
    Свойства и характеристики программного обеспечения, относящиеся к усилиям, необходимым для диагностики недостатков или случаев отказов, или определения составных частей для модернизации.
- *Изменяемость*.
    
    Свойства и характеристики программного обеспечения, относящиеся к усилиям, необходимым для модификации, устранению отказа или для изменения условий эксплуатации.
- *Устойчивость.*

    Свойства и характеристики программного обеспечения, относящиеся к риску от непредвиденных эффектов модификации.
- *Тестируемость.*
        
    Свойства и характеристики программного обеспечения, относящиеся к усилиям, необходимым для проверки модифицированного программного обеспечения.

**Мобильность:**
- *Адаптируемость.*
    
    Свойства и характеристики программного обеспечения, относящиеся к удобству его адаптации к различным конкретным условиям эксплуатации, без применения других действий или способов, кроме тех, что предназначены для этого в рассматриваемом программное обеспечении.
- *Простота внедрения*.
    
    Свойства и характеристики программного обеспечения, относящиеся к усилиям, необходимым для внедрения программного обеспечения в конкретное окружение.
- *Соответствие.*

    Свойства и характеристики программного обеспечения, которые заставляют программу подчиняться стандартам или соглашениям, относящимся к мобильности.
- *Взаимозаменяемость*.
    
    Свойства и характеристики программного обеспечения, относящиеся к простоте и трудоемкости его применения вместо другого конкретного программного средства в среде этого средства. Взаимозаменяемость может включать атрибуты простоты внедрения и адаптируемости.

## 3. Стратегия тестирования

Основными задачами тестирования являются:
- проведение функционального тестирования каждого модуля и компонента системы для проверки его соответствия функциональным требованиям;
- проведение комплексного тестирования для проверки обеспечения взаимодействия модулей и компонентов друг с другом согласно требованиям к системе;
- определение производительности системы и каждого отдельного модуля;
- проведение нагрузочного тестирования для обеспечения уверенности в отказоустойчивости системы и каждого отдельного модуля;
- максимальная автоматизация процесса тестирования;
- разработка достаточного набора контрольных примеров для тестирования новых модулей и компонентов;
- своевременная разработка контрольных примеров для покрытия устраняемых ошибок;
- увеличение покрытия кода тестовыми примерами;
- подготовка документации для тестирования;
- тестирование удобства применения модулей, имеющих графический интерфейс.

3.1 Типы тестирования
3.2 Инструменты тестирования

## 4. Ресурсы

Этот раздел представляет собой рекомендуемые для проекта ресурсы, их главные обязанности, знания и навыки.

4.1 Исполнители и роли

## 5. Основные этапы и трудозатраты

В таблице содержится описание трудоемкости для каждого объема работ. Примерный шаблон приведен в таблице ниже. Подробно информация по каждому этапу будет описана в плане приемочных испытаний.


|Задача |Дата начала|Дата окончания |
|-|-|-|
|Планирование тестов||  |
|Разработка тест-кейсов и чек-листов||  |
|Разработка автоматизированных тестов||  |
|Выполнение тестов|  ||
|Оценка результатов тестов||  |

## 6. Критерии тестирования

6.1 Критерии успешности тестирования:
- все тест-кейсы с высоким приоритетом закрыты с результатом «пройден»;
- тестовое покрытие проверено и является достаточным, где критерий достаточности составляет не менее 80% покрытия требований тестами;
- итоговый отчет составлен и утвержден руководителем отдела тестирования и заказчиком(руководителем проекта).


6.2 Критерии прерывания и продолжения тестирования:\
Критерием прерывания тестирования является появление и занесение блокирующих дефектов в систему отслеживания ошибок;\
Критерием продолжения тестирования является закрытие блокирующей ошибки в системе отслеживания ошибок.

## 7. Риски

Определение требований теста - это только часть подготовки к тестированию. Это этап необходим по следующим причинам:
- самые важные и рискованные требования должны быть протестированы как можно раньше
- тестирование должно включать проверку зависимостей, например, последовательности данных


7.1 Оценка рисков 
Основные риски, которые могут повлиять на успешное тестирование и функционирование Продукта: <...>

7.2 Идентификация рисков

Риски, с которыми может столкнуться команда тестирования *Продукта*:
- неполное или недостаточное количество тестов может привести к упущению дефектов или нежелательному поведению приложения;
- разнообразие мобильных устройств, операционных систем и сетевых условий создает сложности при обеспечении однородности тестирования;
- долгое восстановление сервера после сбоя или медленная работа сервера;
- небезопасное хранение или передача личной информации пользователей может привести к рискам нарушения конфиденциальности.

7.3 Воздействие на процесс тестирования

Вышеперечисленные риски могут повлиять на выполнение тест-плана следующим образом:
- недостаточное покрытие тестами может привести к невыполнению запланированных задач тестирования, так как не все аспекты функциональности приложения будут оценены;
- разнообразие мобильных устройств и операционных систем, а также сложные сценарии тестирования могут потребовать больше времени для проведения тестов или дополнительных циклов тестирования;
- если возникают проблемы с безопасностью данных или отсутствуют проверки специфичные для мобильных устройств, это может привести к недооценке важных аспектов качества приложения;
- долгое время восстановления сервера или медленная его работа может привести к задержкам в выполнении плановых тестовых задач, поскольку некоторые функциональные или интеграционные тесты могут зависеть от доступности сервера;
- несоответствие требованиям качества и недостаточное покрытие тестами может привести к обнаружению дефектов пользователем после релиза, что может негативно сказаться на репутации и успехе приложения.

7.4 Меры по снижению рисков


## 8. Определение серьезности ошибки и приоритета

Поле приоритета ошибок очень важно для классификации ошибок, если и когда ошибки будут исправлены.  Уровни приоритета ошибок будут определяться, как указано в таблице ниже.  При тестировании всем ошибкам будет присвоен приоритет ответственным за проект тестировщиком. Позже руководитель проекта совместно с руководителем разработки и тестировщиком могут пересмотреть заданные приоритеты

8.1 Список приоритетов и серьезность ошибок


## 8. Итоговые отчеты

После окончания тестирования формируются отчеты, в которых отображаются следующие данные:
- количество всех тестов;
- количество: всех тестов: пройденных успешно, не пройденных успешно, тестов, которые не выполнялись;
- информация о критических ошибках, размещённых в системе отслеживания ошибок;
- информация о времени, затраченном на тестирование;
- информация о дате начала и завершения тестирования;
- информация о количестве ошибок: всего ошибок, закрыто ошибок, новые ошибки выявленные в процессе тестирования, новые ошибки выявленные в процессе эксплуатации;
- информация о критических ошибках, размещённых в системе отслеживания ошибок и влияющих на готовность Продукта;
- оценка степени готовности Продукта.


