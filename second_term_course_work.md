# Курсова робота

Завдання на курсову роботу вибирається студентом довільно з наведених нижче варіантів завдання.

Загальні вимоги до додатків:

- додатки повинні мати консольний чи графічний інтерфейс;
- для зберігання даних можна використовувати бази даних або зберігати дані локально в колекціях.

## Перелік тем

### 1. Додаток "Турфірма"

Потрібно розробити програмну систему, призначену для працівників туристичної фірми. Така система повинна забезпечувати зберігання відомостей про наявні у продажу путівки та про клієнтів фірми. Відомості про путівку включають її вартість, час відправлення (початок) та повернення, екскурсії та інші послуги, наприклад, у вартість путівки повністю або частково може входити харчування. Путівка передбачає відвідування одного населеного пункту. Туристична фірма продає стандартні путівки. Кожен клієнт купує одну путівку.

**Можливі сутності та їх властивості:**

- `Client: id, firstName, lastName, phone, passport`;
- `Tour: id, title, startDate, endDate, city, price`;
- `Sale: id, date, tourId, clientId`.

**У додатку має бути реалізований наступний функціонал:**

- додавання, редагування, видалення клієнта;
- додавання, редагування, видалення путівки;
- створення, редагування, видалення продажу.

**Також програма має виводити в консоль таку інформацію:**

- скільки продано путівок до певного міста (назва міста вводиться користувачем);
- скільки продано путівок за певний місяць (місяць запроваджується користувачем);
- загальна вартість проданих путівок за певний місяць (місяць запроваджується користувачем).

### 2. Додаток "Мережа аптек"

Потрібно розробити програмну систему, призначену для директора мережі аптек. Така система повинна забезпечувати зберігання відомостей про аптеку, про наявні в ній поставки товарів та постачальників. Кожна аптека здійснює постачання у різних постачальників, бажано при цьому закуповувати одні види товару в одних постачальників, інші в інших.
Поставки, що є в аптеці, характеризуються найменуванням, ціною, терміном придатності та кількістю. Директор аптеки закуповує потрібні товари партіями у постачальників і списує прострочені партії товарів.

**Можливі сутності та їх властивості:**

- `Pharmacy: id, title, address, phone`;
- `Shipment: id, medicineTitle, shipmentDate, expirationDate, medicineQuality, vendorId`;
- `Vendor: id, title, phone, address`.

**У додатку має бути реалізований наступний функціонал:**

- додавання, редагування, видалення аптеки;
- додавання, редагування, видалення постачання товару;
- створення, редагування, видалення постачальника.

**Також додаток має виводити в консоль таку інформацію:**

- скільки виконано постачань певного товару за минулий місяць (назва товару вводиться користувачем);
- які партії товару близькі до списання (до кінця терміну придатності залишилося менше тижня від поточної дати);
- загальна сума поставок для обраної аптеки від обраного постачальника (аптека та постачальник вводиться користувачем).

### 3. Додаток "Деканат"

Потрібно розробити програмну систему, призначену для працівника деканату. Така система повинна забезпечувати збереження відомостей про групи та студентів, а також результати поточної сесії.

**Можливі сутності та їх властивості:**

- `Student: id, firstName, lastName, groupId`;
- `Group: id, groupName, entryDate, department, disciplines`;
- `Discipline: id, title, examType`.

**У додатку має бути реалізований наступний функціонал:**

- додавання, редагування, видалення студента;
- додавання, редагування, видалення групи;
- створення, редагування, видалення дисципліни;
- виставлення оцінки з дисципліни конкретного студента.

**Також додаток має виводити в консоль таку інформацію:**

- середній бал групи по певній дисципліні (дисципліна вводиться користувачем);
- список студентів з усіх груп, які підлягають відрахуванню (не здано більше двох дисциплін);
- з якої дисципліни найбільше незадовільних оцінок.

### 4. Додаток "Станція технічного обслуговування"

Потрібно розробити програмну систему, яка призначена для диспетчера СТО. Така система повинна забезпечити зберігання інформації про клієнтів, про працівників та автомобілі, які вони ремонтують на даний момент. **Клієнт** - це людина, яка хоча б одного разу використовувала послуги СТО. Про клієнта повинна зберігатися інформація із вказанням автівок, які він здавав в ремонт.

**Можливі сутності та їх властивості:**

- `Client: id, firstName, lastName, phone`;
- `Work: id, vehicleId, workerId, startDate, endDate, price, workPerformed`;
- `Vehicle: id, clientId, color, model, licensePlate`;
- `Worker: id, firstName, lastName`.

**У додатку має бути реалізований наступний функціонал:**

- додавання, редагування, видалення клієнта;
- додавання, редагування, видалення роботи;
- створення, редагування, видалення працівника;
- створення, редагування, видалення автівки.

**Також додаток має виводити в консоль таку інформацію:**

- загальна сума виконаних робіт по кожному робітнику;
- автівки якої моделі ремонтуються частіше всього (перші 5 моделей);
- який клієнт заплатив більше всього (перші 5 клієнтів).

### 5. Власна тема

Студент може запропонувати свою тему для курсової роботи та обговорити її з викладачем.

**Курсові роботи із власною темою допускаються до захисту тільки за умови того, що тема була попередньо узгоджена з викладачем.**