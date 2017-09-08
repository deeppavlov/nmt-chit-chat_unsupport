# Neural Machine Translation (seq2seq) for chit-chat

#### Model

```
wget  http://share.ipavlov.mipt.ru:8080/repository/models/chitchat/nmt-chit-chat-v0.1.2.tgz
export CHITCHAT_MODEL=<PATH_TO_MODEL>
```
#### Example
```
from nmt import interface
import os

model_path = os.environ.get("CHITCHAT_MODEL")
interface.init(model_path)

while True:
    q = input("[Ваш вопрос]> ")
    r = interface.send(q)
    print("[Ответ]> %s" % r[0])

```
