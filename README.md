# РАБОТА С ПЕРЕДАТЧИКАМИ НА ЧАСТОТЕ 433Мгц С ПОМОЩЬЮ RASPBERRY PI

На этих частотах работают современные шлагбаумы, электронные ворота и некоторые электронные замки. Считав значения с приемника, когда идет сигнал с пульта для открытия чего-либо, вы можете повторить этот сигнал, тем самым открыть/закрыть цель.

Для приема и передачи используются такие типы модулей:

![alt text](https://static-sl.insales.ru/images/products/1/1171/141264019/1070.jpg)
![alt text](https://ae01.alicdn.com/kf/HTB1day5aULrK1Rjy1zbq6AenFXa6/QIACHIP-433-Mhz.jpg)

Их я подключил по схеме:

![alt text](https://github.com/EternalB-1/rf/blob/master/img/Screenshot_1.png?raw=true)

Для према сигнала введите:

python3 recieve.py -g 20

Для отправки сигнала:

python3 send.py -g 21 -t * -p ** ***

*-протокол

**-pulse

***-код устройства

Вся информация взята из ролика: https://youtu.be/HCiEaf1HPhE
