# ✅ Product Inventory Dashboard — Build Checklist

---

## 1. Repo & Environment
- [ ] Initialize Next.js + Tailwind project  
- [ ] Add `.env` with `DATABASE_URL`  
- [ ] Add `.env.example`  
- [ ] Commit initial folder structure  

---

## 2. Database & Migrations
- [ ] Create `products` table  
- [ ] Create `categories` table  
- [ ] Add necessary indexes (search, FK, name)  
- [ ] Create `migrations/001_init.sql`  
- [ ] Add seed script with sample data  

---

## 3. Database Client
- [ ] Implement `/lib/db.ts` postgres singleton  
- [ ] Add test script to verify DB connection  

---

## 4. Base UI Shell
- [ ] Create layout with sidebar  
- [ ] Add Dashboard page  
- [ ] Add placeholder stats/cards  

---

## 5. Products Listing (GET Route)
- [ ] Create `/app/api/products/route.ts` (GET only)  
- [ ] Add pagination (`page`, `limit`)  
- [ ] Add search (`search`)  
- [ ] Add sorting (`sort`, `order`)  
- [ ] Build `/app/products/page.tsx` (RSC) using the GET endpoint  
- [ ] Create `ProductTable` to render rows  

---

## 6. Search, Pagination, Sorting UI
- [ ] Implement `SearchInput` component  
- [ ] Implement `Pagination` component  
- [ ] Add sort controls (price/date/name)  
- [ ] Wire components to URL searchParams  
- [ ] Confirm list updates correctly  

---

## 7. Product Form (Server Actions)
- [ ] Create `/app/products/actions.ts`  
- [ ] Implement `createProduct` server action  
- [ ] Implement `updateProduct` server action  
- [ ] Implement `deleteProduct` server action  
- [ ] Build `ProductForm` client component  
- [ ] Connect form to Server Actions  
- [ ] Add optimistic UI or loading states  

---

## 8. Validation & UX Polishing
- [ ] Create zod schemas in `/lib/validators.ts`  
- [ ] Server Actions return `{ success, error }`  
- [ ] Display inline errors in form  
- [ ] Disable submit button during requests  

---

## 9. Final Checks
- [ ] Test: create product  
- [ ] Test: edit product  
- [ ] Test: delete product  
- [ ] Test: search  
- [ ] Test: sort  
- [ ] Test: pagination  
- [ ] Review SQL safety (whitelist `ORDER BY`)  

---

## 10. Documentation
- [ ] Add README with setup instructions  
- [ ] Document migrations & seeding  
- [ ] Add notes on the project structure  

---

