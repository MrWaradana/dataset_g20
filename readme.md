# ANALISIS SENTIMEN MENGENAI KONFERENSI TINGKAT TINGGI G20 BALI 2022 DI TWITTER

## Summary

> Indonesia pada tahun ini berkesempatan untuk memimpin presidensi Gerakan 20 negara dengan mengusung tema semangat bersama pulih bersama. Untuk mensukseskan acara ini, pemerintah dan masyarakat bekerjasama untuk mempersiapkan berbagai hal dalam mendukung Indonesia sebagai tuan rumah hingga akhir november mendatang. Tujuan dari penelitian ini untuk menganalisis respon masyarakat terhadap kepemimpinan Indonesia dalam memimpin G20 ditengah gejolaknya bencana ekonomi dan perang. Dalam analisis ini kami mendapatkan data dari twitter sebanyak 1066 untuk selanjutnya mengelompokkan masyarakat yang mendukung sebanyak 47.6%, netral sebanyak 47.1% , dan tidak mendukung sebanyak 5.3% dengan tingkat akurasi mencapai 90%. Dengan ini dapat disimpulkan bahwa masyarakat cenderung mendukung terselenggaranya berbagai acara KTT G20.

# How to?

## Langkah dalam menggunakan code python untuk sentimen analisis :

1. Crawling data twitter dengan menggunakan library twint (ikuti alur yang ada di [1_crawling_data_g20](/1_crawling_data_g20.ipynb))
2. Cleansing data raw dengan menghilangkan karakter yang diinginkan (ikuti alur yang ada di [2_cleansing_data_g20](/2_cleansing_data_g20.ipynb))
3. Proses data _teks_ menjadi kata yang baku dan menghilangkan kata slang (ikuti alur yang ada di [3.0_text_processing_data_g20](/3.0_text_processing_data_g20.ipynb))
4. Translate hasil proses data ke Bahasa Inggris dengan google sheets
   > TextBlob tidak bisa membuat sentimen dengan bahasa Indonesia
5. Proses data _teks_ yang telah _ditranslate ke bahasa inggris_ menjadi kata yang baku dan menghilangkan kata slang (ikuti alur yang ada di [3.4_text_processing_translated_data_g20](/3.4_text_processing_translated_data_g20.ipynb))
6. Lakukan sentimen analisis dengan library _TextBlob_ [4_sentiment_analysis_data_g20](/4_sentiment_analysis_data_g20.ipynb))
7. Lakukan training dan testing model untuk mengetahui akurasi dari model yang digunakan menggunakan library _sklearn_ [4_sentiment_analysis_data_g20](/4_sentiment_analysis_data_g20.ipynb))
8. Hasil didokumentasikan untuk melihat analisis sentimen
