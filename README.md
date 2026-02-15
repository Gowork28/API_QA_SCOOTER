
# Тестирование API для сервиса Яндекс Самокат

Яндекс Самокат - это сервис аренды самокатов. 
Самокат доставляет курьер в указанный день. Можно выбрать цвет самоката и срок аренды. 

В этом проекте реализованы автоматизированные тесты для ключевых функций API сервиса Яндекс Самокат. Протестированы как позитивные, так и негативные сценарии. Проверки проходили с помощью сравнения кода и статуса ответа, тела ответа.

## Проверенные функции

- **Создание курьера** – проверка возможности регистрации нового курьера.  
- **Логин курьера** – проверка авторизации курьера по логину и паролю, включая негативные сценарии.  
- **Удаление курьера** – тестирование удаления курьера по ID.  
- **Создание заказа** – проверка возможности создания нового заказа на самокат с различными параметрами (адрес, цвет, дата доставки и др.).  
- **Принятие заказа** – проверка возможности курьера принять заказ.  
- **Получение заказа по номеру (track)** – тестирование запроса заказа по уникальному номеру.  
- **Получение списка заказов** – проверка получения всех заказов в системе.

## Стек:
<div align="left">
  <img src="https://img.shields.io/badge/ApiDoc-009688?style=for-the-badge&logo=readthedocs&logoColor=white" alt="ApiDoc"/>
  <img src="https://img.shields.io/badge/Postman-FF6C37?style=for-the-badge&logo=postman&logoColor=white" alt="Postman"/>
  <img src="https://img.shields.io/badge/PyCharm-000000?style=for-the-badge&logo=pycharm&logoColor=white" alt="PyCharm"/>
  <img src="https://img.shields.io/badge/Selenium-43B02A?style=for-the-badge&logo=selenium&logoColor=white" alt="Selenium"/>
  <img src="https://img.shields.io/badge/Allure-FF8C00?style=for-the-badge&logo=allure&logoColor=white" alt="Allure"/>
  <img src="https://img.shields.io/badge/Pytest-0A9EDC?style=for-the-badge&logo=pytest&logoColor=white" alt="Pytest"/>
  <img src="https://img.shields.io/badge/JSON-000000?style=for-the-badge&logo=json&logoColor=white" alt="JSON"/>
</div>

## Инструкция по запуску:

1. Установите зависимости:
pip install -r requirements.txt

2. Запустить все тесты и записать отчет:
pytest tests --alluredir=allure_results

3. Посмотреть отчет по прогону html
allure serve allure_results
