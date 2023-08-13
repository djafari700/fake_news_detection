# تشخیص اخبار دروغین
بخش «پردازش زبان طبیعی» از قیل انجام شده است 
برای حل این مسئله از کتابخانه های زیر کمک گرفتیم
import numpy as np
import pandas as pd 
import scipy.sparse as ss
from sklearn.model_selection import train_test_split
from sklearn.svm import SVC
from sklearn.decomposition import PCA
from sklearn.metrics import classification_report, f1_score



    <br>
    در فایل <code>news_train.csv</code> اطلاعات کلی مانند زمان انتشار، منبع و برچسب خبر آمده است؛ اما خود خبر را در این مجموعه‌داده نداریم. بلکه خود خبر را می‌توان در فایل <code>news_train_text_vectors.npz</code> جستجو کرد. اما در <code>news_train_text_vectors.npz</code> متن خبر قرار نگرفته است، بلکه به کمک روش‌های پردازش زبان طبیعی، متن هر خبر را به یک بردار ۴۲۱۴۱ المانی تبدیل کرده‌ایم و به ازای هر خبر، یک بردار با ابعاد <code>(42141, 1)</code> وجود دارد.
    <br>
