import React, { useState, useEffect } from "react";
import { motion, AnimatePresence } from "framer-motion";
import { ShoppingCart, Moon, Sun, X, CheckCircle, Heart, Search } from "lucide-react";
import { Button } from "@/components/ui/button";
import { Card, CardContent } from "@/components/ui/card";

const products = [
  { id: 1, name: "Golden Crunch Fries", price: "5.99", category: "Fries", description: "Crispy outside, fluffy inside – perfect homemade fries." },
  { id: 2, name: "Creamy Yukon Gold", price: "6.49", category: "Fresh", description: "Buttery smooth potatoes ideal for mashing." },
  { id: 3, name: "Sweet Sunset Gems", price: "7.25", category: "Sweet", description: "Naturally sweet and packed with nutrients." },
  { id: 4, name: "Garlic Herb Spuds", price: "6.99", category: "Seasoned", description: "Infused with aromatic garlic and herbs." },
  { id: 5, name: "BBQ Roast Pack", price: "8.50", category: "Seasoned", description: "Smoky flavored potatoes for grill nights." },
  { id: 6, name: "Mini Baby Taters", price: "5.49", category: "Fresh", description: "Small, tender potatoes perfect for roasting." },
  { id: 7, name: "Classic Fry Cut", price: "6.30", category: "Fries", description: "Perfectly sliced for golden frying." },
  { id: 8, name: "Hash Brown Ready", price: "6.85", category: "Breakfast", description: "Shredded potatoes for crispy breakfasts." },
  { id: 9, name: "Potato Wedges Supreme", price: "8.45", category: "Fries", description: "Thick-cut wedges for sharing." },
  { id: 10, name: "Truffle Luxury Box", price: "12.99", category: "Premium", description: "Infused with elegant truffle aroma." },
  { id: 11, name: "Purple Majesty", price: "8.20", category: "Premium", description: "Rich purple potatoes with antioxidants." },
  { id: 12, name: "Air Fry Healthy Pack", price: "7.60", category: "Healthy", description: "Optimized for crispy air frying." },
  { id: 13, name: "Spicy Fiesta Bites", price: "7.95", category: "Seasoned", description: "Bold spicy flavor explosion." },
  { id: 14, name: "Loaded Baked Kit", price: "10.50", category: "Premium", description: "Everything for loaded baked potatoes." },
  { id: 15, name: "Organic Farm Russet", price: "6.70", category: "Fresh", description: "Farm-grown and naturally harvested." },
  { id: 16, name: "Cheesy Seasoned Spuds", price: "9.40", category: "Seasoned", description: "Cheese-blended flavor boost." },
  { id: 17, name: "Butter Roast Selection", price: "8.10", category: "Premium", description: "Perfect for buttery oven roasting." },
  { id: 18, name: "Breakfast Gold Cubes", price: "6.95", category: "Breakfast", description: "Golden cubes for morning meals." },
  { id: 19, name: "Sweet Potato Deluxe", price: "7.75", category: "Sweet", description: "Premium sweet potato experience." },
  { id: 20, name: "Ultimate Tato Feast", price: "15.99", category: "Premium", description: "All-in-one curated potato feast box." },
];

