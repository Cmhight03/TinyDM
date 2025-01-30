# TinyDM

A lightweight, chat-based Dungeon Master assistant that helps DMs create and manage D&D 5E sessions through natural conversation. TinyDM integrates with Live Agent Studio to provide creative content generation, rules assistance, and improvisational support.

## Features

- 🎲 Quick encounter generation
- 🎭 NPC creation and personality development
- 🏰 Dynamic location descriptions
- 📚 D&D 5E rules clarification
- ⚔️ Tactical combat suggestions
- 🌟 Creative story elements and plot hooks

## Setup Guide

1. **Prerequisites**
   - Python 3.11+
   - PowerShell (Windows)
   - Supabase account
   - Google Cloud account with Gemini API access

2. **Installation**
   ```powershell
   # Clone repository or download setup files
   # Run setup script as Administrator
   .\setup-tinyDM.ps1
   ```

3. **Configuration**
   Edit `.env` file with your credentials:
   ```env
   SUPABASE_URL=your-project.supabase.co
   SUPABASE_KEY=your-anon-key
   BEARER_TOKEN=your-bearer-token
   ```

4. **Starting the Server**
   ```powershell
   # Use the desktop shortcut or
   .\start-tinyDM.ps1
   ```

## User Guide

### Getting Started

TinyDM uses natural language processing to understand and respond to your needs. Simply describe what you want in conversational terms.

### Core Commands

1. **Encounter Generation**
   ```
   "Create an encounter for 4 level 3 players in a forest"
   "I need a random dungeon battle"
   "Generate a hard combat for level 5 players"
   ```

2. **Location Description**
   ```
   "Describe a bustling tavern"
   "Create a creepy dungeon entrance"
   "Help me design a wizard's tower"
   ```

3. **NPC Creation**
   ```
   "Create a mysterious merchant NPC"
   "Generate a town guard captain"
   "I need a villain for my campaign"
   ```

4. **Rules Help**
   ```
   "How does grappling work?"
   "Explain opportunity attacks"
   "What are the rules for darkness?"
   ```

### Sample Prompts

1. **Quick Combat Setup**
   ```
   User: "I need a quick forest encounter for 4 level 2 players"
   TinyDM: "Let me create a balanced forest encounter for your party...
   
   A pack of wolves has been stalking the party. You have:
   - 3 wolves (CR 1/4 each)
   - 1 dire wolf pack leader (CR 1)
   
   Tactical Setup:
   - Wolves approach from different directions
   - Pack leader waits to flank weak targets
   - Dense undergrowth provides partial cover
   
   Would you like the stat blocks or tactical suggestions?"
   ```

2. **Creative Location**
   ```
   User: "Describe a mysterious shrine in the woods"
   TinyDM: "Deep in the forest stands an ancient shrine, its stone walls wrapped in luminescent vines. 
   
   Key features:
   - Crumbling stone archway covered in unknown symbols
   - Small reflecting pool with crystal-clear water
   - Stone altar with mysterious offerings
   - Soft, ethereal humming in the air
   
   Would you like more details about the symbols, the offerings, or potential plot hooks?"
   ```

3. **Quick NPC**
   ```
   User: "Create a suspicious merchant"
   TinyDM: "Meet Darian Blacktrade:
   
   Physical: Well-dressed halfling with a silver-capped cane and nervous eyes
   Personality: Overly friendly but constantly glancing over his shoulder
   Hook: Claims to sell rare items at suspiciously low prices
   
   Would you like his inventory, mannerisms, or potential plot hooks?"
   ```

## Live Agent Studio Submission Information

**Your Name**: Michael Hightower
**Your Email**: mhightower@successequip.com

**Agent Name**: TinyDM

**Agent Description**: 
TinyDM is a lightweight, chat-based Dungeon Master assistant that helps DMs create and manage D&D 5E sessions. It provides instant access to creative content generation, rules clarification, and improvisational support through natural conversation. Perfect for both new and experienced DMs who need quick, creative assistance during game sessions.

**Agent Code/Workflow**:
- FastAPI backend (main.py)
- Supabase database
- Google Gemini for LLM capabilities
- Open5e API integration

All code is provided in the GitHub repository, including:
- Setup scripts
- SQL initialization
- Configuration templates
- Documentation

**Handling Extra Data**:
TinyDM provides all information in chat-friendly format, with optional data structure for enhanced display:

```json
{
  "type": "ai",
  "content": "Human-readable response",
  "data": {
    "responseType": "encounter|narrative|rules",
    "details": {},
    "textFallback": "Formatted text version"
  }
}
```

**Credit URL**: https://www.dumbdumbdice.com/dumb-dumbs-dragons

## Contributing

Contributions are welcome! Please check our contribution guidelines in the repository.

## License

MIT License - Feel free to use and modify for your needs.

## Support

For issues or questions:
1. Check the GitHub repository issues
2. Contact mhightower@successequip.com
