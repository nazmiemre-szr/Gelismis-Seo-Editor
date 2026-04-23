# Gelismis-Seo-Editor
Wordpress Gelişmiş Seo Editör
+ Kategori Açıklamalarını Editörle zenginleştirebilirsiniz. 
+ Oluşturulan kategorilere Meta Title ve Desc ekleyebilirsiniz. (AIOSEO Ücretli versiyonda var.)
+ Meta Title ı olmayan Post, Page ve Category lere title sonrası otomatik ilave title ekleme (AIOSEO de olan hoşuma giden özellik)
+ Eğer daha önceden AIOSEO kullanıyorsanız ve kaldırmak istiyorsanız, AIOSEO'dan eski title ve descp leri çeker.
+ Sabit sayfalardan tarihleri kaldırmam seçeneği
+ Plugın, tema ve wordpress in Meta Generator etiketlerinin tamamını kaldırır.


Temanın archvives.php dosyasında
//bu kodu bulup <?php
        if( have_posts() ) :
//kod sonu
bu satırdan önce aşağıdaki satırı ekle


// Kategori sayfasındaysak ve bir kategori açıklaması varsa göster
if ( is_category() && category_description() ) : 
?>
    <div class="ozel-kategori-aciklamasi" style="margin-bottom: 30px;">
        <?php echo category_description(); ?>
    </div>
<?php endif; ?>
// Kategori sayfasındaysak ve bir kategori açıklaması varsa göster
       
