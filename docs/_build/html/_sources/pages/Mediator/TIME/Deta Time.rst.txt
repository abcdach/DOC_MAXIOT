

Deta Time
---------------------
მოცემული პითონის კოდი გამოიმუშავებს 0 გამოსასვლელზე - თარიღს და დროს

.. code-block:: python
 :linenos:

 #{"_DES_":"Deta Time"}
 #{"_PER_":"1"}
 #{"_OUT_0_DES_":"DATA OUT"}
 #{"_IN_0_PUSH_":"0"}

 import time
 UNIX_TIME = int(time.time())
 import datetime
 local_time = (+4)
 timestamp = int(UNIX_TIME) + (60*60*local_time)
 value = datetime.datetime.fromtimestamp(timestamp)
 x =(value.strftime('%d/%m/%Y %H:%M:%S'))
 OUT_0 = str(x)
