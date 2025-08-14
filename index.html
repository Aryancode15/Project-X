import React, { useEffect, useMemo, useState } from "react";

/**
 * Premium Ebook Store (single-file React + Tailwind)
 * - Splash screen with animated logo
 * - Premium, minimal theme (slate / indigo / gold accents)
 * - Hero, Product grid (₹29/₹49/₹99), Add to Cart, Buy Now
 * - Drawer Cart & lightweight checkout modal (no external UI libs)
 * - No shadcn/ui dependency so it runs with just React + Tailwind
 */

const BOOKS = [
  {
    id: "atomic-habits",
    title: "Atomic Habits (Summary)",
    author: "James Clear",
    price: 49,
    cover: "https://placehold.co/400x560/0f172a/FFFFFF?text=Atomic+Habits\nSummary",
    blurb:
      "A crisp, 25‑page summary that turns habits into a system you can follow daily.",
    learn: [
      "4-step habit loop you can apply",
      "Design your environment for success",
      "Tiny gains → compounding results",
    ],
  },
  {
    id: "rich-dad-poor-dad",
    title: "Rich Dad Poor Dad (Summary)",
    author: "Robert Kiyosaki",
    price: 29,
    cover: "https://placehold.co/400x560/111827/FFFFFF?text=Rich+Dad\nPoor+Dad\nSummary",
    blurb:
      "Mindset shifts about money, assets vs liabilities, and building cashflow.",
    learn: [
      "Assets vs liabilities (simple test)",
      "Earn → Save → Invest flywheel",
      "Cashflow thinking over salary",
    ],
  },
  {
    id: "psychology-of-money",
    title: "The Psychology of Money (Summary)",
    author: "Morgan Housel",
    price: 99,
    cover:
      "https://placehold.co/400x560/0b1220/FFFFFF?text=Psychology+of+Money\nSummary",
    blurb:
      "Timeless rules for behavior around money, risk, and long‑term thinking.",
    learn: [
      "Why behavior beats math",
      "Tail events & risk management",
      "Staying rich vs getting rich",
    ],
  },
];

// ---------- Small UI helpers ----------
const Currency = ({ value }) => <span>₹{Number(value).toLocaleString("en-IN")}</span>;

function IconBag() {
  return (
    <svg width="20" height="20" viewBox="0 0 24 24" fill="none" aria-hidden>
      <path d="M6 7h12l-1 13H7L6 7Z" stroke="currentColor" strokeWidth="1.5" />
      <path d="M9 7a3 3 0 0 1 6 0" stroke="currentColor" strokeWidth="1.5" />
    </svg>
  );
}
function IconFlash() {
  return (
    <svg width="18" height="18" viewBox="0 0 24 24" fill="none" aria-hidden>
      <path d="M13 2 3 14h7v8l11-14h-8l0-6Z" fill="currentColor" />
    </svg>
  );
}
function IconClose(props) {
  return (
    <svg width="20" height="20" viewBox="0 0 24 24" {...props}>
      <path d="M6 6l12 12M18 6 6 18" stroke="currentColor" strokeWidth="1.6" />
    </svg>
  );
}

// ---------- Splash (animated logo) ----------
function Splash({ onDone }) {
  useEffect(() => {
    const t = setTimeout(onDone, 1800);
    return () => clearTimeout(t);
  }, [onDone]);

  return (
    <div className="fixed inset-0 z-[70] grid place-items-center bg-slate-950">
      <div className="relative">
        {/* Outer ring */}
        <div className="absolute inset-0 rounded-full border border-slate-700/60 animate-ping" />
        {/* Logo mark */}
        <div className="h-24 w-24 rounded-3xl bg-gradient-to-br from-indigo-500 via-indigo-400 to-amber-400 shadow-2xl shadow-indigo-900/40 grid place-items-center animate-[pulse_1.2s_ease-in-out_infinite]">
          <IconFlash />
        </div>
        <div className="mt-5 text-center">
          <p className="text-slate-300 tracking-wider text-sm">EBOOK STUDIO</p>
        </div>
      </div>
    </div>
  );
}

