# Постановка задачи

## Регион
Москва, крупные промышленные города

## Тема задачи
Цифровизация промышленности. Автоматизированное отслеживание местонахождения изготавливаемых деталей и сборок

## Проблема
В процессе многономенклатурного единичного и мелкосерийного производства изделий, сборочных единиц и деталей на крупных приборостроительных и машиностроительных предприятиях осуществляется большое количество ручных операций по отслеживанию текущего месторасположения деталей и сборок на производственных участках, в планово-диспетчерских бюро (ПДБ), кладовых, что отнимает значительное время и отрицательно сказывается на производительности труда начальников участков, диспетчеров, кладовщиков, рабочих. Кроме того, в связи с «простоем» деталей до момента ручного учета руководители разных уровней производства не всегда в режиме реального времени могут отследить местоположение изготавливаемого изделия и его частей, а также номенклатуру всего передела, находящегося в цеху, на участке или в кладовой.

Многономенклатурность производства делает необходимым перемещение такелажниками и распределителями работ большого количества различных деталей, загруженных в одну транспортную тару или тележку, по совершенно разным цехам и производственным участкам с текущего месторасположения. Сотрудники, ответственные за транспортировку, руководствуются интуитивными соображениями о том, по какому маршруту следовать между цехами и участками, и не всегда выбирают оптимальный по времени и расстоянию маршрут, а значит возрастает трудоемкость и уменьшается производительность таких межоперационных переносов.

## Задача
Разработать платформу, позволяющую создавать карту производственных помещений и переходов между ними (либо загрузкой готовых карт в определенном формате), возможностью отметки на картах зон цехов, производственных участков, выполняемых на участках типов операций, участков для отгрузки привезенных на участок деталей.

Платформа должна позволять на основе введенной карты автоматически рассчитать минимально требуемое оборудование (RFID-рамки или т.п.) и его месторасположение на карте для автоматизированного отслеживания любых переходов с одного производственного участка (ПДБ, кладовой) на другой.

Учитывать многоэтажность производственных зданий, территориальную распределенность площадок по городу, лифты, лестницы, места расположения автомобильного транспорта для перевозки деталей между площадками.

Учитывать такелажника, осуществляющего транспортировку изделий, транспортную тару (тележка (можно только на лифте), коробка в руках, размер коробки), выдавать ему оптимальный маршрут для перемещения деталей из цеха в цех, с одного участка на другой. Такелажники имеют очки дополненной реальности (AR) или другое мобильное устройство, помогающее им осуществлять перемещение деталей в правильном направлении по рассчитанному оптимальному маршруту.

## Что может помочь решению задачи
1. Данные из открытых источников.
2. Готовые программные модули и библиотеки (только opensource).
3. Самостоятельно сгенерированные данные.

## Требования к результату
Комплекс программ должен поддерживать следующий функционал:
- Построение карты (или ее загрузка в определенном формате) предприятия (возможно территориально распределенное, учитывать лифты, лестницы, автотранспорт для сообщения между площадками), отметка зон цехов, участков и т.д. Возможно использование готовых opensource-систем такого класса.
- Отображение информации (обозначение, наименование, количество, производственный заказ) обо всех изделиях, деталей и сборок, находящихся в настоящий момент на производственном участке или в каком-то помещении (в ПДБ, кладовой).
- Отображение текущего местонахождения всех деталей по производственному заказу, обозначению или наименованию изделия/ДСЕ.
- Отображение на карте «снимка» всех фактических перемещений выбранного изделия, детали или сборки, а также отображение «снимка» по любой выбранной совокупности ДСЕ.
- Автоматический расчет оптимального маршрута для загруженной транспортной тары или тележки.
- Возможность создания вручную расписания перемещений ДСЕ между цехами, участками, помещениями, территориально распределенными площадками.
- На основании расписания и адресов автоматически рассчитать оптимальный маршрут движения. Если будут известны габариты, то и необходимый транспорт.
- Система поддержки для сотрудника, осуществляющего перемещение деталей, с помощью отображения направления движения по маршруту в AR-очках или на мобильном устройстве.
- Сигнализация (или простое логгирование) об отклонениях такелажника или распределителя работ от рассчитанного маршрута.
- Возможно использование в качестве модулей и частей системы сторонних opensource-решений (не использовать проприетарное ПО при наличии открытых альтернатив).

Кроме того, ожидается анализ рынка технических средств, позволяющих с минимальными затратами осуществить реализацию такого автоматизированного отслеживания и системы поддержки сотрудника, осуществляющего перемещение деталей.

## Масштаб внедрения
Система должна внедряться в масштабах предприятия, в том числе территориально распределенного, интегрироваться в функционирующие MES-системы.

## Предполагаемый срок внедрения
Пилотную версию проекта на предприятии можно внедрить за 6 месяцев.

Переход на версию с полным функционалом возможен за 2 года.

## Экономический эффект
Требуется проработка.
