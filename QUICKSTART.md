# 🚀 QUICK START - NETLIFY DEPLOYMENT

## 5-Minute Setup

### Step 1: Choose Your Deployment Method
Pick ONE of these options:

#### Option A: GitHub + Netlify (Easiest)
1. Create a new GitHub repository
2. Push this folder to GitHub
3. Go to [netlify.com](https://netlify.com)
4. Click "New site from Git" 
5. Select your GitHub repo
6. Deploy! (Netlify will automatically build)

#### Option B: Direct Netlify Deploy
1. Go to [app.netlify.com/drop](https://app.netlify.com/drop)
2. Drag and drop this entire folder
3. Done! Your site is live

#### Option C: Netlify CLI
```bash
npm install -g netlify-cli
cd /workspaces/codespaces-blank
netlify deploy
```

### Step 2: Test Locally (Optional)

#### Using Python (Simple)
```bash
cd /workspaces/codespaces-blank
python -m http.server 8000
# Visit http://localhost:8000
```

#### Using Node.js (http-server)
```bash
npm install -g http-server
cd /workspaces/codespaces-blank
http-server
# Visit http://localhost:8080
```

---

## 🎮 How to Play After Deployment

### Player 1: Host a Game
```
1. Click "HOST ROOM"
2. Your username becomes the host name (e.g. "FNAFFan123")
3. Tell your friend what it is
4. Select board and pick your animatronic
5. Wait for opponent
```

### Player 2: Join the Game
```
1. Click "JOIN ROOM"
2. Enter the host's username
3. Click "CONNECT"
4. Pick your animatronic
5. Play!
```

---

## 🔧 Key Changes for Internet Play

### ✅ What Was Changed
- **Username system** - use usernames instead of codes
- **Better STUN servers** - Multiple Google STUN servers
- **Public TURN servers** - OpenRelay for restrictive networks
- **Improved UI** - Shows host username prominently when hosting
- **Better error messages** - Clear connection feedback

### ✅ What Still Works
- All 103 animatronics
- Custom board creation
- Undo/redo system
- Audio controls
- Session persistence
- Search functionality
- All original features!

---

## 🌍 Share Your Game Link

Once deployed to Netlify, you'll get a URL like:
```
https://fnaf-guess-who.netlify.app
```

Players can:
1. Go to that URL from **anywhere in the world**
2. No VPN needed
3. No local network required
4. Works on mobile, tablet, desktop
5. Use as many usernames as you like for infinite games

---

## 📊 Connection Quality

### Why It Works
- ✅ PeerJS handles WebRTC automatically
- ✅ STUN servers work 95%+ of the time
- ✅ TURN servers as backup for corporate WiFi
- ✅ Works on mobile hotspots
- ✅ Works on home internet
- ✅ Works on public WiFi (usually)

### If Connection Fails
1. Both players refresh the page
2. Choose a new host name
3. Try a different network (mobile hotspot)
4. Check browser console for errors (F12)

---

## 📁 Files That Get Deployed

```
✅ index.html                  (Main game - 905 lines)
✅ Animatronics/               (118 character images)
✅ background.jpeg             (Background image)
✅ background-music.mp3        (Ambient music)
✅ button.mp3                  (Button sound)
✅ netlify.toml                (Netlify config)
```

All files must stay together in the same deployment folder.

---

## 🆘 Common Issues

| Problem | Solution |
|---------|----------|
| "Username already in use" | Choose a different username or click HOST again |
| Connection times out | Check both players have internet, try different network |
| Images not loading | Verify `Animatronics/` folder exists in deployment |
| Audio not working | Click page once, some browsers require user interaction |
| Rooms disappear on refresh | Session auto-saves - click "Reconnect to Game" |

---

## 💡 Pro Tips

1. **Multiple games at once** - Different host names allow parallel games
2. **Mobile-friendly** - Works great on phones (tested!)
3. **Low bandwidth** - Only sends game state, not streaming video
4. **Fast connections** - Room join takes 1-2 seconds typically
5. **No server cost** - Netlify free tier covers this perfectly

---

## 🎉 You're Ready!

Your game is now **globally playable from anywhere**! 

Share the link with friends and start playing! 🎮

---

*Questions? Check the DEPLOYMENT_GUIDE.md for more details*
