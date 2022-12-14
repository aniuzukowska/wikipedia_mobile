## Проект автоматизации тестирования мобильного приложения "Wikipedia"
<img width="1162" alt="image" src="https://user-images.githubusercontent.com/109241600/207922538-dab0b3f0-a6e6-4474-8e1d-7b4f6d1f0daa.png">

## Содержание
+ [Технологии и инструменты](#Технологии)
+ [Тест-кейсы](#Тесты)
+ [Запуск автотестов из Jenkins](#Jenkins) 
+ [Оповещение о результатах через Telegram-бот](#Telegram) 
+ [Отчеты о прохождении тестов Allure report](#Allure) 
+ [Интеграция с Allure TestOPS](#TestOPS) 
+ [Интеграция с Jira](#Jira) 



<a name="Технологии">
  
## Технологии и инструменты, использованные в проекте
<p align="center">
<img width="6%" title="PyCharm" src="wikipedia_mobile_tests/utils/images/pycharm.svg">
<img width="6%" title="Python" src="wikipedia_mobile_tests/utils/images/python.svg">
<img width="6%" title="Pytest" src="wikipedia_mobile_tests/utils/images/pytest.svg">
<img width="6%" title="Selenium" src="wikipedia_mobile_tests/utils/images/selenium.png">
<img width="6%" title="Selene" src="wikipedia_mobile_tests/utils/images/selene.png">
<img width="6%" title="GitHub" src="wikipedia_mobile_tests/utils/images/GitHub.svg">
<img width="6%" title="Jenkins" src="wikipedia_mobile_tests/utils/images/Jenkins.svg">  
<img width="6%" title="AllureReport" src="wikipedia_mobile_tests/utils/images/Allure_Report.svg">  
<img width="6%" title="AllureTestOPS" src="wikipedia_mobile_tests/utils/images/Allure_TO.svg"> 
<img width="6%" title="Telegram" src="wikipedia_mobile_tests/utils/images/Telegram.svg">  
<img width="6%" title="Jira" src="wikipedia_mobile_tests/utils/images/jira.svg"> 
<img width="6%" title="Browserstack" src="wikipedia_mobile_tests/utils/images/Browserstack.svg"> 
<img width="5%" title="Appium" src="wikipedia_mobile_tests/utils/images/Appium.svg"> 
</p>

  
<a name="Тесты">
  
## Тест-кейсы
  - Поиск информации
  - Возврат на главную страницу из результатов поиска
  - Переход на страницу с настройками
  - Возврат на главную страницу со страницы настроек
  

  
<a name="Jenkins">

## Запуск автотестов из Jenkins
Для удаленного запуска автотестов в <a href="https://jenkins.autotests.cloud/job/002-annazukowska-python-wikipedia-mobile/" target="_blank">Jenkins</a> создана задача (job), настроена и связана с репозиторием в GitHub.
<img width="1437" alt="image" src="https://user-images.githubusercontent.com/109241600/207936123-2dd2443b-6529-46d4-9136-aba01d4b175f.png">



<a name="Telegram">
  
## Уведомление о результатах тестирования через Telegram-бот
После завершения тестов приходит такое оповещение в Telegram с помощью заранее созданного Telegram-бота, привязанного к задаче в Jenkins.

<img width="349" alt="image" src="https://user-images.githubusercontent.com/109241600/207936849-0bb509ae-d923-4799-b8cc-98c4687306b8.png">


  
<a name="Allure">
  
## Отчеты о прохождении тестов Allure report
После завершения тестов также формируются отчеты <a href="https://jenkins.autotests.cloud/job/002-annazukowska-python-wikipedia-mobile/8/allure/#suites/af2ff67a81e1e0c79ebbaa1e8fbd90b7/3cc0d59c8d44980e" target="_blank">Allure report</a>, которые можно посмотреть со страницы задачи в Jenkins.

<img width="1432" alt="image" src="https://user-images.githubusercontent.com/109241600/207937388-8683e93d-d9f9-4c1f-913c-e5885b31df1d.png">
<img width="1431" alt="image" src="https://user-images.githubusercontent.com/109241600/207937465-602917f9-ae85-4135-ad37-7298bdd53b49.png">


  
<a name="TestOPS">
  
## Интеграция с Allure TestOPS
Настроена интеграция Jenkins с Allure TestOPS.
При первом после интеграции прохождении тестов в Jenkins, в Allure TestOPS были автоматически созданы такие тест-кейсы:

<img width="1432" alt="image" src="https://user-images.githubusercontent.com/109241600/207939178-cb06c9c6-2842-4ab4-8d22-97d180bf3901.png">

Можно посмотреть историю выполненных прогонов:
<img width="1435" alt="image" src="https://user-images.githubusercontent.com/109241600/207939857-d6c2643c-0ef4-4a9d-9b38-864352226e4a.png">
<img width="1432" alt="image" src="https://user-images.githubusercontent.com/109241600/207940026-d465a021-1f23-4b90-83d7-82df2a73ffed.png">


  
<a name="Jira">
  
## Интеграция с Jira
Настроена интеграция Allure TestOPS с Jira. К задаче в Jira привязаны тест-кейсы и прогон с результатами тестирования из Allure TestOPS.

<img width="1433" alt="image" src="https://user-images.githubusercontent.com/109241600/207941082-8a70a718-f42d-4835-abfb-75673ca933cb.png">
<img width="1435" alt="image" src="https://user-images.githubusercontent.com/109241600/207941141-5babd837-6457-4eb1-b163-73c3d0493a8e.png">