// ---------- Product Card ----------
function ProductCard({ book, onAdd, onBuy }) {
  return (
    <div className="group rounded-2xl bg-white/90 border border-slate-200/80 backdrop-blur-sm shadow-sm hover:shadow-xl transition-all duration-300 overflow-hidden">
      <div className="relative">
        <img src={book.cover} alt={book.title} className="h-72 w-full object-cover" />
        <div className="absolute inset-x-0 bottom-0 p-4 bg-gradient-to-t from-slate-900/90 to-transparent">
          <h3 className="text-white font-semibold leading-tight drop-shadow">{book.title}</h3>
          <p className="text-amber-300 font-semibold mt-1"><Currency value={book.price} /> only</p>
        </div>
      </div>
      <div className="p-4">
        <p className="text-sm text-slate-600 line-clamp-3">{book.blurb}</p>
        <div className="mt-4 flex gap-3">
          <button
            onClick={() => onAdd(book)}
            className="flex-1 inline-flex items-center justify-center rounded-xl border border-slate-300 bg-white px-4 py-2 text-slate-800 hover:bg-slate-50 active:scale-[.98]"
          >
            <IconBag />
            <span className="ml-2">Add to Cart</span>
          </button>
          <button
            onClick={() => onBuy(book)}
            className="flex-1 rounded-xl bg-slate-900 text-white px-4 py-2 hover:bg-slate-800 active:scale-[.98]"
          >
            Buy Now
          </button>
        </div>
      </div>
    </div>
  );
}

// ---------- Cart Drawer ----------
function CartDrawer({ open, onClose, items, onRemove, onCheckout }) {
  const total = useMemo(() => items.reduce((s, i) => s + i.price, 0), [items]);
  return (
    <div className={`fixed inset-0 z-50 ${open ? "" : "pointer-events-none"}`}>
      <div
        className={`absolute inset-0 bg-slate-900/50 transition-opacity ${open ? "opacity-100" : "opacity-0"}`}
        onClick={onClose}
      />
      <aside
        className={`absolute right-0 top-0 h-full w-full max-w-md bg-white shadow-2xl p-6 transition-transform duration-300 ${open ? "translate-x-0" : "translate-x-full"}`}
      >
        <div className="flex items-center justify-between">
          <h4 className="text-lg font-semibold">Your Cart</h4>
          <button onClick={onClose} className="text-slate-500 hover:text-slate-800"><IconClose /></button>
        </div>
        <div className="mt-4 space-y-3 max-h-[65vh] overflow-auto pr-2">
          {items.length === 0 && (
            <p className="text-slate-500">Cart is empty.</p>
          )}
          {items.map((b) => (
            <div key={b.id} className="flex items-center gap-3 rounded-xl border border-slate-200 p-3">
              <img src={b.cover} alt="" className="h-16 w-12 object-cover rounded-lg" />
              <div className="flex-1">
                <p className="text-sm font-medium text-slate-800">{b.title}</p>
                <p className="text-sm text-slate-500"><Currency value={b.price} /></p>
              </div>
              <button onClick={() => onRemove(b.id)} className="text-slate-500 hover:text-rose-600">Remove</button>
            </div>
          ))}
        </div>
        <div className="mt-6 border-t pt-4">
          <div className="flex items-center justify-between text-slate-700">
            <span>Total</span>
            <span className="text-lg font-semibold"><Currency value={total} /></span>
          </div>
          <button
            disabled={items.length === 0}
            onClick={onCheckout}
            className="mt-4 w-full rounded-xl bg-slate-900 text-white py-3 hover:bg-slate-800 disabled:opacity-40"
          >
            Checkout
          </button>
        </div>
      </aside>
    </div>
  );
}

