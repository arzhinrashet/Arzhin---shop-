# Arzhin---shop-
<!DOCTYPE html>
<html lang="fa" dir="rtl">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Arzhin Shop</title>
    <style>
        body {
            font-family: 'Tahoma', sans-serif;
            margin: 0;
            padding: 0;
            background-color: #f4f4f4;
            color: #333;
        }
        header {
            background-color: #007bff;
            color: white;
            padding: 20px;
            text-align: center;
        }
        nav {
            background-color: #333;
            padding: 10px;
        }
        nav ul {
            list-style: none;
            margin: 0;
            padding: 0;
            text-align: center;
        }
        nav ul li {
            display: inline;
            margin: 0 15px;
        }
        nav ul li a {
            color: white;
            text-decoration: none;
            font-weight: bold;
        }
        main {
            max-width: 1200px;
            margin: 20px auto;
            padding: 20px;
            background-color: white;
            box-shadow: 0 0 10px rgba(0,0,0,0.1);
        }
        section {
            margin-bottom: 40px;
        }
        h2 {
            color: #007bff;
        }
        .products {
            display: flex;
            flex-wrap: wrap;
            justify-content: space-around;
        }
        .product {
            border: 1px solid #ddd;
            border-radius: 5px;
            padding: 10px;
            margin: 10px;
            width: 300px;
            text-align: center;
        }
        .product img {
            max-width: 100%;
            height: auto;
        }
        .product h3 {
            margin: 10px 0;
        }
        .product .price {
            font-size: 1.2em;
            color: #28a745;
            margin: 10px 0;
        }
        .product button {
            background-color: #007bff;
            color: white;
            border: none;
            padding: 10px 20px;
            cursor: pointer;
            font-size: 1em;
        }
        .product button:hover {
            background-color: #0056b3;
        }
        #admin-section {
            display: none;
        }
        #login-section {
            max-width: 400px;
            margin: 20px auto;
        }
        form label {
            display: block;
            margin: 10px 0 5px;
        }
        form input, form textarea {
            width: 100%;
            padding: 8px;
            margin-bottom: 10px;
        }
        form button {
            background-color: #007bff;
            color: white;
            border: none;
            padding: 10px;
            cursor: pointer;
        }
        footer {
            background-color: #333;
            color: white;
            text-align: center;
            padding: 10px;
            position: fixed;
            width: 100%;
            bottom: 0;
        }
    </style>
