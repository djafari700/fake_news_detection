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



در فایل news_train.csv اطلاعات کلی مانند زمان انتشار، منبع و برچسب خبر آمده است؛ اما خود خبر را در این مجموعه‌داده نداریم. بلکه خود خبر را می‌توان در فایل news_train_text_vectors.npz جستجو کرد. اما درnews_train_text_vectors.npz متن خبر قرار نگرفته است، بلکه به کمک روش‌های پردازش زبان طبیعی، متن هر خبر را به یک بردار ۴۲۱۴۱ المانی تبدیل کرده‌ایم و به ازای هر خبر، یک بردار با ابعاد ( (42141, 1وجود دارد.

