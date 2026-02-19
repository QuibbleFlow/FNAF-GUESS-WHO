# FNAF Guess Who - Multiplayer Online Edition

A peer-to-peer multiplayer "Guess Who?" game themed around Five Nights at Freddy's. Play online with friends from anywhere in the world - no VPN or local network required!

## 🎮 How to Play Online

### Host a Room
1. Enter your username and click "Enter Terminal"
2. Click **"HOST ROOM"**
3. A 6-character **room code** will be generated and displayed
4. Share this code with your friend (Discord, email, etc.)
5. Select the animatronics board you want to play with
6. Pick your secret animatronic
7. Wait for your opponent to join and make their choice

### Join a Room
1. Enter your username and click "Enter Terminal"
2. Click **"JOIN ROOM"**
3. Enter the room code your friend shared
4. Click **"CONNECT"**
5. Select your secret animatronic
6. Try to guess your opponent's choice!

## 🚀 Deploy to Netlify

### Option 1: Deploy via GitHub (Recommended)
1. Push this repository to GitHub
2. Go to [netlify.com](https://netlify.com) and sign in
3. Click "Add new site" → "Import an existing project"
4. Connect your GitHub account and select this repository
5. Click "Deploy"
6. Your site will be live at `https://[your-site-name].netlify.app`
7. Share the link with friends!

### Option 2: Deploy via Drag & Drop
1. Go to [netlify.com](https://netlify.com) and sign in
2. Drag and drop this entire folder into the Netlify deploy zone
3. Your site will be live immediately!

### Option 3: Deploy via Netlify CLI
```bash
npm install -g netlify-cli
netlify deploy
```

## 🔧 Technical Details

### Why It Works Without VPN
- Uses **PeerJS** for WebRTC peer-to-peer connections
- Includes multiple public **STUN servers** for NAT traversal
- Includes public **TURN servers** for restrictive firewalls
- Works on any internet connection (home, mobile, public WiFi)

### Improvements Made
✅ Room code system (easier than sharing usernames)
✅ Enhanced STUN/TURN server configuration
✅ Better error handling for connection issues
✅ Works globally without local network requirements
✅ All assets (images, audio) bundled for deployment

## 📁 File Structure
```
├── index.html              (Main game file)
├── FNAF GUESS WHO.html     (backup of original name) 
├── Animatronics/            (118 character images)
├── background.jpeg
├── background-music.mp3
├── button.mp3
└── netlify.toml             (Deployment config)
```

## 🎮 Features
- **103 FNAF Animatronics** across 9 game categories
- **Custom Boards** - create your own character selections
- **Undo/Redo System** - fix your mistakes
- **Audio Controls** - volume slider for music
- **Session Persistence** - reconnect if connection drops
- **Search & Filter** - find characters quickly
- **Drag-to-Select** - bulk toggle characters in board editor

## ⚠️ Requirements
- Modern web browser (Chrome, Firefox, Safari, Edge)
- Stable internet connection
- Two players (obviously!)

## 🐛 Troubleshooting

### "Connection Failed"
- Verify the room code is spelled correctly (case doesn't matter)
- Check both players have internet connection
- Some corporate networks may block WebRTC - try mobile hotspot

### "Room Code Already in Use"
- Room codes can conflict rarely - just generate a new one

### Audio Not Playing
- Check browser audio permissions
- Some browsers require user interaction before playing audio
- Try clicking the page first

### Images Not Loading
- All images should be in `/Animatronics/` folder
- Check browser console for detailed errors

## 🎵 Audio Assets
- `background-music.mp3` - Background ambience
- `button.mp3` - Button click sound

To change these, replace the files and update the `<audio>` tags in the HTML.

## 🚀 Performance Tips
- Disable background music if experiencing lag
- Reduce browser zoom to 80% for better UI
- Close other browser tabs to free up resources
- Use 2.4GHz WiFi if on wireless (more stable than 5GHz)

## 📝 License
Feel free to modify and share!

---

**Made with ❤️ for FNAF fans** - Now playable anywhere, anytime! 🎮
