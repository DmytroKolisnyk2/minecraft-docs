---
sidebar_position: 12
---

# Мінотавр

#### Опис

:::tip
Сьогодні ми продовжимо працювати в лабіринті й навчимося створювати систему фейєрверків і притискних панелей, а також битимемося з Мінотавром!👾
:::

## Згадаймо🤔

1. Що таке нить Аріадни?&#x20;
2. Хто такий Мінотавр?&#x20;
3. Де з'явився перший фейєрверк?
4. Як створити фейєрверк?

## Сьогодні ми:

1. Побудуємо систему запуску фейєрверків
2. Створимо систему з притискних панелей, пилу редстоуну, липкого поршню та блок смарагду
3. Навчимося виводити на екран різні символи та текст при натисканні натискної панелі (з висування)

### Події

На початку заняття відпрацюємо створення елементів, які можуть сигналізувати про прохід агенту чи гравця в певній точці.

### Фейєрверки

Побудуйте систему запуску фейєрверків з **дубовими притискними пластинами**, **пилом редстоуну** та **розподілювачами**.

![](<img/lesson-12/image (20).png>)

До розподілювачів завантажимо фейєрверки.

![](<img/lesson-12/image (26).png>)![](<img/lesson-12/image (21).png>)

Сформуємо код, який дозволяє поставити агента навпроти створених притискних панелей.

![](<img/lesson-12/image (25).png>)

![](img/lesson-12/image.png)

![](<img/lesson-12/image (24).png>)