export default function TatoAisleWebsite() {
  const [cart, setCart] = useState([]);
  const [wishlist, setWishlist] = useState([]);
  const [darkMode, setDarkMode] = useState(false);
  const [showCart, setShowCart] = useState(false);
  const [showSuccess, setShowSuccess] = useState(false);
  const [search, setSearch] = useState("");
  const [category, setCategory] = useState("All");
  const [orders, setOrders] = useState([]);

  useEffect(() => {
    const savedCart = localStorage.getItem("tato_cart");
    if (savedCart) setCart(JSON.parse(savedCart));
  }, []);

  useEffect(() => {
    localStorage.setItem("tato_cart", JSON.stringify(cart));
  }, [cart]);

  const addToCart = (product) => setCart([...cart, product]);
  const removeFromCart = (index) => setCart(cart.filter((_, i) => i !== index));
  const toggleWishlist = (id) => {
    setWishlist(wishlist.includes(id) ? wishlist.filter((w) => w !== id) : [...wishlist, id]);
  };

  const handleCheckout = () => {
    if (!cart.length) return;
    setOrders([...orders, { id: Date.now(), items: cart, total }]);
    setCart([]);
    setShowSuccess(true);
    setTimeout(() => {
      setShowSuccess(false);
      setShowCart(false);
    }, 2500);
  };

  const total = cart.reduce((sum, item) => sum + parseFloat(item.price), 0).toFixed(2);

  const filteredProducts = products.filter((p) =>
    (category === "All" || p.category === category) &&
    p.name.toLowerCase().includes(search.toLowerCase())
  );

  return (
    <div className={`${darkMode ? "bg-gray-950 text-white" : "bg-gradient-to-br from-yellow-100 via-orange-100 to-pink-100 text-gray-800"} min-h-screen transition-all duration-700`}>
      
      {/* NAVBAR */}
      <nav className="flex justify-between items-center p-6 backdrop-blur-lg bg-white/30 dark:bg-gray-800/40 sticky top-0 z-50 shadow-xl">
        <h1 className="text-2xl font-bold">🥔 Tato Aisle</h1>
        <div className="flex gap-4 items-center">
          <div className="relative">
            <Search className="absolute left-2 top-2.5" size={16} />
            <input
              placeholder="Search..."
              value={search}
              onChange={(e) => setSearch(e.target.value)}
              className="pl-8 pr-2 py-1 rounded-lg text-black"
            />
          </div>
          <select
            value={category}
            onChange={(e) => setCategory(e.target.value)}
            className="rounded-lg px-2 py-1 text-black"
          >
            <option>All</option>
            <option>Fresh</option>
            <option>Fries</option>
            <option>Premium</option>
            <option>Seasoned</option>
            <option>Breakfast</option>
            <option>Sweet</option>
            <option>Healthy</option>
          </select>
          <Button onClick={() => setDarkMode(!darkMode)}>
            {darkMode ? <Sun size={18} /> : <Moon size={18} />}
          </Button>
          <Button onClick={() => setShowCart(true)} className="relative">
            <ShoppingCart size={18} />
            {cart.length > 0 && (
              <span className="absolute -top-2 -right-2 bg-red-500 text-xs px-2 py-0.5 rounded-full">
                {cart.length}
              </span>
            )}
          </Button>
        </div>
      </nav>

      {/* PRODUCTS */}
      <section className="grid md:grid-cols-4 gap-8 px-10 py-16">
        {filteredProducts.map((product) => (
          <motion.div key={product.id} whileHover={{ scale: 1.05 }}>
            <Card className="rounded-2xl shadow-xl dark:bg-gray-800">
              <div className="h-40 bg-gradient-to-br from-yellow-300 to-orange-400" />
              <CardContent className="p-6">
                <div className="flex justify-between items-center">
                  <h3 className="font-semibold">{product.name}</h3>
                  <Heart
                    size={18}
                    onClick={() => toggleWishlist(product.id)}
                    className={`cursor-pointer ${wishlist.includes(product.id) ? "text-red-500" : ""}`}
                  />
                </div>
                <p className="text-sm mb-2">{product.description}</p>
                <p className="font-bold mb-4">${product.price}</p>
                <Button onClick={() => addToCart(product)} className="w-full">
                  Add to Cart
                </Button>
              </CardContent>
            </Card>
          </motion.div>
        ))}
      </section>

      {/* CART */}
      <AnimatePresence>
        {showCart && (
          <motion.div
            initial={{ x: "100%" }}
            animate={{ x: 0 }}
            exit={{ x: "100%" }}
            className="fixed top-0 right-0 w-80 h-full bg-white dark:bg-gray-900 shadow-2xl p-6 z-50"
          >
            <div className="flex justify-between mb-6">
              <h2 className="font-bold">Your Cart</h2>
              <Button onClick={() => setShowCart(false)}><X size={16} /></Button>
            </div>
            {cart.map((item, i) => (
              <div key={i} className="flex justify-between mb-2">
                <span>{item.name}</span>
                <Button size="sm" onClick={() => removeFromCart(i)}>Remove</Button>
              </div>
            ))}
            <p className="font-bold mt-4">Total: ${total}</p>
            <Button onClick={handleCheckout} className="w-full mt-4">Checkout</Button>
          </motion.div>
        )}
      </AnimatePresence>

      {/* SUCCESS */}
      <AnimatePresence>
        {showSuccess && (
          <motion.div className="fixed inset-0 flex items-center justify-center bg-black/50">
            <div className="bg-white dark:bg-gray-800 p-10 rounded-2xl text-center">
              <CheckCircle className="mx-auto mb-4 text-green-500" size={48} />
              <h2 className="text-xl font-bold">Order Confirmed!</h2>
            </div>
          </motion.div>
        )}
      </AnimatePresence>

      {/* FOOTER */}
      <footer className="text-center py-6 bg-white/30 dark:bg-gray-800/40">
        © {new Date().getFullYear()} Tato Aisle
      </footer>
    </div>
  );
}
