# NFC-MusicPlayer
Project of an NFC module for controlling a music player. Features include music playback, album switching, and volume control.
![IMG20250822135023](https://github.com/user-attachments/assets/25920482-cfb0-494b-8d40-a1ed8fb28eb3)
Цей проєкт реалізує NFC-керування музичним плеєром за допомогою модуля ESP32-C3 та прошивки ESPHome. Пристрій дозволяє:

Зчитувати NFC-мітки (RC522 через SPI!!!щоб модуль NFC запрацював потрібно додати резистор 10 кОм між пінами 3,3В і RST!!!) для запуску відтворення музики.

Перемикати альбоми через кнопку енкодера.

Керувати гучністю за допомогою енкодера.

Передавати події до Home Assistant для автоматизацій.

Відображати статус роботи через світлодіод.

Основні можливості

Підтримка Home Assistant: автоматичне відправлення подій nfc_tag_scanned, nfc_tag_removed та album_next.

Регулювання гучності через енкодер у режимі реального часу.

Світлодіодний індикатор стану Wi-Fi та NFC.
Вибір альбомів і виконавців та їх перемикання здійснюється за допомогою автоматизацій:1) NFC Player - Відтворення виконавців. 2) NFC Наступний альбом. 3) NFC зупинити музыку якщо забрали мітку.
Потрібно буде створити помічники: input_text.last_album_played, input_text.last_tag_id.

English

NFCPlayer – Music Control via NFC and ESPHome

This project implements NFC-based music control using an ESP32-C3 board and ESPHome firmware. The device allows:

Reading NFC tags (RC522 via SPI !!!to make the NFC module work, you need to add a 10 kΩ resistor between the 3.3 V and RST pins!!!.) to trigger music playback.

Switching albums via an encoder button.

Controlling volume using a rotary encoder.

Sending events to Home Assistant for automation.

Indicating system status with an LED.

Key Features

Home Assistant integration: automatically sends nfc_tag_scanned, nfc_tag_removed, and album_next events.

Real-time volume control via rotary encoder.

LED indicator for Wi-Fi and NFC status.
Selection of albums and artists, as well as switching between them, is handled through automations:

NFC Player – Play Artists.

NFC – Next Album.

NFC – Stop Music When Tag Is Removed.

You will need to create helpers: input_text.last_album_played, input_text.last_tag_id.


## Підтримати проект ☕

Якщо вам подобається цей проєкт і ви хочете підтримати кавою, ви можете використати один із способів нижче:

https://ko-fi.com/eugeneshcherbakov
