TUGAS INDIVIDU WEEK04 
MATA KULIAH PEMBELAJARAN MESIN 2

oleh : Nasywa Kynda Sanina TI/5
NIM : 442023619074

berikut adalah model cnn yang berfungsi untuk memprediksi gender (pria/wanita) dari citra 2D yang diberikan. model ini menggunakan dataset yang terdiri dari 100 wajah pria dan 100 wajah wanita masing-masing untuk data testing dan training model. 

genderDataset  : https://www.kaggle.com/datasets/nasywakynda/gender-datasets
output best model  : https://drive.google.com/file/d/1oOJ41Zo9AUou6yEOzAW3dvDrF5mkaJFN/view?usp=sharing
output gender checkpoint  : https://drive.google.com/file/d/1QmMw9JxqX-zIpUBlxDeBa57G5oAZki4E/view?usp=sharing

berikut adalah struktur dari model CNN yang digunakan:
WEEK4 INDIVIDU
├── data/ 
|       ├── genderDataset
|           ├── test/
|           │   ├── pria/ 
|           │   └── wanita/
|           ├── train/
|           │   ├── pria/
|           │   └── wanita/
|       ├── image2.jpeg ----- gambar untuk prediksi
|       ├── image.jpeg ----- gambar untuk prediksi
├── output/
|   ├── best_model.pth ----- menyimpan model terbaik pada posisi optimal
|   ├── gender_checkpoint.pth ----- menyimpan model secara berkala
├── README.md
├── nasywa kynda_week4.ipynb ----- file tugas week04


dengan struktur model terdiri dari:
- dataset class 
- data loader
- model menggunakan resnet18
- traing loop
- early stopping dengan 3x patience
- visualisasi loss test & train per epoch
- save model terbaik dan checkpoint model secara berkala
- prediksi gambar
- confusion matrix
