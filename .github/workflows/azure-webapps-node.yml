<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Game Over - متجر أغراض القيمنق</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        :root {
            --primary-color: #6a11cb;
            --secondary-color: #2575fc;
            --accent-color: #ff3860;
            --light-color: #ffffff;
            --dark-color: #121212;
            --gray-color: #f5f5f5;
            --text-color: #333333;
            --success-color: #4CAF50;
        }
        
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        }
        
        body {
            background-color: var(--light-color);
            color: var(--text-color);
            min-height: 100vh;
            overflow-x: hidden;
        }
        
        .container {
            width: 90%;
            max-width: 1200px;
            margin: 0 auto;
            padding: 20px;
        }
        
        /* الترويسة */
        header {
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 20px 0;
            border-bottom: 2px solid rgba(0, 0, 0, 0.1);
            margin-bottom: 30px;
            animation: fadeIn 1s ease;
        }
        
        @keyframes fadeIn {
            from { opacity: 0; }
            to { opacity: 1; }
        }
        
        .logo {
            display: flex;
            align-items: center;
        }
        
        .logo h1 {
            font-size: 2.5rem;
            background: linear-gradient(to right, var(--primary-color), var(--secondary-color));
            -webkit-background-clip: text;
            background-clip: text;
            color: transparent;
            text-shadow: 0 0 10px rgba(106, 17, 203, 0.2);
            animation: glow 2s infinite alternate;
        }
        
        @keyframes glow {
            from { text-shadow: 0 0 10px rgba(106, 17, 203, 0.2); }
            to { text-shadow: 0 0 20px rgba(106, 17, 203, 0.4), 0 0 30px rgba(106, 17, 203, 0.2); }
        }
        
        nav ul {
            display: flex;
            list-style: none;
        }
        
        nav ul li {
            margin-left: 20px;
        }
        
        nav ul li a {
            color: var(--text-color);
            text-decoration: none;
            font-weight: bold;
            transition: color 0.3s;
            position: relative;
            padding: 5px 0;
        }
        
        nav ul li a:hover {
            color: var(--primary-color);
        }
        
        nav ul li a::after {
            content: '';
            position: absolute;
            width: 0;
            height: 2px;
            bottom: 0;
            left: 0;
            background-color: var(--primary-color);
            transition: width 0.3s;
        }
        
        nav ul li a:hover::after {
            width: 100%;
        }
        
        .header-buttons {
            display: flex;
            align-items: center;
            gap: 15px;
        }
        
        .cart-icon {
            position: relative;
            font-size: 1.5rem;
            cursor: pointer;
            color: var(--text-color);
        }
        
        .cart-count {
            position: absolute;
            top: -10px;
            right: -10px;
            background: var(--accent-color);
            color: white;
            border-radius: 50%;
            width: 20px;
            height: 20px;
            display: flex;
            justify-content: center;
            align-items: center;
            font-size: 0.8rem;
            font-weight: bold;
        }
        
        .login-btn {
            padding: 8px 15px;
            background: linear-gradient(to right, var(--primary-color), var(--secondary-color));
            color: white;
            border: none;
            border-radius: 5px;
            cursor: pointer;
            transition: transform 0.3s;
        }
        
        .login-btn:hover {
            transform: translateY(-3px);
        }
        
        /* قسم الخصم */
        .discount-section {
            background: linear-gradient(to right, var(--primary-color), var(--secondary-color));
            padding: 15px;
            border-radius: 10px;
            margin-bottom: 30px;
            text-align: center;
            color: white;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.1);
            animation: pulse 2s infinite;
        }
        
        @keyframes pulse {
            0% { box-shadow: 0 0 0 0 rgba(106, 17, 203, 0.4); }
            70% { box-shadow: 0 0 0 10px rgba(106, 17, 203, 0); }
            100% { box-shadow: 0 0 0 0 rgba(106, 17, 203, 0); }
        }
        
        .discount-form {
            display: flex;
            justify-content: center;
            align-items: center;
            gap: 10px;
            margin-top: 10px;
        }
        
        .discount-form input {
            padding: 10px 15px;
            border: none;
            border-radius: 5px;
            width: 250px;
            background: rgba(255, 255, 255, 0.9);
        }
        
        .discount-btn {
            padding: 10px 20px;
            background: var(--accent-color);
            color: white;
            border: none;
            border-radius: 5px;
            cursor: pointer;
            transition: background 0.3s;
        }
        
        .discount-btn:hover {
            background: #ff002b;
        }
        
        /* قسم تسجيل الدخول */
        .login-section {
            background-color: var(--gray-color);
            padding: 20px;
            border-radius: 10px;
            margin-bottom: 30px;
            text-align: center;
        }
        
        .social-login {
            display: flex;
            justify-content: center;
            gap: 15px;
            margin-top: 15px;
        }
        
        .social-btn {
            display: flex;
            align-items: center;
            justify-content: center;
            gap: 8px;
            padding: 10px 20px;
            border: none;
            border-radius: 5px;
            cursor: pointer;
            transition: transform 0.3s;
            color: white;
            font-weight: bold;
        }
        
        .social-btn:hover {
            transform: translateY(-3px);
        }
        
        .google-btn {
            background: #DB4437;
        }
        
        .facebook-btn {
            background: #4267B2;
        }
        
        .twitter-btn {
            background: #1DA1F2;
        }
        
        /* المنتجات */
        .products-grid {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(250px, 1fr));
            gap: 30px;
            margin-bottom: 50px;
        }
        
        .product-card {
            background: white;
            border-radius: 15px;
            overflow: hidden;
            transition: transform 0.3s, box-shadow 0.3s;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.05);
            animation: fadeInUp 0.5s ease;
        }
        
        .product-card:hover {
            transform: translateY(-10px);
            box-shadow: 0 15px 30px rgba(0, 0, 0, 0.1);
        }
        
        @keyframes fadeInUp {
            from {
                opacity: 0;
                transform: translateY(20px);
            }
            to {
                opacity: 1;
                transform: translateY(0);
            }
        }
        
        .product-image {
            width: 100%;
            height: 200px;
            overflow: hidden;
        }
        
        .product-image img {
            width: 100%;
            height: 100%;
            object-fit: cover;
            transition: transform 0.5s;
        }
        
        .product-card:hover .product-image img {
            transform: scale(1.1);
        }
        
        .product-info {
            padding: 20px;
        }
        
        .product-info h3 {
            margin-bottom: 10px;
            font-size: 1.2rem;
            color: var(--text-color);
        }
        
        .product-info p {
            color: #666;
            margin-bottom: 15px;
            font-size: 0.9rem;
        }
        
        .product-price {
            display: flex;
            justify-content: space-between;
            align-items: center;
            margin-top: 15px;
        }
        
        .price {
            font-weight: bold;
            font-size: 1.3rem;
            color: var(--primary-color);
        }
        
        .original-price {
            text-decoration: line-through;
            color: #999;
            font-size: 0.9rem;
            margin-left: 10px;
        }
        
        .add-to-cart {
            background: var(--secondary-color);
            color: white;
            border: none;
            padding: 8px 15px;
            border-radius: 5px;
            cursor: pointer;
            transition: background 0.3s;
        }
        
        .add-to-cart:hover {
            background: #1a63db;
        }
        
        /* السلة */
        .cart-section {
            background: var(--gray-color);
            padding: 20px;
            border-radius: 15px;
            margin-top: 30px;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.05);
        }
        
        .cart-section h2 {
            margin-bottom: 20px;
            text-align: center;
            color: var(--primary-color);
        }
        
        .cart-items {
            margin-bottom: 20px;
        }
        
        .cart-item {
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 10px 0;
            border-bottom: 1px solid rgba(0, 0, 0, 0.1);
        }
        
        .cart-total {
            text-align: right;
            font-size: 1.2rem;
            margin-bottom: 20px;
        }
        
        .checkout-btn {
            display: block;
            width: 100%;
            padding: 15px;
            background: var(--accent-color);
            color: white;
            border: none;
            border-radius: 5px;
            font-size: 1.1rem;
            cursor: pointer;
            transition: background 0.3s;
        }
        
        .checkout-btn:hover {
            background: #ff002b;
        }
        
        /* التذييل */
        footer {
            text-align: center;
            padding: 30px 0;
            margin-top: 50px;
            border-top: 2px solid rgba(0, 0, 0, 0.1);
        }
        
        .social-icons {
            display: flex;
            justify-content: center;
            gap: 20px;
            margin: 20px 0;
        }
        
        .social-icons a {
            color: var(--text-color);
            font-size: 1.5rem;
            transition: color 0.3s;
        }
        
        .social-icons a:hover {
            color: var(--primary-color);
        }
        
        /* تأثيرات Responsive */
        @media (max-width: 768px) {
            header {
                flex-direction: column;
                text-align: center;
            }
            
            nav ul {
                margin-top: 20px;
                justify-content: center;
            }
            
            .products-grid {
                grid-template-columns: repeat(auto-fill, minmax(200px, 1fr));
            }
            
            .discount-form {
                flex-direction: column;
            }
            
            .discount-form input {
                width: 100%;
                margin-bottom: 10px;
            }
            
            .social-login {
                flex-direction: column;
            }
        }
    </style>
