<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Ranjit Enterprises</title>

  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;500;600;700&display=swap" rel="stylesheet">

  <style>
    *{
      margin:0;
      padding:0;
      box-sizing:border-box;
      scroll-behavior:smooth;
    }

    body{
      font-family:'Poppins',sans-serif;
      background:#f5f5f5;
      color:#222;
    }

    a{
      text-decoration:none;
    }

    /* HERO */
    .hero{
      height:100vh;
      background:url('https://i.ibb.co/fdMJB8jt/pexels-kriss-32549954-1.jpg') center/cover no-repeat;
      position:relative;
      display:flex;
      align-items:center;
      justify-content:center;
      text-align:center;
      padding:20px;
    }

    .overlay{
      position:absolute;
      inset:0;
      background:rgba(0,0,0,0.55);
    }

    .hero-content{
      position:relative;
      z-index:2;
      color:white;
      max-width:700px;
    }

    .hero h1{
      font-size:3rem;
      margin-bottom:10px;
      font-weight:700;
    }

    .hero p{
      font-size:1.2rem;
      margin-bottom:30px;
      opacity:0.95;
    }

    .shop-btn{
      display:inline-block;
      padding:14px 30px;
      background:#ff9800;
      color:white;
      border-radius:50px;
      font-weight:600;
      transition:0.3s;
    }

    .shop-btn:hover{
      background:#ff7700;
      transform:translateY(-2px);
    }

    /* SECTION */
    section{
      padding:60px 20px;
    }

    .section-title{
      text-align:center;
      font-size:2rem;
      margin-bottom:35px;
      font-weight:700;
    }

    /* PRODUCTS */
    .products-wrapper{
      overflow-x:auto;
      display:flex;
      gap:20px;
      scroll-snap-type:x mandatory;
      padding-bottom:10px;
    }

    .products-wrapper::-webkit-scrollbar{
      height:8px;
    }

    .products-wrapper::-webkit-scrollbar-thumb{
      background:#ccc;
      border-radius:10px;
    }

    .product-card{
      min-width:280px;
      background:white;
      border-radius:20px;
      overflow:hidden;
      box-shadow:0 6px 18px rgba(0,0,0,0.08);
      scroll-snap-align:start;
      transition:0.3s;
    }

    .product-card:hover{
      transform:translateY(-5px);
    }

    .product-card img{
      width:100%;
      height:260px;
      object-fit:cover;
    }

    .product-info{
      padding:18px;
    }

    .product-info h3{
      font-size:1.1rem;
      margin-bottom:10px;
    }

    .price{
      font-size:1rem;
      color:#ff6600;
      font-weight:600;
      margin-bottom:15px;
    }

    .add-cart{
      width:100%;
      border:none;
      padding:12px;
      border-radius:12px;
      background:#111;
      color:white;
      font-weight:600;
      cursor:pointer;
      transition:0.3s;
    }

    .add-cart:hover{
      background:#ff9800;
    }

    /* FLOATING CART */
    .cart-floating{
      position:fixed;
      right:20px;
      bottom:90px;
      width:60px;
      height:60px;
      border-radius:50%;
      background:#111;
      color:white;
      display:flex;
      align-items:center;
      justify-content:center;
      font-size:24px;
      cursor:pointer;
      z-index:999;
      box-shadow:0 5px 15px rgba(0,0,0,0.3);
    }

    .cart-count{
      position:absolute;
      top:-5px;
      right:-2px;
      background:red;
      color:white;
      width:24px;
      height:24px;
      border-radius:50%;
      display:flex;
      align-items:center;
      justify-content:center;
      font-size:12px;
      font-weight:700;
    }

    /* CART MODAL */
    .cart-modal{
      position:fixed;
      top:0;
      right:-100%;
      width:100%;
      max-width:420px;
      height:100%;
      background:white;
      z-index:1000;
      transition:0.4s;
      padding:25px;
      overflow-y:auto;
      box-shadow:-5px 0 20px rgba(0,0,0,0.15);
    }

    .cart-modal.active{
      right:0;
    }

    .close-btn{
      float:right;
      font-size:28px;
      cursor:pointer;
    }

    .cart-item{
      display:flex;
      justify-content:space-between;
      align-items:center;
      margin:15px 0;
      border-bottom:1px solid #eee;
      padding-bottom:10px;
    }

    .cart-item button{
      background:red;
      border:none;
      color:white;
      padding:5px 10px;
      border-radius:8px;
      cursor:pointer;
    }

    .cart-form{
      margin-top:25px;
    }

    .cart-form input,
    .cart-form textarea{
      width:100%;
      margin-bottom:15px;
      padding:12px;
      border-radius:12px;
      border:1px solid #ddd;
      font-family:inherit;
    }

    .send-order{
      width:100%;
      padding:14px;
      border:none;
      border-radius:14px;
      background:#25D366;
      color:white;
      font-size:1rem;
      font-weight:600;
      cursor:pointer;
    }

    /* WHATSAPP */
    .whatsapp-btn{
      position:fixed;
      right:20px;
      bottom:20px;
      background:#25D366;
      color:white;
      width:60px;
      height:60px;
      border-radius:50%;
      display:flex;
      align-items:center;
      justify-content:center;
      font-size:30px;
      z-index:999;
      box-shadow:0 5px 15px rgba(0,0,0,0.25);
    }

    footer{
      text-align:center;
      padding:25px;
      background:#111;
      color:white;
    }

    @media(max-width:768px){
      .hero h1{
        font-size:2.2rem;
      }

      .hero p{
        font-size:1rem;
      }
    }
  </style>