</head>
<body>

    <header>
        <h1>خوش آمدید به Arzhin Shop</h1>
        <p>فروشگاه آنلاین برای خرید محصولات متنوع</p>
    </header>

    <nav>
        <ul>
            <li><a href="#home">خانه</a></li>
            <li><a href="#about">درباره ما</a></li>
            <li><a href="#products">محصولات</a></li>
            <li><a href="#contact">تماس</a></li>
            <li><a href="#admin">ادمین</a></li>
        </ul>
    </nav>

    <main>
        <section id="home">
            <h2>خانه</h2>
            <p>این بخش خانه فروشگاه است. اینجا می‌توانید محصولات ویژه را ببینید.</p>
            <img src="https://via.placeholder.com/800x400?text=بنر+فروشگاه" alt="بنر فروشگاه" style="width:100%; height:auto;">
        </section>

        <section id="about">
            <h2>درباره ما</h2>
            <p>Arzhin Shop یک فروشگاه آنلاین است که محصولات با کیفیت بالا ارائه می‌دهد. این متن نمونه است.</p>
        </section>

        <section id="products">
            <h2>محصولات</h2>
            <div class="products" id="product-list">
                <!-- محصولات پیش‌فرض -->
                <div class="product">
                    <img src="https://via.placeholder.com/300x300?text=محصول+1" alt="محصول 1">
                    <h3>محصول 1</h3>
                    <p>توضیحات کوتاه محصول 1. کیفیت عالی و قیمت مناسب.</p>
                    <div class="price">۱۰۰,۰۰۰ تومان</div>
                    <button>افزودن به سبد خرید</button>
                </div>
                <div class="product">
                    <img src="https://via.placeholder.com/300x300?text=محصول+2" alt="محصول 2">
                    <h3>محصول 2</h3>
                    <p>توضیحات کوتاه محصول 2. جدیدترین مدل.</p>
                    <div class="price">۱۵۰,۰۰۰ تومان</div>
                    <button>افزودن به سبد خرید</button>
                </div>
                <div class="product">
                    <img src="https://via.placeholder.com/300x300?text=محصول+3" alt="محصول 3">
                    <h3>محصول 3</h3>
                    <p>توضیحات کوتاه محصول 3. تخفیف ویژه.</p>
                    <div class="price">۸۰,۰۰۰ تومان</div>
                    <button>افزودن به سبد خرید</button>
                </div>
                <!-- محصولات اضافه شده توسط ادمین اینجا نمایش داده می‌شوند -->
            </div>
        </section>

        <section id="contact">
            <h2>تماس با ما</h2>
            <form action="#" method="post">
                <label for="name">نام:</label>
                <input type="text" id="name" name="name" required><br><br>
                
                <label for="email">ایمیل:</label>
                <input type="email" id="email" name="email" required><br><br>
                
                <label for="message">پیام:</label><br>
                <textarea id="message" name="message" rows="4" required></textarea><br><br>
                
                <input type="submit" value="ارسال">
            </form>
        </section>

        <section id="admin">
            <h2>پنل ادمین</h2>
            <div id="login-section">
                <form id="login-form">
                    <label for="username">نام کاربری:</label>
                    <input type="text" id="username" required>
                    
                    <label for="password">کد ورود:</label>
                    <input type="password" id="password" required>
                    
                    <button type="submit">ورود</button>
                </form>
            </div>
            <div id="admin-section">
                <h3>آپلود محصول جدید</h3>
                <form id="upload-form">
                    <label for="product-name">نام محصول:</label>
                    <input type="text" id="product-name" required>
                    
                    <label for="product-price">قیمت (تومان):</label>
                    <input type="number" id="product-price" required>
                    
                    <label for="product-about">توضیحات:</label>
                    <textarea id="product-about" rows="4" required></textarea>
                    
                    <label for="product-image">عکس محصول:</label>
                    <input type="file" id="product-image" accept="image/*" required>
                    
                    <button type="submit">آپلود محصول</button>
                </form>
            </div>
        </section>
    </main>

    <footer>
        <p>&copy; 2025 Arzhin Shop. تمام حقوق محفوظ است.</p>
    </footer>

    <script>
        // نام کاربری و پسورد ادمین
        const adminUsername = "Arzhin rashet";
        const adminPassword = "arr7arr7";

        // بررسی لاگین
        const loginForm = document.getElementById('login-form');
        const adminSection = document.getElementById('admin-section');
        const loginSection = document.getElementById('login-section');

        loginForm.addEventListener('submit', function(e) {
            e.preventDefault();
            const username = document.getElementById('username').value;
            const password = document.getElementById('password').value;

            if (username === adminUsername && password === adminPassword) {
                loginSection.style.display = 'none';
                adminSection.style.display = 'block';
                alert('ورود موفق!');
            } else {
                alert('نام کاربری یا کد ورود اشتباه است.');
            }
        });

        // بارگذاری محصولات از LocalStorage
        function loadProducts() {
            const productList = document.getElementById('product-list');
            const products = JSON.parse(localStorage.getItem('products')) || [];

            // پاک کردن محصولات اضافه شده قبلی (به جز پیش‌فرض)
            const addedProducts = productList.querySelectorAll('.added-product');
            addedProducts.forEach(prod => prod.remove());

            products.forEach(product => {
                const productDiv = document.createElement('div');
                productDiv.classList.add('product', 'added-product');
                productDiv.innerHTML = `
                    <img src="\( {product.image}" alt=" \){product.name}">
                    <h3>${product.name}</h3>
                    <p>${product.about}</p>
                    <div class="price">${product.price} تومان</div>
                    <button>افزودن به سبد خرید</button>
                `;
                productList.appendChild(productDiv);
            });
        }

        // آپلود محصول
        const uploadForm = document.getElementById('upload-form');
        uploadForm.addEventListener('submit', function(e) {
            e.preventDefault();

            const name = document.getElementById('product-name').value;
            const price = document.getElementById('product-price').value;
            const about = document.getElementById('product-about').value;
            const imageFile = document.getElementById('product-image').files[0];

            if (imageFile) {
                const reader = new FileReader();
                reader.onload = function(event) {
                    const imageUrl = event.target.result; // Base64 برای نمایش محلی
                    const products = JSON.parse(localStorage.getItem('products')) || [];
                    products.push({ name, price, about, image: imageUrl });
                    localStorage.setItem('products', JSON.stringify(products));
                    loadProducts();
                    alert('محصول با موفقیت آپلود شد!');
                    uploadForm.reset();
                };
                reader.readAsDataURL(imageFile);
            }
        });

        // بارگذاری اولیه محصولات
        window.onload = loadProducts;
    </script>

</body>
</html>