// ---------- Checkout Modal (mock) ----------
function CheckoutModal({ open, onClose, book, onPay }) {
  if (!open) return null;
  return (
    <div className="fixed inset-0 z-50">
      <div className="absolute inset-0 bg-slate-900/50" onClick={onClose} />
      <div className="absolute left-1/2 top-1/2 -translate-x-1/2 -translate-y-1/2 w-[92vw] max-w-lg rounded-2xl bg-white shadow-2xl p-6">
        <div className="flex items-start justify-between">
          <div>
            <h4 className="text-xl font-semibold">Instant Checkout</h4>
            <p className="text-sm text-slate-500 mt-1">Secure payment & immediate download</p>
          </div>
          <button onClick={onClose} className="text-slate-500 hover:text-slate-800"><IconClose /></button>
        </div>
        <div className="mt-5 flex gap-4">
          <img src={book.cover} alt="" className="h-24 w-18 object-cover rounded-lg" />
          <div className="flex-1">
            <p className="font-medium text-slate-800">{book.title}</p>
            <p className="text-slate-500 text-sm mt-1">{book.blurb}</p>
          </div>
          <div className="text-right">
            <p className="text-sm text-slate-500">Price</p>
            <p className="text-lg font-semibold"><Currency value={book.price} /></p>
          </div>
        </div>
        <button onClick={onPay} className="mt-6 w-full rounded-xl bg-slate-900 text-white py-3 hover:bg-slate-800">
          Proceed to Payment
        </button>
        <p className="text-xs text-slate-500 mt-3 text-center">You’ll be redirected to a secure gateway. After success, your download starts instantly.</p>
      </div>
    </div>
  );
}

