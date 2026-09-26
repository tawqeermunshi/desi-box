# DesiBox

DesiBox runs a home kitchen's business so the cook can cook. It was built at a Kellogg hackathon (September 2026) for Manna's Kitchen, a tiffin service that serves Kellogg students.

**Live demo:** https://tawqeermunshi.github.io/desi-box/

## What it does

**For students**
- See the whole week's menu (veg and non-veg platters, Monday to Friday)
- Pick a main, rice or chapati, extras, or swap starters with the other platter
- Pay upfront and track each order from Cooking to Delivered
- See estimated nutrition (calories, protein, carbs, fat, fiber) and allergens for every dish, and filter for high-protein or lighter meals
- Rate each dish after delivery, with tags and a comment

**For the kitchen**
- Orders dashboard with payment status and one-tap batch updates
- Prep list: exact totals of mains, chapatis, rice and starters for each day
- Weekly menu planner: drafts next week's menu from what sells and what it costs
- Inventory autopilot: turns orders into ingredients and drafts the weekly grocery order under a spending cap
- Off-menu items for selling extra dishes
- Feedback: ratings by dish, most common complaints, and recent reviews. Ratings feed the demand forecast and the menu planner.
- Nutrition figures are estimates computed from each dish's recipe

Use the **Student / Kitchen** switch at the top right to move between the two sides.

## About this demo

- One self-contained `index.html`, no build step.
- Data lives in a shared Supabase (Postgres) database, so orders, menus and stock persist and sync live across devices. On first load the database is filled with sample data.
- The demo database is open: anyone with the link can read and change it. Don't enter real personal details.
- All menus, orders, dish performance, costs and stock levels are sample data.
- Payments and supplier orders are simulated. No money moves.
- In this GitHub version, the menu planner uses Quick draft (built-in rules). Full drafting runs in the Claude-hosted version.
