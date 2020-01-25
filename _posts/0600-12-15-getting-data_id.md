---
layout: doc
title: Mendapatkan Data OSM
permalink: /en/osm-data/getting-data/
lang: id
category: osm-data
---

Mendapatkan Data OSM
=================  

> Diperiksa 2016-04-05

Ketika Anda ingin mendapatkan data OpenStreetMap yang paling terbaru, cara paling mudah untuk mendownloadnya adalah dengan mengekspor dari sebuah situs. Ada beberapa jenis situs layanan yang menyediakan ekspor data untuk area yang Anda tentukan.   

Men-download Data OSM
--------------------------

### GeoFabrik

[GeoFabrik](http://geofabrik.de) adalah perusahaan spesifik yang bekerja dengan menggunakan OpenStreetMap. Mereka menyediakan jenis data spasial dalam bentuk shapefile dan raw data OSM dalam situs [download website](http://download.geofabrik.de). Keunggulan men-download data dari GeoFabrik adalah data diperbaharui setiap hari, mudah dan dapat dipercaya. Salah satu kelemahannya adalah data yang disediakan berdasarkan batas negara, dan tidak semua negara tersedia datanya.  

### BBBike  

[BBBike](http://download.bbbike.org/osm/bbbike/) menyediakan shapefile dan format data OSM untuk kota-kota di dunia, data diperbaharui perminggu. Situs ini dapat digunakan jika Anda ingin melihat data berdasarkan batas kota/kabupaten.

>Hal yang harus diingat yaitu beberapa fitur di dalam OpenStreetMap memiliki "free" tags dengan jumlah huruf yang tidak terbatas,
>tetapi shapefiles memiliki penyimpanan atribut dengan jumlah huruf yang terbatas pada atribut kolom. Ini berarti
>ketika data OSM akan diubah ke dalam shapefile, hanya tag spesifik yang akan 
>termasuk ke dalam tabel atribut shapefile. Pada situs ini hanya menyediakan shapefile
>dengan tags default yang pada umumnya digunakan, tetapi jika Anda ingin mendapatkan shapefile dengan tag spesifik
>Anda dapat menggunakan situs layanan yang lebih spesifik yang dapat memilih tag tertentu pada sub bab berikutnya
>atau Anda dapat mempelajari bagaimana cara mengekspor data.

Kustomisasi Data
-------------------

### HOT Exports  

The [Humanitarian OpenStreetMap Team](http://hotosm.org) telah membuat sebuah layanan yang memungkinkan pengguna untuk memilih sebuah wilayah yang ingin diambil datanya dengan menggunakan [JOSM Presets](/en/josm/josm-presets/)
untuk memilih tags yang diinginkan yang akan tersaring di dalam proses ekspor. Layanan ini tersedia untuk semua negara dimana HOT bekerja, situs tersebut yaitu [export.hotosm.org](http://export.hotosm.org).

![hot exports][]

### BBBike  

Anda dapat memilih wilayah yang spesifik yang Anda inginkan dengan menggunakan [http://extract.bbbike.org/](http://extract.bbbike.org/). Kelemahan dari layanan ini yaitu Anda tidak dapat memilih tag yang di kustomisasi dan jumlah data yang Anda download akan terbatas.  

### Overpass

Overpass API (Application Programming Interface) adalah untuk mengekstrak data dari server OpenStreetMap yang akan sesuai dengan jumlah data yang dihasilkan. Dengan menggunakan kueri Anda dapat mengkustomisasi bagian data yang Anda peroleh. Anda dapat juga menggunakan API secara langsung dengan menghasilkan sebuah http-request atau melalui tampilan overpass turbo. 

#### Overpass Turbo

[Overpass Turbo](http://overpass-turbo.eu/) adalah sebuah kueri generator yang interaktif dimana Anda harus memperbesar peta dan memilih wilayah yang Anda inginkan. Masukkan kueri Anda di kotak sebelah kiri dari halaman dan gunakan beberapa menu yang terdapat di bagian atas halaman. Jika Anda baru menggunakan bahasa kueri, klik pada bagian wizard untuk memulai. OSM wiki berisi konten [deskripsi lebih lanjut](http://wiki.openstreetmap.org/wiki/Overpass_API/Overpass_QL) dari sintaksis bahasa kueri yang sama dengan [contoh](http://wiki.openstreetmap.org/wiki/Overpass_API/Overpass_API_by_Example).

Peta akan menampilkan semua data yang diseleksi dengan kueri yang nantinya bisa Anda modifikasi. Tekan "Run" untuk memperbaharui tampilan. Jika Anda telah selesai klik "Export" akan menampilkan jumlah data, diantara raw data OSM. Jika jumlah data terbatas, Anda dapat mengaksesnya dengan memindahkan diantara tampilan peta dan tampilan data degan menggunakan tombol di sisi bagian atas. Pilihan eskpor *Query -> compact OverpassQL* akan memproses hyperlink yang digunakan untuk Overpass API. 

![overpass turbo][]

If you want to engineer a fancy query in order to obtain a subset of the data from a large area then it is a good idea to test and improve this query in Overpass Turbo on a small area. You can then zoom out to your complete region of interest and use the resulting query url directly for the API. The next section explains how you can do this.

#### Overpass API

[Overpass API](http://wiki.openstreetmap.org/wiki/Overpass_API) is a dedicated service optimized for querying but not writing OpenStreetMap data. Due to this optimization it operates very fast compared to the main database api and has virtually no limits on the amount of data transferred. Several instances of this service are available on the net, the one used in the following example also provides some information on [its homepage](http://overpass-api.de/)

If you have a working query-URL for submitting an http-request to the Overpass API then a tool such as [wget](https://www.gnu.org/software/wget/) - available for different operating systems, see [here](http://wget.addictivecode.org/FrequentlyAskedQuestions?action=show&redirect=Faq#download) - allows you to download the raw OSM data directly from the server and store them locally. The following snippet is a script for the bash shell common on Unix systems which obtains all data within a specified bounding box:

```
echo lower left latitude
read ll_lat
echo lower left longitude
read ll_lon
echo upper right latitude
read ur_lat
echo upper_right longitude
read ur_lon
echo output file
read file
url="http://overpass-api.de/api/interpreter?data=(node($ll_lat,$ll_lon,$ur_lat,$ur_lon);<;rel(br););out meta;"
wget -O $file "$url"
```
>What happens here (for the curious who do not want to read the full query language documentation)?  
>node(...) selects all nodes within a bounding box;  
>< recurses up fully, i.e. selects all ways containing these nodes and all relations containing these nodes and ways;  
>rel(br) selects all parent relations of relations obtained so far (otherwise master relations would not be obtained)
>



Summary
-------  

The services mentioned in this chapter are all that the average user needs to get the OSM data they want and be able to work with it in GIS software. However, you may want to learn more powerful ways of working with the data yourself. The remaining chapters in this section are quite technical, but show more advanced methods of manipulating and accessing OSM data.  


[hot exports]: /images/osm-data/hot-exports.png
[overpass turbo]: /images/osm-data/overpass_turbo.png