// ---------- Main App ----------
export default function PremiumEbookStore() {
  const [showSplash, setShowSplash] = useState(true);
  const [cartOpen, setCartOpen] = useState(false);
  const [items, setItems] = useState([]);
  const [query, setQuery] = useState("");
  const [buyNowBook, setBuyNowBook] = useState(null);

  const filtered = useMemo(() => {
    const q = query.trim().toLowerCase();
    if (!q) return BOOKS;
    return BOOKS.filter((b) => b.title.toLowerCase().includes(q) || b.author.toLowerCase().includes(q));
  }, [query]);

  const addToCart = (book) => {
    setItems((prev) => (prev.find((i) => i.id === book.id) ? prev : [...prev, book]));
  };
  const removeFromCart = (id) => setItems((prev) => prev.filter((i) => i.id !== id));

  const handleCheckout = () => {
    // TODO: integrate Razorpay/Instamojo here.
    alert("Checkout pressed — integrate Razorpay/Instamojo here.");
  };

  const handlePay = () => {
    // Replace with live gateway integration.
    alert("Proceed to payment — plug your gateway here.");
    setBuyNowBook(null);
  };

  return (
    <div className="min-h-screen bg-gradient-to-b from-slate-50 to-white text-slate-900 selection:bg-amber-200/60">
      {showSplash && <Splash onDone={() => setShowSplash(false)} />}

      {/* Header */}
      <header className="sticky top-0 z-40 bg-white/80 backdrop-blur border-b border-slate-200/70">
        <div className="mx-auto max-w-6xl px-4 py-4 flex items-center justify-between">
          <div className="flex items-center gap-3">
            <div className="h-8 w-8 rounded-xl bg-gradient-to-br from-indigo-500 to-amber-400 grid place-items-center text-white shadow">
              <IconFlash />
            </div>
            <span className="font-semibold tracking-tight">Ebook Studio</span>
          </div>
          <nav className="hidden md:flex items-center gap-6 text-sm text-slate-600">
            <a href="#shop" className="hover:text-slate-900">Shop</a>
            <a href="#benefits" className="hover:text-slate-900">Benefits</a>
            <a href="#about" className="hover:text-slate-900">About</a>
            <a href="#contact" className="hover:text-slate-900">Contact</a>
          </nav>
          <div className="flex items-center gap-3">
            <div className="relative hidden sm:block">
              <input
                value={query}
                onChange={(e) => setQuery(e.target.value)}
                placeholder="Search summaries…"
                className="peer w-56 rounded-xl border border-slate-300 bg-white px-3 py-2 text-sm outline-none focus:border-slate-900"
              />
              <span className="pointer-events-none absolute right-3 top-1/2 -translate-y-1/2 text-slate-400">⌕</span>
            </div>
            <button
              onClick={() => setCartOpen(true)}
              className="inline-flex items-center gap-2 rounded-xl border border-slate-300 px-3 py-2 text-sm hover:bg-slate-50"
            >
              <IconBag />
              <span>Cart ({items.length})</span>
            </button>
          </div>
        </div>
      </header>

      {/* Hero */}
      <section className="relative isolate">
        <div className="mx-auto max-w-6xl px-4 py-16">
          <div className="grid md:grid-cols-2 items-center gap-10">
            <div>
              <h1 className="text-4xl md:text-5xl font-semibold leading-tight tracking-tight">Learn from bestselling books in minutes.</h1>
              <p className="mt-4 text-slate-600 md:text-lg max-w-prose">Professionally crafted summaries with actionable insights and bonus reading prompts. No fluff. Pure value.</p>
              <div className="mt-6 flex gap-3">
                <a href="#shop" className="rounded-xl bg-slate-900 text-white px-5 py-3 text-sm hover:bg-slate-800">Browse Summaries</a>
                <a href="#benefits" className="rounded-xl border border-slate-300 px-5 py-3 text-sm hover:bg-slate-50">Why Us</a>
              </div>
            </div>
            <div className="relative">
              <div className="aspect-[4/3] rounded-3xl bg-gradient-to-br from-indigo-50 to-amber-50 border border-slate-200 shadow-inner" />
              <div className="absolute -bottom-6 -right-6 h-20 w-20 rounded-2xl bg-gradient-to-br from-indigo-500 to-amber-400 blur-xl opacity-30" />
            </div>
          </div>
        </div>
      </section>

      {/* Shop */}
      <section id="shop" className="mx-auto max-w-6xl px-4 py-12">
        <div className="flex items-end justify-between">
          <div>
            <h2 className="text-2xl font-semibold">Trending Summaries</h2>
            <p className="text-slate-600">Premium insights, instant downloads</p>
          </div>
          <div className="text-sm text-slate-500">Prices: ₹29 / ₹49 / ₹99</div>
        </div>
        <div className="mt-6 grid gap-6 sm:grid-cols-2 lg:grid-cols-3">
          {filtered.map((b) => (
            <ProductCard key={b.id} book={b} onAdd={addToCart} onBuy={setBuyNowBook} />
          ))}
        </div>
      </section>

      {/* Benefits */}
      <section id="benefits" className="bg-white/60 border-y border-slate-200/70">
        <div className="mx-auto max-w-6xl px-4 py-12 grid md:grid-cols-3 gap-8">
          {[
            { title: "Save Time", desc: "Read the key ideas in 10–15 minutes with action steps." },
            { title: "Learn Anywhere", desc: "Clean PDFs & mobile‑friendly summaries for on‑the‑go learning." },
            { title: "Premium Quality", desc: "Carefully edited, professionally designed, no fluff." },
          ].map((f) => (
            <div key={f.title} className="rounded-2xl border border-slate-200 p-6 bg-white">
              <div className="h-10 w-10 rounded-xl bg-slate-900 text-white grid place-items-center mb-4"><IconFlash /></div>
              <h3 className="font-semibold">{f.title}</h3>
              <p className="text-sm text-slate-600 mt-1">{f.desc}</p>
            </div>
          ))}
        </div>
      </section>

      {/* About & Contact (simple placeholders) */}
      <section id="about" className="mx-auto max-w-6xl px-4 py-12">
        <h2 className="text-2xl font-semibold">About</h2>
        <p className="text-slate-600 mt-2 max-w-prose">We craft concise, high‑value book summaries to help busy people learn faster. Each summary includes practical frameworks and prompts you can apply the same day.</p>
      </section>
      <section id="contact" className="mx-auto max-w-6xl px-4 py-12">
        <h2 className="text-2xl font-semibold">Contact</h2>
        <p className="text-slate-600 mt-2">Email: hello@ebookstudio.example • Instagram: @ebookstudio</p>
      </section>

      {/* Footer */}
      <footer className="border-t border-slate-200/70 bg-white/60">
        <div className="mx-auto max-w-6xl px-4 py-8 text-sm text-slate-500 flex flex-col sm:flex-row items-center justify-between">
          <p>© {new Date().getFullYear()} Ebook Studio. All rights reserved.</p>
          <div className="mt-3 sm:mt-0">Made with ♥ for readers</div>
        </div>
      </footer>

      <CartDrawer
        open={cartOpen}
        onClose={() => setCartOpen(false)}
        items={items}
        onRemove={removeFromCart}
        onCheckout={handleCheckout}
      />

      <CheckoutModal open={!!buyNowBook} onClose={() => setBuyNowBook(null)} book={buyNowBook || BOOKS[0]} onPay={handlePay} />
    </div>
  );
}
