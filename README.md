# How to Edit the Hovlim Website

This guide will show you, in very easy steps, how to add or remove products from the Hovlim website.

You don’t need to know any programming — just follow along slowly ❤️

## Step 1 — Install the program that runs the website (Hugo)

If this computer is a Mac, open the Terminal (you can find it with Spotlight 🔍).
Then copy and paste this line and press Enter:

```bash
brew install hugo
```

When it’s done, Hugo is ready — that’s the program that shows you the website before it goes online.

## Step 2 — Where the products live

All the products on the website live in a folder called:

```
content/products
```

Each product has its own little file.
Think of it like one drawer per t-shirt.

Example:

```
deer.md
lion.md
tiger.md
```

Each file has the name of the product, like deer, lion, or tiger.

## Step 3 — To remove a product

If you don’t want a product anymore:
	1.	Go into the folder `content/products`.
	2.	Find the file for that product, for example `lion.md`.
	3.	Delete that file.
	4.	The next time you open the site, the lion will be gone 🦁❌.

⸻

💚 Step 4 — To add a new product
	1.	Go into the folder `content/products`.
	2.	Make a copy of one of the existing product files (for example, deer.md).
	3.	Rename it — maybe `new-shirt.md`.
	4.	Open it (you can open it with any text editor, like TextEdit, VS Code, or Notepad).

Inside, you’ll see a block of text that looks like this:

```yaml
---
title: Deer
name: Sacha the Deer
description_markdown: >-
  A soft and elegant shirt with our favorite deer design.
price: '9.00'
sku: deer
stock: 10
sizes:
  - Small
  - Medium
  - Large
styles:
  - name: Black
    color: '#000000'
    image: /images/products/deer/black.jpg
  - name: Blue
    color: '#39589e'
    image: /images/products/deer/blue.jpg
---
```

Now change the details for your new item:
	•	title → a short name (example: T-Shirt)
	•	name → full name that shows on the website
	•	description_markdown → describe your product
	•	price → write the price (use quotes: '19.00')
	•	sizes → list available sizes (Small, Medium, Large, etc.)
	•	styles → here you can list the colors and pictures

That’s it!
Save the file.

## Step 5 — Add the pictures

Pictures go in this folder:

```
static/images/products/
```

Inside, make a folder with your product name.

**Example:**

```
static/images/products/new-shirt/
```

Put your pictures inside there, like:

```
black.jpg
blue.jpg
green.jpg
```

Then in the product file, make sure the picture names match what you called them.

**Example:**
```
  - name: Blue
    color: '#39589e'
    image: /images/products/new-shirt/blue.jpg
```

## Step 6 — Check how it looks

**To see the site on your own computer:**

1. Open Terminal again.
2. Go to the website folder.
3. Type:
	```
	hugo server
	```
4. Open your web browser and go to `http://localhost:1313`.￼

You’ll see your website with the new product!

## Step 7 — Put it online

When you’re happy with how it looks, send (push) the changes to GitHub (you can ask someone to help with that part).

After a minute or two, the site updates automatically at `https://hovlim.github.io/`.

### You did it!

>[!NOTE]
> Adding products = copying and editing one small file.
> Removing products = deleting that file.
> That’s all. 🌞

