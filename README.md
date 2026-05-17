<a target="_blank" href="https://colab.research.google.com/github.com/syamaniulm/hand_flood/blob/main/Hand_Based_Flood_Depth_Modeling.ipynb">
  <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/>
</a>

# Estimasi Cepat Sebaran Genangan Banjir

Pernahkah Anda bertanya atau membayangkan? Ketika ada yang mengukur kedalaman genangan banjir pada suatu titik koordinat, sampai dimanakah kira-kira sebaran genangannya? Dan seperti apa sebaran kedalamannya?<br>

<html>
  <body>
    <div>
       <img src="flood_depth_measurement.png" alt="Flood Depth Measurement Illustration"  style="width:600px;">
      </a>
    </div>
  </body>
</html>

Dengan mengintegrasikan antara data topografis, yaitu Height Above Nearest Drainage (HAND) dan data koordinat kedalaman genangan banjir lapangan, pertanyaan-pertanyaan seperti di atas dapat terjawab. Dengan kata lain, dengan menggunakan data koordinat dan kedalaman banjir eksak dari lapangan, kita dapat mengestimasi luas dan sebaran kedalaman genangan banjir.<br>

## Petunjuk Penggunaan

Sumber data lapangan harus berisi data koordinat dalam lintang bujur, dan data kedalaman genangan banjir untuk setiap koordinat dalam satuan meter. Data dibuat dalam bentuk tabel dan disimpan dalam format CSV. Karena kode program disiapkan untuk dijalankan menggunakan Google Colab, maka file CSV harus disimpan di dalam Google Drive. Jika kode program dijalankan menggunakan Jupyter Lab atau VS Code, maka harus ada penyesuaian pada beberapa bagian kode. Ikuti format tabel yang dicontohkan pada file ```Flood_Locations.csv```.<br>

Di dalam tabel wajib ada kolom ```Long``` yang berisi data bujur dalam decimal degree, ```Lat``` yang berisi data lintang dalam decimal degree, dan ```Depth``` yang berisi data kedalaman banjir dalam satuan meter. Format penulisan huruf besar dan kecil untuk nama-nama kolom ini harus persis sebagaimana contoh. Jika ada perubahan format penulisan, maka harus ada penyesuaian pada beberapa bagian kode.

### Persyaratan

Anda harus memiliki akun Google Earth Engine untuk menjalankan kode program ini.


### Penafian

Kode program ini merupakan proyek eksperimental. Sehingga masih memerlukan validasi di lapangan.

### Petunjuk Sitasi

Penggunaan HAND di dalam dokumen resmi wajib mengutip literatur ini: <a href="https://www.sciencedirect.com/science/article/abs/pii/S0022169411002599">https://www.sciencedirect.com/science/article/abs/pii/S0022169411002599</a>
