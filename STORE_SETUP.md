# STORE_SETUP — Halal Da Nang GrabFood Portal Playbook

> Field-by-field GrabMerchant data-entry guide. Store: halal cloud kitchen, **Đà Nẵng, Vietnam**.
> Menu structure source = `SOT.md`; **prices here are FINAL Da Nang prices and override SOT.md** (SOT is stale, orchestrator to update).
> App: GrabMerchant (iPad). Nav: bottom **Menu** → top tabs **Items** / **Option Groups**.
> Naming: single Name field, **English – Vietnamese** (brand product names kept as-is).
> Image spec: 800×800px, JPEG/PNG, **≤2MB each (up to 4 photos)**. Prices shown for options = *add-on* amount.
> Item form field order: Item name → Item photo → Description → Category → Price → Option groups → Availability schedule.
> ⚠️ = priced but **pending ingredient confirmation** (SOT §3) — do not go live until confirmed.

Status: Categories 1–4 drafted.

---

## Category 1: Custom Noodle Bar – Tự Làm Mì Trộn Cay

### Step 1 — Create the Category
**Menu → Items tab → + Add category**
| Field | Value |
|---|---|
| Category name | Custom Noodle Bar – Tự Làm Mì Trộn Cay |

(Existing categories: Healthy Fruit Juice / Soft Drink / Finger Food — this adds a new one.)

### Step 2 — Base option group (reuse existing)
**Menu → Option Groups tab → open "Chọn Cấp Độ Cay (Choose Your Noodle Base)"** (0 items linked)
1. Rename → **Name:** Pick Your Noodle – Chọn Sợi Mì
2. **+ Add an option** (brand names kept as-is):
| Option name | Price |
|---|---|
| Mi Sedaap Korean Spicy Chicken | 0₫ (default) |
| Samyang Quattro Cheese | 6.000₫ |
| Samyang Habanero Lime | 6.000₫ |
| Samyang 2x Spicy | 8.000₫ |
3. Toggles: **Make mandatory = ON**, **Allow multiple selections = OFF** → **Save**

### Step 3 — Toppings option group (new)
**Menu → Option Groups tab → + Add an option group → "Toppings" template** (or New)
1. **Name:** Toppings – Topping
2. **+ Add an option:**
| Option name | Price | Status |
|---|---|---|
| Boiled Egg – Trứng Luộc | 8.000₫ | Live |
| Tofu – Đậu Hũ | 12.000₫ | Live |
| K&U Popcorn Chicken – Gà Popcorn K&U | 29.000₫ | Live |
| Chicken Strips – Gà Strips | 29.000₫ | Live |
| Chicken Skewer – Gà Xiên | 15.000₫ | Live |
| Fried Shrimp – Tôm Chiên | 35.000₫ | ⚠️ PENDING (shrimp) |
3. Toggles: **Make mandatory = OFF**, **Allow multiple selections = ON** → **Save**

