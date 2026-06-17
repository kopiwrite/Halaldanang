# STORE_SETUP — Halal Da Nang GrabFood Portal Playbook

> Field-by-field GrabMerchant data-entry guide. Menu/pricing source of truth = `SOT.md`.
> App: GrabMerchant (iPad). Nav: bottom **Menu** → top tabs **Items** / **Option Groups**.
> Image spec: 800×800px, JPEG/PNG, ≤6MB. Prices shown are the *add-on* amount.
> ⚠️ = phantom-ingredient item, pending source-or-swap decision (SOT §3) — do not enter live.

Status: Category 1 drafted · Categories 2–4 pending.

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
| 2 | Item photo | 800×800px, JPEG/PNG, ≤6MB (from Image Studio) |
| 3 | Description | Bát mì trộn cay tự chọn — chọn loại mì, thêm topping tuỳ thích. (Build-your-own spicy mixed-noodle bowl — pick your noodle, stack your toppings.) |
| 4 | Category | Tự Làm Mì Trộn Cay (Custom Noodle Bar) |
| 5 | Price | 35.000₫ |
| 6 | Option groups | Link **Pick Your Noodle** + **Add Toppings** |
| 7 | Availability schedule | All open hours |

Then **Save**.
