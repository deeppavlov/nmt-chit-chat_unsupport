# Neural Machine Translation (seq2seq) for chit-chat

#### Model

```
wget  http://share.ipavlov.mipt.ru:8080/repository/models/chitchat/nmt-chit-chat-v0.1.2.tgz
export CHITCHAT_MODEL=<PATH_TO_MODEL>
```
#### Example
```
from nmt import interface

interface.init('{PATH}/model')

answer = interface.send('Здравствуйте, нет заисления зарплаты по реестру 9 от 31.03.17 года, реестр висит со вчерашнего дня?')


```