(Don't reuse the generic "Thêm vị món ăn càng ngon" group — shared by 4 other items, prices differ.)

### Step 4 — Item
| # | Field | Value |
|---|---|---|
| 1 | Item name | Custom Noodle Bowl – Tự Làm Mì Trộn Cay |
| 2 | Item photo | 800×800px, ≤2MB |
| 3 | Description | Build-your-own spicy mixed-noodle bowl — pick your noodle, stack your toppings. / Bát mì trộn cay tự chọn — chọn sợi mì, thêm topping tuỳ thích. |
| 4 | Category | Custom Noodle Bar – Tự Làm Mì Trộn Cay |
| 5 | Price | 39.000₫ |
| 6 | Option groups | Link **Pick Your Noodle** + **Toppings** |
| 7 | Availability schedule | All opening hours |

---

## Category 2: Burgers & Chicken Mains – Burger & Món Gà

### Step 1 — Create the Category
**Menu → Items tab → + Add category**
| Field | Value |
|---|---|
| Category name | Burgers & Chicken Mains – Burger & Món Gà |

### Step 2 — Sauce option group (for Bánh Gà)
**Menu → Option Groups tab → + Add an option group → New**
1. **Name:** Choose Your Sauce – Chọn Sốt
2. **+ Add an option:**
| Option name | Price | Note |
|---|---|---|
| Tomato & Mayo – Cà Chua & Mayo | 0₫ | list first = default |
| Chilli – Ớt | 0₫ | |
3. Toggles: **Make mandatory = ON**, **Allow multiple selections = OFF** → **Save**

### Step 3 — Item: Chicken Patty, Choice of Sauce
| # | Field | Value |
|---|---|---|
| 1 | Item name | Chicken Patty, Choice of Sauce – Bánh Gà Sốt Tự Chọn |
| 2 | Item photo | 800×800px, ≤2MB |
| 3 | Description | Crispy chicken patty with your choice of sauce. / Bánh gà giòn, chọn sốt tuỳ thích. |
| 4 | Category | Burgers & Chicken Mains – Burger & Món Gà |
| 5 | Price | 49.000₫ |
| 6 | Option groups | Link **Choose Your Sauce** |
| 7 | Availability schedule | All opening hours |

### Step 4 — Item: Hamburger Cheese
| # | Field | Value |
|---|---|---|
| 1 | Item name | Hamburger Cheese – Burger Bò Phô Mai |
| 2 | Item photo | 800×800px, ≤2MB |
| 3 | Description | Grilled beef patty with cheese & tomato sauce, served with chips. / Bánh bò nướng với phô mai & sốt cà chua, ăn kèm khoai tây chiên. |
| 4 | Category | Burgers & Chicken Mains – Burger & Món Gà |
| 5 | Price | 160.000₫ |
| 6 | Option groups | none |
| 7 | Availability schedule | All opening hours |

### Step 5 — Item: Hamburger Egg
| # | Field | Value |
|---|---|---|
| 1 | Item name | Hamburger Egg – Burger Bò Trứng |
| 2 | Item photo | 800×800px, ≤2MB |
| 3 | Description | Grilled beef patty with egg, cheese & tomato sauce, served with chips. / Bánh bò nướng với trứng, phô mai & sốt cà chua, ăn kèm khoai tây chiên. |
| 4 | Category | Burgers & Chicken Mains – Burger & Món Gà |
| 5 | Price | 170.000₫ |
| 6 | Option groups | none |
| 7 | Availability schedule | All opening hours |

### Step 6 — Item: Double Hamburger
| # | Field | Value |
|---|---|---|
| 1 | Item name | Double Hamburger – Burger Bò Đôi |
| 2 | Item photo | 800×800px, ≤2MB |
| 3 | Description | Two grilled beef patties & two slices of cheese with tomato sauce, served with chips. / Hai bánh bò nướng & hai lát phô mai với sốt cà chua, ăn kèm khoai tây chiên. |
| 4 | Category | Burgers & Chicken Mains – Burger & Món Gà |
| 5 | Price | 250.000₫ |
| 6 | Option groups | none |
| 7 | Availability schedule | All opening hours |

### Step 7 — Item: Chicken Burger
| # | Field | Value |
|---|---|---|
| 1 | Item name | Chicken Burger – Burger Gà |
| 2 | Item photo | 800×800px, ≤2MB |
| 3 | Description | Grilled chicken patty with cheese & tomato sauce, served with chips. / Bánh gà nướng với phô mai & sốt cà chua, ăn kèm khoai tây chiên. |
| 4 | Category | Burgers & Chicken Mains – Burger & Món Gà |
| 5 | Price | 170.000₫ |
| 6 | Option groups | none |
| 7 | Availability schedule | All opening hours |

### Step 8 — ⚠️ Item: Chicken Schnitzel — PENDING INGREDIENT CONFIRMATION
Priced, but chicken breast unresolved (SOT §3). Confirm before going live.
| # | Field | Value |
|---|---|---|
| 1 | Item name | Chicken Schnitzel – Gà Tẩm Bột Chiên Xù |
| 2 | Item photo | 800×800px, ≤2MB |
| 3 | Description | pending |
| 4 | Category | Burgers & Chicken Mains – Burger & Món Gà |
| 5 | Price | 99.000₫ |
| 6 | Option groups | none |
| 7 | Availability schedule | All opening hours |

### Step 9 — ⚠️ Item: Fish & Chips — PENDING INGREDIENT CONFIRMATION
Priced, but fish fillet unresolved (SOT §3). Confirm before going live.
| # | Field | Value |
|---|---|---|
| 1 | Item name | Fish & Chips – Cá & Khoai Tây Chiên |
| 2 | Item photo | 800×800px, ≤2MB |
| 3 | Description | pending |
| 4 | Category | Burgers & Chicken Mains – Burger & Món Gà |
| 5 | Price | 109.000₫ |
| 6 | Option groups | none |
| 7 | Availability schedule | All opening hours |

---

## Category 3: Salads & Finger Foods – Salad & Món Ăn Vặt

### Step 1 — Category
**Menu → Items tab.** A "Finger Food" category already exists → **rename it**:
| Field | Value |
|---|---|
| Category name | Salads & Finger Foods – Salad & Món Ăn Vặt |

### Items (no option groups)
Each: **+ Add item** · Photo 800×800 ≤2MB · Category = Salads & Finger Foods – Salad & Món Ăn Vặt · Availability = All opening hours.

| Item name | Description (EN / VN) | Price | Status |
|---|---|---|---|
| Garlic Bread – Bánh Mì Bơ Tỏi | Toasted garlic butter bread. / Bánh mì bơ tỏi nướng giòn. | 35.000₫ | Live |
| Hand-Cut Chips – Khoai Tây Chiên Cắt Tay | Hand-cut fries. / Khoai tây chiên cắt tay. | 35.000₫ | Live |
| Garden Salad – Salad Rau Củ | Fresh garden salad. / Salad rau củ tươi. | 49.000₫ | Live |
| Egg Salad – Trứng Salad | Garden salad with egg. / Salad rau củ với trứng. | 49.000₫ | Live |
| Shrimp Salad – Salad Tôm | Garden salad with shrimp. / Salad rau củ với tôm. | 69.000₫ | ⚠️ PENDING (shrimp) |
| Egg & Shrimp Salad – Trứng & Tôm Salad | Salad with egg & shrimp. / Salad với trứng và tôm. | 75.000₫ | ⚠️ PENDING (shrimp) |
| Popcorn Chicken – Gà Popcorn | Crispy popcorn chicken. / Gà popcorn giòn. | 45.000₫ | Live |
| Chicken Strips 6pc – Gà Strips 6 Miếng | 6 crispy chicken strips. / 6 miếng gà chiên giòn. | 59.000₫ | Live |
| Strips + Chips – Gà Strips & Khoai Tây | Chicken strips with chips. / Gà chiên giòn kèm khoai tây. | 79.000₫ | Live |
| Chicken Skewer – Gà Xiên | Grilled chicken skewer. / Xiên gà nướng. | 25.000₫ | Live |
| Skewer + BBQ – Gà Xiên Sốt BBQ | Chicken skewer with BBQ sauce. / Xiên gà kèm sốt BBQ. | 35.000₫ | Live |
| Veg Seafood Tofu – Đậu Hũ Hải Sản Chay | Vegetarian seafood tofu. / Đậu hũ hải sản chay. | 45.000₫ | Live |

---

## Category 4: Drinks & Desserts – Đồ Uống & Tráng Miệng

### Step 1 — Category
**Menu → Items tab.** Existing "Soft Drink" + "Healthy Fruit Juice" overlap → **merge into one**:
| Field | Value |
|---|---|
| Category name | Drinks & Desserts – Đồ Uống & Tráng Miệng |

(Move existing drink items into this category, then delete the empty old ones.)

### Items (no option groups)
Each: **+ Add item** · Photo 800×800 ≤2MB · Category = Drinks & Desserts – Đồ Uống & Tráng Miệng · Availability = All opening hours.

| Item name | Description (EN / VN) | Price | Status |
|---|---|---|---|
| Canned Drinks – Nước Ngọt Lon | Canned soft drink. / Nước ngọt lon. | 15.000₫ | Live |
| Iced Milk Coffee – Cà Phê Sữa Đá | Vietnamese iced milk coffee. / Cà phê sữa đá. | 29.000₫ | Live |
| Fruit Juice – Nước Ép Trái Cây | Fresh fruit juice. / Nước ép trái cây. | 35.000₫ | Live |
| Smoothies – Sinh Tố | Fruit smoothie. / Sinh tố trái cây. | 39.000₫ | Live |
| Coconut Cream Rice Balls – Bánh Trôi Nước Cốt Dừa | Rice balls (red bean/sesame) in coconut cream. / Bánh trôi nhân đậu đỏ/mè đen, sốt nước cốt dừa. | 29.000₫ | Live |
| Fresh Fruit Bowl – Trái Cây Tươi | Fresh cut fruit bowl. / Trái cây tươi cắt sẵn. | 55.000₫ | Live |