</head>
<body>

  <!-- HERO -->
  <section class="hero">
    <div class="overlay"></div>

    <div class="hero-content">
      <h1>Ranjit Enterprises</h1>
      <p>Best Product At Best Price</p>

      <a href="#products" class="shop-btn">
        Shop Now
      </a>
    </div>
  </section>

  <!-- PRODUCTS -->
  <section id="products">
    <h2 class="section-title">Our Products</h2>

    <div class="products-wrapper" id="productContainer"></div>
  </section>

  <!-- FLOATING CART -->
  <div class="cart-floating" onclick="openCart()">
    🛒
    <div class="cart-count" id="cartCount">0</div>
  </div>

  <!-- CART MODAL -->
  <div class="cart-modal" id="cartModal">

    <span class="close-btn" onclick="closeCart()">×</span>

    <h2>Your Cart</h2>

    <div id="cartItems"></div>

    <div class="cart-form">
      <input type="text" id="customerName" placeholder="Your Name" required>

      <input type="tel" id="customerPhone" placeholder="Phone Number" required>

      <textarea id="customerAddress" rows="3" placeholder="Address"></textarea>

      <button class="send-order" onclick="sendOrder()">
        Send Order
      </button>
    </div>
  </div>

  <!-- WHATSAPP -->
  <a href="https://wa.me/919800200813" class="whatsapp-btn" target="_blank">
    💬
  </a>

  <!-- FOOTER -->
  <footer>
    © 2026 Ranjit Enterprises | Best Product At Best Price
  </footer>

  <!-- EMAILJS -->
  <script src="https://cdn.jsdelivr.net/npm/@emailjs/browser@4/dist/email.min.js"></script>

  <script>

    // EMAILJS INIT
    emailjs.init("YOUR_PUBLIC_KEY");

    // PRODUCTS
    const products = [
      {
        name:"Premium Product 1",
        price:"₹499",
        image:"https://i.ibb.co/whLTQBxk/IMG-20260410-WA0007.jpg"
      },
      {
        name:"Premium Product 2",
        price:"₹599",
        image:"https://i.ibb.co/LdrtvJdX/IMG-20260407-WA0029.jpg"
      },
      {
        name:"Premium Product 3",
        price:"₹699",
        image:"https://i.ibb.co/PZmTnZKF/IMG-20260313-WA0000.jpg"
      },
      {
        name:"Premium Product 4",
        price:"₹799",
        image:"https://i.ibb.co/3Y9wgkYM/IMG-20260408-WA0046.jpg"
      },
      {
        name:"Premium Product 5",
        price:"₹899",
        image:"https://i.ibb.co/gMZ0RX2V/IMG-20260408-WA0045.jpg"
      },
      {
        name:"Premium Product 6",
        price:"₹999",
        image:"https://i.ibb.co/F477YgbZ/IMG-20260407-WA0008.jpg"
      },
      {
        name:"Premium Product 7",
        price:"₹1199",
        image:"https://i.ibb.co/8ZjRBJN/IMG-20260407-WA0034.jpg"
      },
      {
        name:"Premium Product 8",
        price:"₹1299",
        image:"https://i.ibb.co/TCXvM52/IMG-20260312-WA0037.jpg"
      },
      {
        name:"Premium Product 9",
        price:"₹1399",
        image:"https://i.ibb.co/ccj4k6G2/IMG-20251106-WA0004.jpg"
      },
      {
        name:"Premium Product 10",
        price:"₹1499",
        image:"https://i.ibb.co/LzSD8YHV/IMG-20251106-WA0003.jpg"
      }
    ];

    const productContainer = document.getElementById("productContainer");

    let cart = [];

    // RENDER PRODUCTS
    products.forEach((product,index)=>{

      productContainer.innerHTML += `
        <div class="product-card">
          <img src="${product.image}" alt="${product.name}">

          <div class="product-info">
            <h3>${product.name}</h3>

            <div class="price">${product.price}</div>

            <button class="add-cart" onclick="addToCart(${index})">
              Add To Cart
            </button>
          </div>
        </div>
      `;
    });

    // ADD TO CART
    function addToCart(index){

      cart.push(products[index]);

      updateCart();

      alert(products[index].name + " added to cart!");
    }

    // UPDATE CART
    function updateCart(){

      document.getElementById("cartCount").innerText = cart.length;

      const cartItems = document.getElementById("cartItems");

      cartItems.innerHTML = "";

      cart.forEach((item,index)=>{

        cartItems.innerHTML += `
          <div class="cart-item">
            <div>
              <strong>${item.name}</strong><br>
              ${item.price}
            </div>

            <button onclick="removeItem(${index})">
              X
            </button>
          </div>
        `;
      });
    }

    // REMOVE ITEM
    function removeItem(index){

      cart.splice(index,1);

      updateCart();
    }

    // OPEN CART
    function openCart(){

      document.getElementById("cartModal").classList.add("active");
    }

    // CLOSE CART
    function closeCart(){

      document.getElementById("cartModal").classList.remove("active");
    }

    // SEND ORDER
    function sendOrder(){

      const name = document.getElementById("customerName").value;
      const phone = document.getElementById("customerPhone").value;
      const address = document.getElementById("customerAddress").value;

      if(cart.length === 0){
        alert("Your cart is empty!");
        return;
      }

      if(name === "" || phone === ""){
        alert("Please fill all details");
        return;
      }

      let orderList = "";

      cart.forEach((item,index)=>{
        orderList += `${index+1}. ${item.name} - ${item.price}\n`;
      });

      const templateParams = {

        customer_name:name,

        customer_phone:phone,

        customer_address:address,

        order_items:orderList,

        owner_email:"ramanbhagat1422@gmail.com"
      };

      emailjs.send(
        "YOUR_SERVICE_ID",
        "YOUR_TEMPLATE_ID",
        templateParams
      )
      .then(function(){

        alert("Order Sent Successfully!");

        cart = [];

        updateCart();

        document.getElementById("customerName").value = "";
        document.getElementById("customerPhone").value = "";
        document.getElementById("customerAddress").value = "";

        closeCart();

      }, function(error){

        alert("Failed To Send Order");
        console.log(error);
      });
    }

    // AUTO SLIDE
    let scrollAmount = 0;

    setInterval(()=>{

      const container = document.querySelector('.products-wrapper');

      scrollAmount += 300;

      if(scrollAmount >= container.scrollWidth - container.clientWidth){
        scrollAmount = 0;
      }

      container.scrollTo({
        left:scrollAmount,
        behavior:'smooth'
      });

    },3000);

  </script>

</body>
</html>
