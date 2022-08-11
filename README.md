# Final_Project_Labirint
Тестирование функционала интернет-магазина Лабиринт https://www.labirint.ru/

Автотесты выполнены на Python 3.10 с применением Pytest и Selenium, используется браузер Chrome.

В папке pages находятся файлы, содержащие классы и методы для работы с сайтом, а также локаторы (locators) и список url (url_list).

В папке tests находятся автотесты, папка с полученными в результате тестирования скриншотами (screenshots), файл conftest с фикстурами для запуска драйвера.

Файлы автотестов:
test_home_page.py - проверяют страницу авторизации
test_header.py - проверяют работу кнопок меню в header
test_header_search.py - проверяют работу строки поиска в header
test_main_page.py - проверяют корректность загрузки главной страницы сайта.

Команды для запуска тестов:

python -m pytest -v --driver Chrome --driver-path C://chromedriver/chromedriver.exe /tests/test_home_page.py
python -m pytest -v --driver Chrome --driver-path C://chromedriver/chromedriver.exe /tests/test_header.py
python -m pytest -v --driver Chrome --driver-path C://chromedriver/chromedriver.exe /tests/test_header_search.py
python -m pytest -v --driver Chrome --driver-path C://chromedriver/chromedriver.exe /tests/test_main_page.py

где C://chromedriver/chromedriver.exe находится путь к драйверу Selenium для текущей ОС
