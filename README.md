# TestEcsLite

## Количество часов потраченных на разработку

Потрачено 11 часов

## Серверная симуляция

Для симуляции на сервере необходимы следующий системы: 

* EntityMovementSystem
* DoorCheckStateSystem
* DoorOpenSystem
* ButtonCollisionSystem
    
Данные системы необходимы для полной симуляции мира. Они будут работать уже на созданном мире(двигать игрока, проверять колизии с кнопкой и открывать двери). Сейчас мир создается на клиенте и с зависимостями на юнити. Так же в них есть зависимости на UnityEngine, а именно на Vector3 и Time.deltaTime. По тз их можно использовать, но для работы этих систем на сервере без юнити надо это править либо писать обвязку для них. 

Так же все, что связано с Ecs лежит в папке Assets/Script/Logic.Ecs. Компоненты и системы разнесены по папкам Client и Server для удобства.
  
