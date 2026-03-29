# 🎨 Issue-Ink  
## 🌍 The Global Rorschach Canvas

A collaborative pixel canvas powered entirely by **GitHub Issues + GitHub Actions**.

No backend.  
No database.  
Just commits.

---

## 🖼 Live Canvas

![Canvas](map.svg?ts=0)

---

## ✍️ Paint a Pixel

Anyone can contribute.

1. Go to the **Issues** tab  
2. Click **New Issue**  
3. Use this exact format as the **title**:

```
Paint [A5] #FF5733
```

Submit — and your pixel is painted automatically.

---

## ⚡ What Happens Next?

When you open an issue:

1. The title is parsed  
2. A GitHub Action validates your input  
3. The SVG canvas (`map.svg`) is updated  
4. Game state is stored in `data/state.json`  
5. Changes are committed  
6. The canvas refreshes in this README  

Everything happens in public.

---

## 📏 Canvas Coordinates

- Rows: **A–H**  
- Columns: **1–8**

Examples:

- `Paint [A1] #FF0000`  
- `Paint [H8] #00FFAA`  

---

## ⏳ Rules

- 🕒 **One paint per user every 24 hours**
- 🔒 **Each tile is locked for 1 hour after being painted**
- Format must match exactly:
  `Paint [Coordinate] #HEXCODE`
- Only valid **6-digit HEX colors** allowed
- Invalid input → Issue labeled `Invalid`
- Successful paint → Issue labeled `Completed`

---

## 🧠 What Is This?

This is not just a canvas.

It’s a shared system where:

- Anyone can overwrite anything  
- No one has permanent control  
- Patterns emerge through conflict and cooperation  

Over time, the grid becomes:

- A drawing  
- A battleground  
- A record of behavior  

It’s not about the pixels.

It’s about what people do with them.

---

## ⚙️ How It Works

The entire system runs inside this repository:

```
Issue → GitHub Action → SVG Update → Commit → README
```

### Components

- `map.svg` → visual canvas  
- `data/state.json` → persistent game state  
- GitHub Actions → logic engine  
- Git history → permanent ledger  

No external services are used.

---

## 📊 State Transparency

All game data is publicly stored:

- Last paint per user  
- Tile locks  
- Paint history  

See: `data/state.json`

---

## 🚫 What This Is Not

- Not a web app  
- Not a real-time game  
- Not centrally controlled  

This is a **slow system by design**.

---

## 🤝 Contributing

Want to improve the system?

See [`CONTRIBUTING.md`](CONTRIBUTING.md)

---

## 🧩 Core Principle

> Input → Mutation → Public Record

That’s the entire engine.

---

Built entirely with GitHub.  
Minimal by design.
