# Standart Güncelleme Denetleyici

Excel'deki standart listesini yükleyin, her standart için arama linklerine tıklayın, güncel mi değil mi işaretleyin, Excel'e aktarın.

## Render.com'a Yükleme (Ücretsiz)

### 1. GitHub'a yükle
1. github.com → **New repository** → isim: `standart-kontrol` → **Create repository**
2. Bilgisayarınızda bu klasörü açın
3. Sağ tık → **Git Bash Here** (veya terminal)
4. Şu komutları sırayla yapıştırın:
```
git init
git add .
git commit -m "ilk yükleme"
git branch -M main
git remote add origin https://github.com/KULLANICI_ADINIZ/standart-kontrol.git
git push -u origin main
```

### 2. Render.com'da yayınla
1. render.com → **Sign up** (GitHub ile giriş yapın)
2. **New** → **Web Service**
3. GitHub reponuzu seçin (`standart-kontrol`)
4. Ayarlar otomatik gelir (`render.yaml` sayesinde)
5. **Create Web Service** butonuna basın
6. 2-3 dakika bekleyin → size bir link verilir

### 3. Kullanım
- Verilen linke tarayıcıdan girin
- Excel dosyanızı yükleyin
- Her standart için arama linklerine tıklayın
- ✅ Güncel veya ⚠️ Güncelleme Var olarak işaretleyin
- Excel'e Aktar ile sonuçları indirin

## Yerel Çalıştırma (Test için)
```
pip install -r requirements.txt
python app.py
```
Tarayıcıda: http://localhost:5000
