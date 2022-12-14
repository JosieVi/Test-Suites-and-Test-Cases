# Test-Suites and Test-Cases
## Homework-1
Необходимо протестировать Android приложение "TO-DO-MVP".
Для одного любого модуля, который вы определите, напишите тестовый набор с кейсами.\
<b>Результат выполнения задания в TMS QASE:</b>\
[Homework-1](https://github.com/JosieVi/Test-Suites-and-Test-Cases/blob/main/Homework-1.pdf)

## Homework-2
Напишите тестовые кейсы для тестирования API запросов коллекции для 4 методов из блока store: https://petstore.swagger.io/#/store/placeOrder
\
<b>Результат выполнения задания:</b>\
[Homework-2](https://github.com/JosieVi/Test-Suites-and-Test-Cases/blob/main/Homework-2.pdf)
или [Google Диск](https://docs.google.com/spreadsheets/d/1U2-QOqwjSa5a_JUMo50xEAfwhsmjokHxvaiPEJ-HezE/edit?usp=sharing)

## Homework-3											
1. Необходимо проанализировать требования, указанные ниже. Все несоответствия и дополнительные вопросы по ним внести в новую таблицу.
2. Необходимо составить тест кейсы на функциональность Add Customer в TMS QASE по ссылке https://demo.guru99.com/telecom/index.html												


<b>Результат выполнения задания:</b>\
[Homework-3.1](https://github.com/JosieVi/Test-Suites-and-Test-Cases/blob/main/Homework-3.1.pdf)
или [Google Диск](https://docs.google.com/spreadsheets/d/18OX-cD6kwX9pq_J-IxspmPUtVl6lQsJxb3jfyMwtG2E/edit#gid=0)\
[Homework-3.2](https://github.com/JosieVi/Test-Suites-and-Test-Cases/blob/main/Homework-3.2.pdf)

**Требования. Главная страница**
1. Перед вами система, которая позволяет создавать аккаунты новых пользователей, новые тарифы, а также привязывать тарифный план к пользователю.
2. Также есть возможность просмотреть информацию о текущем счете пользователя.
3. На главной странице в шапке (header) содержится информация о названии сервиса Guru99 telecom, после нажатия на которую страница обновляется.
4. На главной странице должен присутствовать картинка с телефоном и 4 активные кнопки: Add Customer, Add Tariff Plan, Add Tariff Plan to Customer, Pay Billing и Delete Customer, а также описание для каждой из них.\
На данный момент оно выполнено в виде текста-филлера, но в следующих релизах будет обновлено.
5. При нажатии на кнопку пользователь должен перенаправляться на страницу с указанным действием.
6. Также пользователь может вызвать эти кнопки, используя боковое гамбургер-меню.\
Названия кнопок и действия после нажатия должны быть такими же, как и в пунктах 3, 4.												
7. Пользователь может закрыть боковое меню, нажав на любое свободное место на сайте или используя кнопку X.
		
**Требования. Add Customer**
1. Для пользователя доступно лого в шапке и боковое меню, которое работает по тому же принципу, как и для главной страницы.\
Под шапкой располагается название самой страницы Add Customer.		
2. Background Check обозначает статус пользователя. Pending - пользователь ожидает одобрения. Done - пользователь создан. \
Можно выбрать только один вариант.	
3. Billing Addres - это платежный адрес пользователя. При создании необходимо ввести First Name, Last Name, Email, Address и Mobile Number.	
4. У каждого поля должно быть название указанное в пункте 4 и placeholder (подсказка) внутри поля для ввода, которая должна повторять название.	
5. Все описанные поля (пп. 4 и 5) обязательные и должны быть отмечены *.\
Если оставить их пустыми, то должно появиться всплывающее окно - Please fill all fields.
6. При выборе поля для ввода оно должно подсвечиваться голубым цветом.
7. Кнопка Reset обнуляет все заполненные значения и сообщения об ошибке.	
8. Кнопка Submit сохраняет пользователя в базе.\
После ее нажатия появляется информация о Customer ID, сообщение Please Note Down Your Customer ID и кнопка Home, которая возвращает пользователя на главную страницу.	
\
Customer ID должен быть уникальным и состоять из 6.

**Требования к валидациям**		
1. First Name 
- Можно ввести только буквы.
- Требований к ограничению длины нет. 
- В случае ввода цифр должно появится сообщение - Numbers are not allowed.
- При вводе спецсимволов - Special characters are not allowed.
- При вводе кириллицы - Cyrillic are not allowed.
- При вводе цифр, латиницы и спецсимволов - Numbers, Cyrillic and special characters are not allowed.
- Если поле оставить пустым и нажать на кнопку Submit должно появиться сообщение - First Name must not be blank	.	

2. Last Name
- Можно ввести только буквы. 
- Требований к ограничению длины нет. 
- В случае ввода цифр должно появится сообщение - Numbers are not allowed. 
- При вводе спецсимволов - Special characters are not allowed. 
- При вводе кириллицы - Cyrillic are not allowed. 
- При вводе цифр, кириллицы и спецсимволов - Numbers, Cyrillic and special characters are not allowed. 
- Если поле оставить пустым и нажать на кнопку Submit должно появиться сообщение - Last Name must not be blank.

3. Email
- В поле Email встроена специальная проверка, которая проверяет наличие латиницы, обязательность @ и доменной зоны, например, .com. 
- Требований к ограничению длины нет. 
- В случае, если в это поле ввести просто буквы (кириллица или латиница), цифры или спецсимволы, должно появляться сообщение Email is not valid. 
- Если поле оставить пустым и нажать на кнопку Submit должно появиться сообщение - Last Name must not be blank.

4. Address
- Можно ввести только буквы. 
- Требований к ограничению длины нет. 
- При вводе спецсимволов - Special characters are not allowed. 
- Точка и запятая разрешены. 
- При вводе кириллицы - Cyrillic are not allowed. 
- При вводе кириллицы и спецсимволов - Cyrillic and special characters are not allowed. 
- При вводе цифр, букв и спецсимволов - Numbers and special characters are not allowed. 
- Если поле оставить пустым и нажать на кнопку Submit должно появиться сообщение - Last Name must not be blank.

5. Mobile number
- Можно ввести только цифры. 
- Требований к ограничению длины нет. 
- При вводе спецсимволов - Special characters are not allowed. 
- При вводе букв - Characters are not allowed. 
- При вводе букв и спецсимволов - Numbers and special characters are not allowed. 
- Если поле оставить пустым и нажать на кнопку Submit должно появиться сообщение - Mobile must not be blank.