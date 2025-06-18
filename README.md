# The Prompt2Game project
This repository aims to generate a fully playable and complex game from a single prompt, using multiple models such as LLMs and difusion models

# Goal of the project
The aim of the project is to generate a fully playable game by converting a single prompt into a full game representation for few-shots game creation
Every steps will be modifiable by user making a very flexible game creation engine

# Project status
- Prompt ▶ Game Design Document - ✅ In progress
- Game Design Document ▶ character list + game plot - ❌ Not done yet
- Game Character list / graphics ▶ Assets (3d or 2d generation) - ✅ In progress
- Game plot & Character list ▶ Game states (Menu - Cutscenes - Game - End screen) - ❌ Not done yet
- Game plot + Character list + states + details ▶ Game file structure (assets/scripts) - ❌ Not done yet
- Game file structure ▶ Full game with coding - ❌ Not done yet

# Prompt ▶ Game Design Document
From the game idea, generate the .json game design document.

**Input :** 
Title: Galactic Conquest
Prompt: In a distant future, where the universe is ruled by a vast galactic empire, players must lead a rebellion against the oppressive rule to restore freedom and justice. With a diverse crew of allies and strategic decision-making, players will navigate through epic space battles, explore uncharted territories, and forge alliances to ultimately overthrow the empire and usher in a new era of peace and prosperity.

**Output :**
```{

  "title": "Galactic Conquest",
  
  "genre": ["Action", "Strategy", "Adventure"], 
  
  "mechanics": ["Real-time strategy", "Exploration", "Diplomacy", "Combat"], 
  
  "aesthetics": "Sci-fi", 
  
  "platforms": ["PC", "Playstation", "Xbox", "Switch"], 
  
  "perspective": "Third-person", 
  
  "controls": {` 
  
    "keys": { 
    
      "W": "Move Forward", 
      
      "A": "Turn Left", 
      
      "S": "Move Backward", 
      
      "D": "Turn Right", 
      
      "Q": "Rotate Camera Left", 
      
      "E": "Rotate Camera Right", 

      "Space": "Jump", 
      
      "Mouse Click Left": "Shoot", 
      
      "Mouse Click Right": "Select/Use Item", 
      
      "Tab": "Switch Characters", 
      
      "P": "Pause" 
      
    } 
    
  }, 
  
  "goals": [ 
  
    "Defeat the galactic empire", 
    
    "Explore uncharted territories", 
    
    "Forge alliances", 
    
    "Restore freedom and justice" 
    
  ], 
  
  "plot_description": "In a distant future, the universe is ruled by a vast galactic empire. Lead a rebellion against the oppressive rule and navigate through epic space battles, explore uncharted territories, and forge alliances to overthrow the empire and usher in a new era of peace and prosperity."
}```

# Assets generation
## 3D generation
Useful repos and APIs : 
- Stable-Fast-3D : https://github.com/Stability-AI/stable-fast-3d
- Meshy.ai API
