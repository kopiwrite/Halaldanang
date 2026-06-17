# STORE_SETUP — Halal Da Nang GrabFood Portal Playbook

> Field-by-field GrabMerchant data-entry guide. Menu/pricing source of truth = `SOT.md`.
> App: GrabMerchant (iPad). Nav: bottom **Menu** → top tabs **Items** / **Option Groups**.
> Image spec: 800×800px, JPEG/PNG, **≤2MB each (up to 4 photos)**. Prices shown are the *add-on* amount.
> Item form field order: Item name → Item photo → Description → Category → Price → Option groups → Availability schedule.
> ⚠️ = phantom-ingredient item, pending source-or-swap decision (SOT §3) — do not enter live.
> NOTE: SOT §4 still says 6MB; live app form says 2MB each — orchestrator to correct SOT.

Status: Categories 1–2 drafted · Categories 3–4 pending.

---

## Category 1: Custom Noodle Bar

Do the steps in order.

### Step 1 — Create the Category
**Menu → Items tab → + Add category**

| Field | Value |
|---|---|
| Category name | Tự Làm Mì Trộn Cay (Custom Noodle Bar) |

(Existing categories are Healthy Fruit Juice / Soft Drink / Finger Food — this adds a new one, no duplicate.)

### Step 2 — Fix & fill the Base option group (reuse existing)
**Menu → Option Groups tab → open "Chọn Cấp Độ Cay (Choose Your Noodle Base)"** (0 items linked)

1. Rename to remove the VN/EN mismatch → **Name:** Chọn Loại Mì · **Edit translations → EN:** Pick Your Noodle
2. **+ Add an option** for each (Name + Price):

| Option name | Price |
|---|---|
| Mi Sedaap Korean Spicy Chicken | 0₫ |
| Samyang Quattro Cheese | 6.000₫ |
| Samyang Habanero Lime | 6.000₫ |
| Samyang 2x Spicy | 8.000₫ |

3. Toggles: **Make mandatory = ON**, **Allow multiple selections = OFF** → **Save**

### Step 3 — Create the Toppings option group (new, dedicated)
**Menu → Option Groups tab → + Add an option group → "Toppings" template** (or New)

1. **Name:** Thêm Topping · **Edit translations → EN:** Add Toppings
2. **+ Add an option** for each:

| Option name | Price | Status |
|---|---|---|
| Trứng Luộc (Boiled Egg) | 10.000₫ | Live |
| Đậu Hũ (Tofu) | 15.000₫ | Live |
| Gà Popcorn (K&U Popcorn Chicken) | 18.000₫ | Live |
| Gà Miếng (99Poultry Strips) | 18.000₫ | Live |
| Gà Xiên (99Poultry Skewer) | 22.000₫ | Live |
| ⚠️ Tôm Chiên (Fried Shrimp) | 25.000₫ | PENDING — don't add until shrimp sourcing resolved (SOT §3) |

3. Toggles: **Make mandatory = OFF**, **Allow multiple selections = ON** → **Save**

(Don't reuse the generic "Thêm vị món ăn càng ngon" group — it's shared by 4 other items and its prices differ from SOT.)

### Step 4 — Create the Item
**Menu → Items tab → + Add item** (fields in app order):

| # | Field | Value |
|---|---|---|
| 1 | Item name | Tự Làm Mì Trộn Cay (Custom Noodle Bowl) |
| 2 | Item photo | 800×800px, ≤2MB (from Image Studio) |
| 3 | Description | Bát mì trộn cay tự chọn — chọn loại mì, thêm topping tuỳ thích. (Build-your-own spicy mixed-noodle bowl — pick your noodle, stack your toppings.) |
| 4 | Category | Tự Làm Mì Trộn Cay (Custom Noodle Bar) |
| 5 | Price | 35.000₫ |
| 6 | Option groups | Link **Pick Your Noodle** + **Add Toppings** |
| 7 | Availability schedule | All opening hours |

Then **Save**.

---

## Category 2: Burgers & Chicken Mains

Do the steps in order.

### Step 1 — Create the Category
**Menu → Items tab → + Add category**

| Field | Value |
|---|---|
| Category name | Burger & Món Gà (Burgers & Chicken Mains) |

### Step 2 — Create the Sauce option group (for Bánh Gà)
**Menu → Option Groups tab → + Add an option group → New**

1. **Name:** Chọn Sốt · **Edit translations → EN:** Choose Your Sauce
2. **+ Add an option** for each:

| Option name | Price | Note |
|---|---|---|
| Sốt Cà & Mayo (Tomato & Mayo) | 0₫ | list first = default |
| Sốt Ớt (Chilli) | 0₫ | |

3. Toggles: **Make mandatory = ON**, **Allow multiple selections = OFF** → **Save**

### Step 3 — Create Item: Bánh Gà Sốt Tự Chọn
**Menu → Items tab → + Add item** (fields in app order):

| # | Field | Value |
|---|---|---|
| 1 | Item name | Bánh Gà Sốt Tự Chọn (Chicken Patty, Choice of Sauce) |
| 2 | Item photo | 800×800px, ≤2MB (from Image Studio) |
| 3 | Description | Bánh gà giòn, chọn sốt tuỳ thích. (Crispy chicken patty, choice of sauce.) |
| 4 | Category | Burger & Món Gà |
| 5 | Price | 39.000₫ |
| 6 | Option groups | Link **Choose Your Sauce** |
| 7 | Availability schedule | All opening hours |

Then **Save**.

### Step 4 — Create Item: Burger Gà & Khoai Tây
| # | Field | Value |
|---|---|---|
| 1 | Item name | Burger Gà & Khoai Tây (Chicken Burger + Chips) |
| 2 | Item photo | 800×800px, ≤2MB (from Image Studio) |
| 3 | Description | Burger gà ăn kèm khoai tây chiên. (Chicken burger served with chips.) |
| 4 | Category | Burger & Món Gà |
| 5 | Price | 59.000₫ |
| 6 | Option groups | none |
| 7 | Availability schedule | All opening hours |

Then **Save**.

### Step 5 — Create Item: Big Hamburger Cheese
| # | Field | Value |
|---|---|---|
| 1 | Item name | Big Hamburger Cheese (Burger Bò Phô Mai Lớn) |
| 2 | Item photo | 800×800px, ≤2MB (from Image Studio) |
| 3 | Description | Burger bò phô mai cỡ lớn. (Big beef cheeseburger.) |
| 4 | Category | Burger & Món Gà |
| 5 | Price | 69.000₫ |
| 6 | Option groups | none |
| 7 | Availability schedule | All opening hours |

Then **Save**.

### Step 6 — Create Item: Big Hamburger Egg
| # | Field | Value |
|---|---|---|
| 1 | Item name | Big Hamburger Egg (Burger Bò Trứng Lớn) |
| 2 | Item photo | 800×800px, ≤2MB (from Image Studio) |
| 3 | Description | Burger bò trứng cỡ lớn. (Big beef burger with egg.) |
| 4 | Category | Burger & Món Gà |
| 5 | Price | 75.000₫ |
| 6 | Option groups | none |
| 7 | Availability schedule | All opening hours |

Then **Save**.

### Step 7 — Create Item: Big Double Hamburger Cheese
| # | Field | Value |
|---|---|---|
| 1 | Item name | Big Double Hamburger Cheese (Burger Bò Đôi Phô Mai Lớn) |
| 2 | Item photo | 800×800px, ≤2MB (from Image Studio) |
| 3 | Description | Burger bò đôi phô mai cỡ lớn. (Big double beef cheeseburger.) |
| 4 | Category | Burger & Món Gà |
| 5 | Price | 95.000₫ |
| 6 | Option groups | none |
| 7 | Availability schedule | All opening hours |

Then **Save**.

### Step 8 — ⚠️ Item: Chicken Schnitzel — PENDING (do not enter live)
Blocked: chicken breast unresolved (SOT §3, source-or-swap). Enter only after orchestrator confirms.

| # | Field | Value |
|---|---|---|
| 1 | Item name | Chicken Schnitzel (Gà Tẩm Bột Chiên Xù) |
| 2 | Item photo | pending |
| 3 | Description | pending |
| 4 | Category | Burger & Món Gà |
| 5 | Price | 79.000₫ |
| 6 | Option groups | TBD |
| 7 | Availability schedule | All opening hours |

### Step 9 — ⚠️ Item: Fish & Chips — PENDING (do not enter live)
Blocked: fish fillet unresolved (SOT §3, source-or-rebrand). Enter only after orchestrator confirms.

| # | Field | Value |
|---|---|---|
| 1 | Item name | Fish & Chips (Cá & Khoai Tây Chiên) |
| 2 | Item photo | pending |
| 3 | Description | pending |
| 4 | Category | Burger & Món Gà |
| 5 | Price | 85.000₫ |
| 6 | Option groups | TBD |
| 7 | Availability schedule | All opening hours |
