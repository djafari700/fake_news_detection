# تشخیص اخبار دروغین

در فایل news_train.csv اطلاعات کلی مانند زمان انتشار، منبع و برچسب خبر آمده است؛ اما خود خبر را در این مجموعه‌داده نداریم. بلکه خود خبر را می‌توان در فایل news_train_text_vectors.npz جستجو کرد. اما درnews_train_text_vectors.npz متن خبر قرار نگرفته است، بلکه به کمک روش‌های پردازش زبان طبیعی، متن هر خبر را به یک بردار ۴۲۱۴۱ المانی تبدیل کرده‌ایم و به ازای هر خبر، یک بردار با ابعاد ( (42141, 1وجود دارد.

