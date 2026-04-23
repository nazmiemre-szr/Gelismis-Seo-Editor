# Gelismis-Seo-Editor
Wordpress Gelişmiş Seo Editör


Temanın archvives.php dosyasında
 <?php
        if( have_posts() ) :
        bu satırdan önce aşağıdaki satırı ekle


// Kategori sayfasındaysak ve bir kategori açıklaması varsa göster
if ( is_category() && category_description() ) : 
?>
    <div class="ozel-kategori-aciklamasi" style="margin-bottom: 30px;">
        <?php echo category_description(); ?>
    </div>
<?php endif; ?>
       
