Структура серверів яку планую реалізувати в проекті olx аналіз.
![[olx_server.png]]
файл xml:
![[olxserver.drawio]]
Olx Client: [[olx client]]
Olx Main: [[olx_sv main serv]]
Olx Analiz: [[olx_sv analiz serv]]
Olx Manager Db: [[olx_sv manager db]]
Olx Db: [[olx_sv db]]
### + Структури
Завдяки такій структурі це все можна буде легко маштабувати.
Olx Analiz цей сервер він не буде один. Кожен буде аналізувати свою катигорію що збільшить швидкість аналізу.
Manager Db цей сервер відповідає за те щоб правильно розприділяти дані по базама. Це збільшить швидкість пошуку,додавання і тд.
Olx Main і Olx Manager db будуть теж говорити. 
Olx Main треба говорити з Olx Manager db для того щоб отримувати про аналізованні товари та відсилати їх Olx Client.
[[olx аналіз]]