**Тестове завдання**

У моєму тестовому завданні я виконав такі завдання:
1. Реалізував зміну роботи Web API Canvas, а саме методоа fillRect(), для того, щоб малювання прямокутника завжди повертало змінені значення пікселів. Тобто, щоб у створеному зображенні кожен піксель був змінений на випадкове значення в межах ±5 від оригінального кольору. Зміни знаходяться [у цьому](src/third_party/blink/renderer/modules/canvas/canvas2d/base_rendering_context_2d.cc) файлі. <br>
  Також ось посилання на змінені ділянки коду:
    - [зміна 1](src/third_party/blink/renderer/modules/canvas/canvas2d/base_rendering_context_2d.cc#L26)
    - [зміна 2](src/third_party/blink/renderer/modules/canvas/canvas2d/base_rendering_context_2d.cc#L1767-L1822)
2. Додав можливість збереження і завантаження cookies з JSON-файлу. Формат файлу: `[{"name":"example","value":"value123","domain":".example.com" }]`. Зміни знаходяться [у цьому](src/content/browser/storage_partition_impl.cc) файлі. <br>
    Реалізував 2 методи:
    - [Завантаження cookies у браузер із JSON файлу](src/content/browser/storage_partition_impl.cc#L187-L244)
    - [Збереження поточних cookies у JSON файл](src/content/browser/storage_partition_impl.cc#L248-L276) <br>
Також ось посилання на змінені ділянки коду:
    - [зміна 1](src/content/browser/storage_partition_impl.cc#L3578-L3584)
    - [зміна 2](src/content/browser/storage_partition_impl.cc#L3240-L3246)
3. Змінив логіку RTCPeerConnection так, щоб під час створення WebRTC-з'єднання браузер завжди повідомляв IP-адресу 192.0.2.1. Зміни знаходяться [у цьому](src/third_party/blink/renderer/modules/peerconnection/rtc_peer_connection.cc#L2351-L2360) файлі. <br>
4. Свій кастомізований браузер не зібрав, оскільки збірка триває вже 3 дні і невідомо, скільки вона ще триватиме. Тому цей код не протестований


Інструкція по збірці браузеру <br>
Скопіювати папку `srs` в папку з вихідним кодом Chromium <br>
`git clone https://github.com/Bruvamasc/Test_task_1.git`