![](https://github.com/mikh-maksi/minecraft_cards2/raw/main/lesson04/img/fireworks08.gif)

### Липкий поршень

Створіть систему з притискних панелей, пилу редстоуну, липкого поршню та блок смарагду.

![](https://github.com/mikh-maksi/minecraft_cards2/raw/main/lesson04/img/piston01.png)

Перевірте роботу створеної системи.

![](https://github.com/mikh-maksi/minecraft_cards2/raw/main/lesson04/img/piston02.gif)

Визначте координати поруч із блоком смарагду **(-30;4;-99)**.&#x20;

{% hint style="warning" %}
**Зверніть увагу!** У вас координати (-30;4;-99) будуть іншими, їх значення необхідно брати із вказівника координат в точці, куде липкий поршень пересуває блок смарагду **у вашому світі.**
:::

\***\*![](<img/lesson-12/image (19).png>)\*\***

Сформуйте код, який контролює наявність блоку смарагду у визначених координатах (-30;4;-99).

![](<img/lesson-12/image (17).png>)

Перевірте роботу відповідного елементу.

![](https://github.com/mikh-maksi/minecraft_cards2/raw/main/lesson04/img/piston05.gif)

### Події

|               |                                                                                                                                                                                                                                                                                          |
| ------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Завдання**  | <p></p><ol><li>Виведіть на екран символи «<strong>:-)</strong>» при натисканні натискної панелі (із висування).</li><li>Виведіть на екран символи «<strong>!</strong>» при натисканні натискної панелі.</li><li>Виведіть поточний ігровий час при натисканні натискної панелі.</li></ol> |
| **Код**       | <p><img src="https://github.com/mikh-maksi/minecraft_cards2/raw/main/lesson04/img/piston03.png" alt="no-img"/><br/><img src="https://github.com/mikh-maksi/minecraft_cards2/raw/main/lesson04/img/piston04.png" alt="no-img"/></p>                                                       |
| **Результат** | ![](https://github.com/mikh-maksi/minecraft_cards2/raw/main/lesson04/img/piston05.gif)                                                                                                                                                                                                   |

### Одна дія

Ви можете побачити в попередньому завданні, що виведення на екран тексту повторюється декілька разів. Для того, щоб дія повторювалася лише один раз, необхідно використовувати змінну, якій значення задаємо при команді «start». Встановимо код, який задає змінній flag **значення 0** та виведемо на екран повідомлення «**(+) Flag activated.**»

![](<img/lesson-12/image (2).png>)

Додамо умову спрацьовування (знаходження блоку смарагду в точці (-30;4;-99)) та за умови, що змінна flag має значення 0

![](<img/lesson-12/image (8).png>)

Змінимо значення змінної **flag на 1**. В результі дія, що зазначена в цій умові (в нашому випадку це вивід на екран символів «**:-)**») відбудеться лише 1 раз.

![](<img/lesson-12/image (3).png>)

Змінимо текст повідомлення на «**(-) Flag deactivated.**»

![](https://github.com/mikh-maksi/minecraft_cards2/raw/main/lesson04/img/piston09.gif)

Для створеної системи з притискної панелі, пилу редстоуну, липкого поршню та блоку смарагду запрограмуйте наступні дії (_**зверніть увагу**, що в вашому випадку координати можуть відрізнятися, і вам необхідно визначати координати місця, у яке переміщується блок смарагду самостійно_):

| **Завдання**  | <ol><li>Запрограмуйте так, щоб при команді <strong>start</strong> на екран було виведено текст <strong>(+)Flag activated</strong>, а при натисканні панелі — один раз було виведено <strong>(-)Flag deactivated</strong></li><li>Запрограмуйте так, щоб при команді <strong>start</strong> на екран було виведено текст <strong>Action started!</strong>, а при натисканні панелі — один раз було виведено <strong>Action stoped!</strong></li></ol> |
| ------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Код**       | <p><img src="https://github.com/mikh-maksi/minecraft_cards2/raw/main/lesson04/img/piston11.png" alt="no-img"/><br/><img src="https://github.com/mikh-maksi/minecraft_cards2/raw/main/lesson04/img/piston10.png" alt="no-img"/></p>                                                                                                                                                                                                                   |
| **Результат** | ![](https://github.com/mikh-maksi/minecraft_cards2/raw/main/lesson04/img/piston09.gif)                                                                                                                                                                                                                                                                                                                                                               |

## Творче завдання:

1. Задайте самостійно за власним бажанням текст, що буде виводитися на екран при команді чату start та при натисканні натискної панелі.

## Фіксація розбиття блоків

За команди чату **start2** задамо змінній **flag2** значення **1** та виведемо на екран повідомлення «**start**». А також перенесемо гравця в точку **(-40;4;-90)** та розмістимо блок алмазу в точці **(-45;4;-90)**

\***\*![](<img/lesson-12/image (16).png>)\*\***

Задамо код, який виводить повідомлення «**finish**», якщо блок алмазу знищити. Задамо код, який виводить повідомлення «**finish**», якщо блок алмазу знищити.

![](https://github.com/mikh-maksi/minecraft_cards2/raw/main/lesson04/img/piston13.png)

Подивимось на на результат

![](https://github.com/mikh-maksi/minecraft_cards2/raw/main/lesson04/img/piston14.gif)

## Фіксація розбиття 2-х блоків

Створимо два блоку: смарагду та алмазу та задамо змінним **flag3** та **flag4** значення 1, а також виведемо на екран текст «**Initialisation**»

![](<img/lesson-12/image (12).png>)

При знищенні алмазного блоку напишемо на екрані **Start,** при знищенні смарагдового — напишемо на екрані **Finish**

\***\*![](<img/lesson-12/image (22).png>)\*\***

Подивимось на результат

![](https://github.com/mikh-maksi/minecraft_cards2/raw/main/lesson04/img/piston17.gif)

## Лабіринт \*\*\*\* Мінотавра

Поновимо лабіринт з попереднього заняття.

|     **1**     | ![](<img/lesson-12/image (5).png>)  |
| :-----------: | ----------------------------------- |
|     **2**     | ![](<img/lesson-12/image (13).png>) |
|     **3**     | ![](<img/lesson-12/image (9).png>)  |
|     **4**     | ![](<img/lesson-12/image (7).png>)  |
| **Результат** | ![](<img/lesson-12/image (27).png>) |
|               |                                     |

:::info
Як ви пам'ятаєте, **Мінотавр** — міфічна страшна істота з тулубом людини і головою бика — був народжений Пасіфаєю, дружиною царя Міноса (одного з трьох синів Зевса і Європи) від бика, якого володар морів Посейдон відправив на острів Крит. Цар Мінос замкнув Мінотавра в лабіринті, складній споруді, яку побудував спеціально для цього Дедал.

Андрогеос, син Міноса, взяв участь в іграх в Афінах і **став переможцем у всіх спортивних дисциплінах**. Хтось зі скривджених афінян влаштував засідку і **вбив його**. Це вбивство викликало гнів Міноса, він негайно ж оголосив війну Афінам і розпочав воєнний похід. Відшкодування збитку, яке він зажадав у афінського царя Егея, було набагато жорсткіше й ганебніше, ніж сама поразка Афін: _**кожні 9 років Егей повинен був відправляти в лабіринт 7 дівчат і 7 юнаків**_. Їх зачиняли у величезному палаці-лабіринті, де їх пожирало чудовисько.

![](<img/lesson-12/image (1).png>)
:::

Створимо в нашому лабіринті Мінотавра і спробуємо з ним битися!

![](<img/lesson-12/image (14).png>)

![](<img/lesson-12/image (10).png>)

![](https://github.com/mikh-maksi/minecraft_cards2/raw/main/lesson04/img/labirint13.gif)

## Супер-творче завдання

Додайте до лабіринту власні елементи за бажанням:&#x20;

- притискні панелі з феєрверками;
- липкі поршні, що дозволяють фіксувати наявності блоків в точці з певними координатами;
- а також появою негативних мобів за умови доходження до кінці лабіринту.

![Підсумки заняття](<img/lesson-12/Group 2393.png>)