</head>
<body>
    <div class="container">
        <header>
            <div class="logo">
                <h1>Game Over</h1>
            </div>
            <nav>
                <ul>
                    <li><a href="#">الرئيسية</a></li>
                    <li><a href="#">منتجاتنا</a></li>
                    <li><a href="#">عنا</a></li>
                    <li><a href="#">اتصل بنا</a></li>
                </ul>
            </nav>
            <div class="header-buttons">
                <div class="cart-icon">
                    <i class="fas fa-shopping-cart"></i>
                    <span class="cart-count">0</span>
                </div>
                <button class="login-btn">تسجيل الدخول</button>
            </div>
        </header>
        
        <section class="discount-section">
            <h2>استخدم كود الخصم "SIF" للحصول على خصم 10%!</h2>
            <div class="discount-form">
                <input type="text" placeholder="أدخل كود الخصم هنا" id="discount-code">
                <button class="discount-btn" onclick="applyDiscount()">تطبيق الخصم</button>
            </div>
        </section>
        
        <section class="login-section">
            <h3>سجل الدخول باستخدام</h3>
            <div class="social-login">
                <button class="social-btn google-btn">
                    <i class="fab fa-google"></i>
                    جوجل
                </button>
                <button class="social-btn facebook-btn">
                    <i class="fab fa-facebook-f"></i>
                    فيسبوك
                </button>
                <button class="social-btn twitter-btn">
                    <i class="fab fa-twitter"></i>
                    تويتر
                </button>
            </div>
        </section>
        
        <div class="products-grid">
            <!-- المنتج 1 -->
            <div class="product-card">
                <div class="product-image">
                    <img src="https://images.unsplash.com/photo-1600080972464-8e5f35f63d08?ixlib=rb-4.0.3&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=435&q=80" alt="لوحة المفاتيح الميكانيكية">
                </div>
                <div class="product-info">
                    <h3>لوحة المفاتيح الميكانيكية</h3>
                    <p>لوحة مفاتيح ميكانيكية بإضاءة RGB، مقاومة للماء، تصميم مريح للاعبين المحترفين.</p>
                    <div class="product-price">
                        <div>
                            <span class="price">350 ر.س</span>
                            <span class="original-price">389 ر.س</span>
                        </div>
                        <button class="add-to-cart">إضافة إلى السلة</button>
                    </div>
                </div>
            </div>
            
            <!-- المنتج 2 -->
            <div class="product-card">
                <div class="product-image">
                    <img src="https://images.unsplash.com/photo-1619551734325-3c2ae2f72b6c?ixlib=rb-4.0.3&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=580&q=80" alt="ماوس الألعاب">
                </div>
                <div class="product-info">
                    <h3>ماوس الألعاب</h3>
                    <p>ماوس ألعاب بدقة 16000 نقطة في البوصة، 8 أزرار قابلة للبرمجة، إضاءة RGB متطورة.</p>
                    <div class="product-price">
                        <div>
                            <span class="price">220 ر.س</span>
                            <span class="original-price">244 ر.س</span>
                        </div>
                        <button class="add-to-cart">إضافة إلى السلة</button>
                    </div>
                </div>
            </div>
            
            <!-- المنتج 3 -->
            <div class="product-card">
                <div class="product-image">
                    <img src="https://images.unsplash.com/photo-1593640408182-31c70c8268f5?ixlib=rb-4.0.3&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=842&q=80" alt="سماعة الألعاب">
                </div>
                <div class="product-info">
                    <h3>سماعة الألعاب</h3>
                    <p>سماعة ألعاب محيطية 7.1، ميكروفون مدمج، إضاءة RGB، تصميم مريح للاستخدام الطويل.</p>
                    <div class="product-price">
                        <div>
                            <span class="price">280 ر.س</span>
                            <span class="original-price">311 ر.س</span>
                        </div>
                        <button class="add-to-cart">إضافة إلى السلة</button>
                    </div>
                </div>
            </div>
            
            <!-- المنتج 4 -->
            <div class="product-card">
                <div class="product-image">
                    <img src="https://images.unsplash.com/photo-1596461404969-9ae70f2830c1?ixlib=rb-4.0.3&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=870&q=80" alt="كرسي الألعاب">
                </div>
                <div class="product-info">
                    <h3>كرسي الألعاب</h3>
                    <p>كرسي ألعاب مريح، دعم كامل للظهر، إمكانية تعديل الارتفاع، مواد عالية الجودة.</p>
                    <div class="product-price">
                        <div>
                            <span class="price">900 ر.س</span>
                            <span class="original-price">1000 ر.س</span>
                        </div>
                        <button class="add-to-cart">إضافة إلى السلة</button>
                    </div>
                </div>
            </div>
            
            <!-- المنتج 5 -->
            <div class="product-card">
                <div class="product-image">
                    <img src="https://images.unsplash.com/photo-1593642632823-8f785ba67e45?ixlib=rb-4.0.3&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=812&q=80" alt="شاشة الألعاب">
                </div>
                <div class="product-info">
                    <h3>شاشة الألعاب</h3>
                    <p>شاشة ألعاب 27 بوصة، دقة 2K، معدل تحديث 144Hz، تقنية FreeSync.</p>
                    <div class="product-price">
                        <div>
                            <span class="price">1200 ر.س</span>
                            <span class="original-price">1333 ر.س</span>
                        </div>
                        <button class="add-to-cart">إضافة إلى السلة</button>
                    </div>
                </div>
            </div>
            
            <!-- المنتج 6 -->
            <div class="product-card">
                <div class="product-image">
                    <img src="https://images.unsplash.com/photo-1592899677977-9c10ca588bbd?ixlib=rb-4.0.3&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=772&q=80" alt="لوحة تحكم">
                </div>
                <div class="product-info">
                    <h3>لوحة تحكم</h3>
                    <p>لوحة تحكم لاسلكية، تصميم مريح، بطارية طويلة الأمد، متوافقة مع الأجهزة المختلفة.</p>
                    <div class="product-price">
                        <div>
                            <span class="price">180 ر.س</span>
                            <span class="original-price">200 ر.س</span>
                        </div>
                        <button class="add-to-cart">إضافة إلى السلة</button>
                    </div>
                </div>
            </div>
            
            <!-- المنتج 7 -->
            <div class="product-card">
                <div class="product-image">
                    <img src="https://images.unsplash.com/photo-1593642633279-1796119d5482?ixlib=rb-4.0.3&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=868&q=80" alt="سطح المكتب">
                </div>
                <div class="product-info">
                    <h3>سطح المكتب</h3>
                    <p>سطح مكتب مخصص للألعاب، تصميم عصري، مساحة كبيرة، مواد متينة.</p>
                    <div class="product-price">
                        <div>
                            <span class="price">450 ر.س</span>
                            <span class="original-price">500 ر.س</span>
                        </div>
                        <button class="add-to-cart">إضافة إلى السلة</button>
                    </div>
                </div>
            </div>
            
            <!-- المنتج 8 -->
            <div class="product-card">
                <div class="product-image">
                    <img src="https://images.unsplash.com/photo-1593541925857-7d0ad303adeb?ixlib=rb-4.0.3&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=870&q=80" alt="إضاءة RGB">
                </div>
                <div class="product-info">
                    <h3>إضاءة RGB</h3>
                    <p>شريط إضاءة RGB، تحكم عن بعد، 16 مليون لون، مقاوم للالتصاق.</p>
                    <div class="product-price">
                        <div>
                            <span class="price">90 ر.س</span>
                            <span class="original-price">100 ر.س</span>
                        </div>
                        <button class="add-to-cart">إضافة إلى السلة</button>
                    </div>
                </div>
            </div>
            
            <!-- المنتج 9 -->
            <div class="product-card">
                <div class="product-image">
                    <img src="https://images.unsplash.com/photo-1593642532744-d377ab507dc8?ixlib=rb-4.0.3&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=869&q=80" alt="كرت الشاشة">
                </div>
                <div class="product-info">
                    <h3>كرت الشاشة</h3>
                    <p>كرت شاشة قوي، 8GB VRAM، تبريد مزدوج، أداء عالي في الألعاب.</p>
                    <div class="product-price">
                        <div>
                            <span class="price">1600 ر.س</span>
                            <span class="original-price">1778 ر.س</span>
                        </div>
                        <button class="add-to-cart">إضافة إلى السلة</button>
                    </div>
                </div>
            </div>
            
            <!-- المنتج 10 -->
            <div class="product-card">
                <div class="product-image">
                    <img src="https://images.unsplash.com/photo-1593642634443-44adaa066e75?ixlib=rb-4.0.3&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=725&q=80" alt="لوح التزلج">
                </div>
                <div class="product-info">
                    <h3>لوح التزلج للألعاب</h3>
                    <p>لوح تزلج مخصص للاعبين، تصميم فريد، مواد عالية الجودة، تحكم دقيق.</p>
                    <div class="product-price">
                        <div>
                            <span class="price">270 ر.س</span>
                            <span class="original-price">300 ر.س</span>
                        </div>
                        <button class="add-to-cart">إضافة إلى السلة</button>
                    </div>
                </div>
            </div>
            
            <!-- المنتج 11 -->
            <div class="product-card">
                <div class="product-image">
                    <img src="https://images.unsplash.com/photo-1593642532842-98d0fd5ebc1a?ixlib=rb-4.0.3&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=870&q=80" alt="حاسوب الألعاب">
                </div>
                <div class="product-info">
                    <h3>حاسوب الألعاب</h3>
                    <p>حاسوب ألعاب بقوة معالجة عالية، كرت شاشة مخصص، إضاءة RGB، تبريد متقدم.</p>
                    <div class="product-price">
                        <div>
                            <span class="price">3600 ر.س</span>
                            <span class="original-price">4000 ر.س</span>
                        </div>
                        <button class="add-to-cart">إضافة إلى السلة</button>
                    </div>
                </div>
            </div>
        </div>
        
        <section class="cart-section">
            <h2>سلة التسوق</h2>
            <div class="cart-items">
                <p>سلتك فارغة حالياً</p>
            </div>
            <div class="cart-total">
                المجموع: <span>0 ر.س</span>
            </div>
            <button class="checkout-btn">إتمام الشراء</button>
        </section>
        
        <footer>
            <div class="social-icons">
                <a href="#"><i class="fab fa-twitter"></i></a>
                <a href="#"><i class="fab fa-instagram"></i></a>
                <a href="#"><i class="fab fa-youtube"></i></a>
                <a href="#"><i class="fab fa-discord"></i></a>
            </div>
            <p>© 2023 Game Over. جميع الحقوق محفوظة</p>
        </footer>
    </div>

    <script>
        // كود JavaScript للخصم وإضافة المنتجات للسلة
        document.addEventListener('DOMContentLoaded', function() {
            const cartButtons = document.querySelectorAll('.add-to-cart');
            const cartCount = document.querySelector('.cart-count');
            const cartItems = document.querySelector('.cart-items');
            const cartTotal = document.querySelector('.cart-total span');
            let count = 0;
            let total = 0;
            let discountApplied = false;
            
            // إضافة منتج إلى السلة
            cartButtons.forEach(button => {
                button.addEventListener('click', function() {
                    count++;
                    cartCount.textContent = count;
                    
                    const productCard = this.closest('.product-card');
                    const productName = productCard.querySelector('h3').textContent;
                    const productPrice = parseFloat(productCard.querySelector('.price').textContent);
                    
                    total += productPrice;
                    updateCart();
                    
                    // تأثير عند الإضافة
                    this.textContent = 'تمت الإضافة!';
                    this.style.background = 'var(--success-color)';
                    
                    setTimeout(() => {
                        this.textContent = 'إضافة إلى السلة';
                        this.style.background = '';
                    }, 1500);
                    
                    // تأثير اهتزاز للسلة
                    cartCount.parentElement.classList.add('shake');
                    setTimeout(() => {
                        cartCount.parentElement.classList.remove('shake');
                    }, 500);
                });
            });
            
            // تحديث السلة
            function updateCart() {
                cartItems.innerHTML = `
                    <div class="cart-item">
                        <span>${count} منتج</span>
                        <span>${total.toFixed(2)} ر.س</span>
                    </div>
                `;
                
                cartTotal.textContent = `${total.toFixed(2)} ر.س`;
            }
            
            // تطبيق الخصم
            window.applyDiscount = function() {
                const discountCode = document.getElementById('discount-code').value;
                
                if (discountCode.toUpperCase() === 'SIF' && !discountApplied) {
                    total = total * 0.9; // خصم 10%
                    discountApplied = true;
                    updateCart();
                    
                    // عرض رسالة نجاح
                    alert('تم تطبيق الخصم بنجاح! تم خصم 10% من إجمالي الطلب.');
                } else if (discountApplied) {
                    alert('تم تطبيق الخصم مسبقاً!');
                } else {
                    alert('كود الخصم غير صحيح!');
                }
            };
        });
    </script>
</body>
</html>
