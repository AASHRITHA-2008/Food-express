# FoodExpress – Online Food Ordering (React + Vite)

Converted from the original HTML/CSS/JS project to **React + Vite**. All data is stored in the browser's **Local Storage** (no backend).

## Modules
| Module | Routes | What it does |
|---|---|---|
| Public | `/`, `/login`, `/signup` | Landing page, user login & signup |
| **User** | `/user/home` `menu` `cart` `checkout` `orders` `track-order` `profile` | Browse/filter menu, cart, checkout, order history, live tracking, profile |
| **Admin** | `/admin/login`, `/admin/dashboard` `manage-food` `manage-orders` `manage-users` | Stats dashboard, food CRUD, update order status, manage users |

## Demo credentials
- User: `user@example.com` / `password123` (or sign up a new account)
- Admin: `admin` / `admin123`

## Run locally
```bash
npm install
npm run dev
```

## Deploy on Vercel
1. Push this folder to a GitHub repository.
2. On vercel.com → **Add New → Project** → import the repo.
3. Framework preset: **Vite** (build command `npm run build`, output `dist`).
4. Deploy. `vercel.json` already rewrites all routes to `index.html` so page refreshes work.

## Project structure
```
src/
  main.jsx, App.jsx          entry + routes
  context/AppContext.jsx     auth, cart, orders, toasts (localStorage)
  utils/                     storage helpers, seed data
  components/                navbars, layouts, ProtectedRoute, FoodCard
  pages/                     Landing, Login, Signup
  pages/user/                user module
  pages/admin/               admin module
  styles/                    original CSS (unchanged)
```
"# Food-express" 
