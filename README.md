# ImageCaptioning

Bu projede OBSS şirketinin sağlamış olduğu veri ile image captioning(görsele altyazı üretme) görevi yapan bir model oluşturmak hedelenmiştir.

Bu problemler için encoder + decoder ile veri çözülür elde edilen özellikler ile decoder ile kelimeler üretilir.

Model yapısında encoder olarak Swin S Transformer ı pretrained şekilde alındı.Daha sonra decoder boyutuna uyumlu olması için bir lineer katman ve son olarak decoder olarakta transformers kütüphanesi ile oluşturduğum transformer decoder var.

Özelliklerin kelimelere çevrilmesi için Distil-Bert kullanılmıştır.

Modelde encoder güçlendirilerek ve daha uygun bir tokenizer tercih edilerek daha tutarlı ve anlamlı caption lar üretilebilir.

Sonuç başarısı gte-small metriği ile ölçülüp 0.24 loss dur.
