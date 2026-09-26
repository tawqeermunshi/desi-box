# DesiBox

DesiBox runs a home kitchen's business so the cook can cook. It was built at a Kellogg hackathon (September 2026) for Manna's Kitchen, a tiffin service that serves Kellogg students.

**Live demo:** https://tawqeermunshi.github.io/desi-box/

## What it does

**For students**
- See the whole week's menu (veg and non-veg platters, Monday to Friday)
- Pick a main, rice or chapati, extras, or swap starters with the other platter
- Pay upfront and track each order from Cooking to Delivered

**For the kitchen**
- Orders dashboard with payment status and one-tap batch updates
- Prep list: exact totals of mains, chapatis, rice and starters for each day
- AI weekly menu planner: drafts next week's menu from what sells and what it costs
- Inventory autopilot: turns orders into ingredients and drafts the weekly grocery order under a spending cap
- Off-menu items for selling extra dishes

Use the **Student / Kitchen** switch at the top right to move between the two sides.

## About this demo

- One self-contained `index.html`, no build step.
- Data lives in a shared Supabase (Postgres) database, so orders, menus and stock persist and sync live across devices. On first load the database is filled with sample data.
- The demo database is open: anyone with the link can read and change it. Don't enter real personal details.
- All menus, orders, dish performance, costs and stock levels are sample data.
- Payments and supplier orders are simulated. No money moves.
- In this GitHub version, the menu planner uses built-in rules. The Claude-powered planner and the shared live database run in the Claude-hosted version.
