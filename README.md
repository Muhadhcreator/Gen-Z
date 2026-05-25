index.html
style.css
script.js
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Men T-Shirt Store</title>
  <link rel="stylesheet" href="style.css"/>
</head>
<body>

  <header>
    <h1>Men T-Shirt Store</h1>
    <p>Premium Fashion Collection</p>
  </header>

  <section class="products">

    <div class="card">
      <img src="https://images.unsplash.com/photo-1521572163474-6864f9cf17ab" alt="">
      <h2>Black T-Shirt</h2>
      <p>$20</p>
      <button onclick="orderNow('Black T-Shirt')">
        Order Now
      </button>
    </div>

    <div class="card">
      <img src="https://images.unsplash.com/photo-1503341504253-dff4815485f1" alt="">
      <h2>White Oversized</h2>
      <p>$25</p>
      <button onclick="orderNow('White Oversized')">
        Order Now
      </button>
    </div>

    <div class="card">
      <img src="https://images.unsplash.com/photo-1489987707025-afc232f7ea0f" alt="">
      <h2>Streetwear Tee</h2>
      <p>$30</p>
      <button onclick="orderNow('Streetwear Tee')">
        Order Now
      </button>
    </div>

  </section>

  <script src="script.js"></script>
</body>
</html>
body{
  margin:0;
  font-family:Arial;
  background:#111;
  color:white;
}

header{
  text-align:center;
  padding:30px;
  background:black;
}

.products{
  display:grid;
  grid-template-columns:1fr;
  gap:20px;
  padding:20px;
}

.card{
  background:#1e1e1e;
  border-radius:15px;
  overflow:hidden;
  box-shadow:0 0 10px rgba(255,255,255,0.1);
}

.card img{
  width:100%;
  height:300px;
  object-fit:cover;
}

.card h2,p{
  padding-left:15px;
}

button{
  margin:15px;
  padding:12px;
  width:90%;
  border:none;
  border-radius:10px;
  background:#ff3c3c;
  color:white;
  font-size:16px;
}
function orderNow(product){

  let phone = "947XXXXXXXX";

  let message =
   "Hello, I want to order: " + product;

  let url =
   "https://wa.me/" + phone +
   "?text=" + encodeURIComponent(message);

  window.open(url, "_blank");
}
94754668668
