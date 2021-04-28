# Learning XOR mapping with a MLP using TF (Keras)
En başta bu kodda kullanacağımız **fonksiyonları** çağıracağımız **kütüphaneleri** dahil ediyoruz.</br>
First we import the **libraries** to use the **functions** that we are going to invoke in this code.</br>
```
import tensorflow as tf
import matplotlib.pyplot as plt
import numpy as np # numerical python kütüphanesi
import pandas as pd
import sys
from numpy import random
```

Bildiğimiz gibi, *XOR* problemi *Elektrik-Elektronik Mühendisliğinde* mantıksal devreler (**logic circuits**) alanında karşımıza çıkan bir problem. İki girişli ve tek çıkışlı (**two input one output**) bir sistemin girişleri *TRUE-FALSE* (veya *1-0* veya *HIGH-LOW*) olarak isimlendirilen *Boolean* veri tipinde değer alıyorlar. Benzer şekilde çıkış da yine *1-0* Boolean değişkenlerinden birisi oluyor.


Aşağıda **numpy** kütüphanesi kullanarak giriş (**input**) ve hedef (**target**) verilerini oluşturduk. Dikkat edin, burada hedef verisine İngilizce'de **annonation** deniyor. Yani bizler hedef değişkenini oluşturduğumuzda giriş verisini **annotate** etmiş (etiket - **label**) oluyoruz.
