# Pong Game - Online Multiplayer 🎮🏓

A feature-rich Pong game with **Single Player (AI)**, **Local Multiplayer (2 Players)**, and **Online Multiplayer** modes!

## 🎮 Features

### Game Modes
- **Single Player**: Challenge an AI opponent with difficulty levels
- **Local Multiplayer**: Play against a friend on the same keyboard
- **Online Multiplayer**: Play with friends online in real-time

### Gameplay Features
✅ Ball physics with bounce and spin effects
✅ Advanced collision detection (walls & paddles)
✅ Real-time scoreboard
✅ Start/Pause functionality
✅ Reset score button
✅ Responsive design
✅ Modern neon theme

## 🚀 Quick Start

### Single & Local Multiplayer (No Backend Required)
Simply open `index.html` in your browser and start playing!

### Online Multiplayer (Requires Backend Server)

#### Prerequisites
- Node.js (v14 or higher)
- npm

#### Setup Instructions

1. **Clone the repository**
```bash
git clone https://github.com/anshulraj1458/pong-game.git
cd pong-game
```

2. **Install backend dependencies**
```bash
npm install
```

3. **Start the backend server**
```bash
npm start
```
The server will run on `http://localhost:3000`

4. **Open the game**
Open `index.html` in your browser and select **"Online Multiplayer"** mode

5. **Share and Play**
- Create a room and share the room code with your friend
- Your friend joins with the same room code
- Click "Start Game" when both players are ready

## 🎮 Controls

### Single Player Mode
- **Mouse**: Move paddle vertically
- **Arrow Keys**: ↑/↓ to move paddle
- **W/S**: Alternative keyboard control

### Local Multiplayer Mode
- **Player 1 (Left)**: Arrow Keys (↑/↓) or W/S
- **Player 2 (Right)**: I/K keys or Mouse position

### Online Multiplayer Mode
- **Your Paddle**: Arrow Keys (↑/↓) or W/S
- **Opponent**: Controlled by your friend in real-time

## 📋 How to Play Online

1. **Create a Room**
   - Enter your name (optional)
   - Click "Create Room"
   - Share the room code with your friend

2. **Join a Room**
   - Enter your name (optional)
   - Enter the room code
   - Click "Join Room"

3. **Start Playing**
   - Both players click "Start Game"
   - Try to score by hitting the ball past your opponent!

## 🛠️ Technology Stack

### Frontend
- HTML5
- CSS3
- JavaScript (Vanilla)
- Socket.IO Client

### Backend
- Node.js
- Express.js
- Socket.IO
- CORS

## 📁 File Structure

```
pong-game/
├── index.html          # Main game UI
├── script.js           # Client-side game logic
├── styles.css          # Game styling
├── server.js           # Backend server (Node.js)
├── package.json        # Backend dependencies
└── README.md          # This file
```

## 🌐 Deployment

### Deploy to Cloud

#### Option 1: Heroku (Recommended)
```bash
heroku login
heroku create pong-game-online
git push heroku main
```

#### Option 2: Railway.app
1. Connect your GitHub repository
2. Set environment variable: `PORT=3000`
3. Deploy!

#### Option 3: Render
1. Connect your GitHub repository
2. Select Node.js environment
3. Build command: `npm install`
4. Start command: `npm start`

### Update Client Connection
In `script.js`, change the server URL:
```javascript
socket = io('https://your-deployed-url.com');
```

## 🎯 Game Rules

- Each player controls a paddle on their side
- The ball bounces off walls and paddles
- Score a point when the ball passes your opponent
- First to X points wins (configurable)
- Paddle spin affects ball trajectory

## 🐛 Troubleshooting

### "Failed to connect to server"
- Make sure backend server is running: `npm start`
- Check if port 3000 is not in use
- On Windows, you might need to allow the app through firewall

### "Opponent disconnected"
- The opponent's internet connection was lost
- Try creating a new room and re-inviting them

### Ball not syncing
- Check your internet connection
- Make sure both players are in the same room
- Reload the page and try again

## 📝 Future Enhancements

- [ ] Database for player rankings
- [ ] Chat system between players
- [ ] Difficulty levels selection
- [ ] Power-ups and special abilities
- [ ] Mobile app version
- [ ] Spectator mode
- [ ] Tournament support

## 📄 License

MIT License - Feel free to use and modify!

## 🤝 Contributing

Contributions are welcome! Feel free to:
1. Fork the repository
2. Create a feature branch
3. Submit a pull request

## 📧 Support

For issues or questions, please open an issue on GitHub!

---

**Enjoy the game! 🎉**
