[form-styles.css](https://github.com/user-attachments/files/23858343/form-styles.css) 
![formgif](https://github.com/user-attachments/assets/0667dde6-02ef-49a4-93af-9b099cc047c5)

 

 [form.html](https://github.com/user-attachments/files/23858335/form.html)
<!DOCTYPE html>
<html lang="tr">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Kayıt Formu Ödevi</title>
    <link rel="stylesheet" href="form-styles.css">
</head>
<body>

    <h1 id="title">Yazılım Geliştirme Kayıt Formu</h1>
    
    <p id="description">Kısa bir anket ile beklentilerinizi ve deneyiminizi paylaşın.</p>

    <form id="survey-form">

        <div class="form-group">
            <label id="name-label" for="name">Adınız Soyadınız:</label>
            <input 
                type="text" 
                id="name" 
                placeholder="Adınızı buraya girin" 
                required 
            />
        </div>

        <div class="form-group">
            <label id="email-label" for="email">E-posta Adresiniz:</label>
            <input 
                type="email" 
                id="email" 
                placeholder="ornek@mail.com" 
                required 
            />
            </div>

        <div class="form-group">
            <label id="number-label" for="number">Yaşınız (18-99):</label>
            <input 
                type="number" 
                id="number" 
                placeholder="Örn: 25" 
                min="18" 
                max="99" 
                required 
            />
            </div>
        
        <div class="form-group">
            <label for="dropdown">Mevcut Rolünüz Nedir?</label>
            <select id="dropdown" required>
                <option disabled selected value>Lütfen bir seçim yapın</option>
                <option value="student">Öğrenci</option>
                <option value="developer">Yazılımcı</option>
                <option value="designer">Tasarımcı</option>
                <option option="manager">Yönetici</option>
                <option value="other">Diğer</option>
            </select>
        </div>

        <div class="form-group">
            <label>Geliştiriciliğe Yönelik İlginiz Nasıl?</label>
            <label class="radio-label">
                <input type="radio" name="interest-level" value="high" checked /> Yüksek
            </label>
            <label class="radio-label">
                <input type="radio" name="interest-level" value="medium" /> Orta
            </label>
            <label class="radio-label">
                <input type="radio" name="interest-level" value="low" /> Düşük
            </label>
        </div>
        
        <div class="form-group">
            <label>Öğrenmek İstediğiniz Konular (Birden çok seçin):</label>
            <label class="checkbox-label">
                <input type="checkbox" name="topics" value="frontend" /> Frontend Geliştirme
            </label>
            <label class="checkbox-label">
                <input type="checkbox" name="topics" value="backend" /> Backend Geliştirme
            </label>
            <label class="checkbox-label">
                <input type="checkbox" name="topics" value="database" /> Veritabanı Yönetimi
            </label>
            <label class="checkbox-label">
                <input type="checkbox" name="topics" value="devops" /> DevOps Araçları
            </label>
        </div>

        <div class="form-group">
            <label for="comments">Ek Yorumlar ve Geri Bildirimler:</label>
            <textarea 
                id="comments" 
                name="comments" 
                rows="5" 
                placeholder="Buraya yorumlarınızı ve önerilerinizi yazabilirsiniz..."
            ></textarea>
        </div>

        <button type="submit" id="submit">
            Gönder
        </button>

    </form>

</body>
</html>







 form-styles.css

 
body {
    font-family: Arial, sans-serif;
    background-color: #f4f4f9;  
    color: #333;
    line-height: 1.6;
    margin: 0;
    padding: 20px;
    text-align: center;
}

 
#title, #description {
    text-align: center;
    margin-bottom: 5px;
}

#title {
    color: #007bff;  
}

 
#survey-form {
    max-width: 600px;
    margin: 30px auto;
    padding: 25px;
    background-color: #fff;  
    border-radius: 8px;
    box-shadow: 0 4px 12px rgba(0, 0, 0, 0.1);
    text-align: left;  
}

 
.form-group {
    margin-bottom: 20px;
    padding: 10px;
    border-bottom: 1px solid #eee;
}

 
label {
    display: block;
    margin-bottom: 8px;
    font-weight: bold;
    color: #555;
}

 
input[type="text"],
input[type="email"],
input[type="number"],
select,
textarea {
    width: 100%;
    padding: 10px;
    border: 1px solid #ccc;
    border-radius: 4px;
    box-sizing: border-box;  
    font-size: 16px;
}

select {
    height: 40px;  
}

 
.radio-label, .checkbox-label {
    display: block;  
    font-weight: normal;
    margin-bottom: 5px;
}

.radio-label input, .checkbox-label input {
    margin-right: 10px;
}


#submit {
    width: 100%;
    padding: 12px;
    background-color: #28a745; /* Yeşil Buton */
    color: white;
    border: none;
    border-radius: 4px;
    cursor: pointer;
    font-size: 18px;
    margin-top: 15px;
    transition: background-color 0.3s ease;
}

#submit:hover {
    background-color: #218838;  
}ng form-styles.css…]()




