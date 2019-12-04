Здесь собраны вместе идеи проектов.


# Идеи проектов по беспилотникам

## kagle baidoo 3d pose estimation
    - how is that applicable to appolo/autoware ? Do they do the same processing at some stage ?
    - плюсы
        - тренировка себя в области CV/ML
        - строчка в резюме, ачивка
    - минусы
        - как это применить к нашим проектам ?
    - задачи

## indoor car (follow/capture a person)
    - no lidar applicable, but stereo
    - плюсы
        - можно тестировать, не отходя от компа 
        - проще в создании, программировании. Позволяет опробовать базовые системы локализации, навигациии и.т.д.
        - можно построить распределенную систему, вынести ресурсоемкие модули в облако.
    - минусы
        - мало общего с работой в условиях дороги/города. Решает другие, упрощенные задачи.
    - задачи
        - generate HD maps
        - what stack to use? appolo/autoware/custom ?

## outdoor car (pizza delivery)
    - no lidar applicable (too expensive), but stereo
    - плюсы
        - проще в создании, программировании. Позволяет опробовать базовые системы локализации, навигациии и.т.д.
        - решает похожие задачи, что и беспилотные авто: локализация на HD карте, распознавание дорог/тротуаров, участие в ПДД
    - минусы
        - нельзя построить распределенную систему, вынести ресурсоемкие модули в облако.
        - придется испытывать на улице
    - задачи
        - generate HD maps

## contribute to starline/apollo
    - плюсы 
        - перспекива найти работу если оценят твой вклад
        - практический опыт интеграции production-grade стека
        - работа над беспилотными авто, а не чем-то другим. Возможность получить доступ к дорогому оборудованию.
    - минусы
        - твой труд уйдет к другим забесплатно
        - софт для авто все-равно придется адаптировать если делать что-то еще, например робот доставки пиццы 
        - проверить можно только в симуляторе. Apollo/autoware обязательно требуют лидар, много лидаров.  Appolo Lite нет! 
    - задачи
        - generate HD maps ?
        - run simulation with Russian world/signs/rules, identify shortcomings
            - do they need better recognition ? How Kaggle competition is applicable here ?
                * идентификации элементов дорожной инфраструктуры
                * сценариев поведения для российских пдд

## Другие варианты
    - изучить работу autoware/appolo со стерео-камерой
    - построить свой небольшой робот на упрощенном стеке 
    - улучшить работу apollo/autoware в специальных условиях. Например, automatic valet parking.
    - HD карты похоже будут очень востребованы. Можно начать создавать их уже сейчас. Также они нужны для проекта Outdoor car.



# Ссылки:

**kaggle**: 
    https://www.kaggle.com/c/pku-autonomous-driving


**starline**
    Appolo
        https://github.com/apolloauto
        https://github.com/ApolloAuto/apollo

        https://classroom.udacity.com/courses/ud0419
        https://github.com/ApolloAuto/apollo/blob/master/docs/howto/how_to_understand_architecture_and_workflow.md
        http://apollo.auto/devcenter/devcenter.html

    run simulation, get data for Russian environments
        Simulation Dreamland
            https://azure.apollo.auto/?locale=en-us
        Carla Local
        file:///home/usr/car/nemodrive-apollo-latest.pdf
    News
        https://www.reddit.com/r/SelfDrivingCars
        https://twitter.com/starline_oscar
    RICAR https://smartcar.starline.ru/ricar/
    OSCAR https://smartcar.starline.ru/oscar/
    https://gitlab.com/starline/oscar/wikis/home
    https://smartcar.starline.ru/category/publications/articles/
    В ближайших планах:
        1. Развитие системы компьютерного зрения для улучшения системы идентификации и локализации препятствий и дополнения системы локализации.
        2. Развитие системы идентификации элементов дорожной инфраструктуры и сценариев поведения на базе российских ПДД.        
        ------from README ----- 
        Разработка математических библиотек для обработки данных от выбранных датчиков.
        Разработка LTE модуля для взаимодействия с сервером.
        Разработка серверного ПО и пользовательских приложений.
    