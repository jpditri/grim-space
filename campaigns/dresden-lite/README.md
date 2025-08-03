campaign:: dresden-lite
type:: campaign-overview
setting:: Modern Boston-North Shore Massachusetts
theme:: Hidden supernatural world (Dresden Files inspired)
magic-level:: Hidden (magic must be concealed from public)
atmosphere:: Modern urban environment with supernatural secrets
tags:: #dresden-lite #urban-fantasy #boston #hidden-magic #modern-setting #masquerade

# Dresden Lite Campaign

Welcome to **Dresden Lite** - an urban fantasy campaign set in modern Boston-North Shore Massachusetts where magic hides in the shadows of the real world.

## Campaign Overview
- **Setting**: Modern Boston-North Shore Massachusetts  
- **Theme**: Hidden supernatural world (Dresden Files inspired)  
- **Magic Level**: Hidden (magic must be concealed from public)  
- **Atmosphere**: Modern urban environment with supernatural secrets

## Key Elements
- ### The Hidden World
	- **Magic Exists**: But must be kept secret from mundane population
	- **Supernatural Creatures**: Ghosts, goblins, and other creatures hide in plain sight
	- **Dragons**: Extremely rare, often take human form
	- **The Masquerade**: Authorities explain away supernatural events with conventional explanations
- ### Modern Setting Rules
	- **No Open Magic**: Magic performed in public causes panic and official investigation
	- **Firearms Mechanics**: D20 to hit, automatic weapons have disadvantage beyond 30ft unless trained
	- **Automatic Weapons**: Roll D4 for number of hits if attack succeeds
	- **Weapon Concealment**: Carrying weapons openly draws police attention
	- **Human Only**: Only human race allowed for this campaign
- ### Key Locations
	- **[[Wonderland Station Revere]]** - Public transit hub
	- **[[TD Garden]]** - Major sports and entertainment venue
	- **[[South Station]]** - Central transportation terminal
	- **[[China Town Boston]]** - Cultural district with hidden supernatural elements
	- **[[Essex Street Salem]]** - Historic witchcraft tourism area
	- **[[The Wharf Salem]]** - Waterfront district
	- **[[Old Town Marblehead]]** - Historic seaside community
	- **[[Marblehead Neck]]** - Affluent peninsula area
	- **[[Lynn Woods]]** - Large forest preserve (supernatural activity)
	- **[[Riptide Bar Marblehead]]** - Local gathering spot
	- **[[The Tavern on the Square Salem]]** - Popular restaurant/bar
	- **[[Peabody Essex Museum]]** - Art and culture museum
	- **[[YMCA Salem]]** - Community center

## Getting Started
- To activate this campaign:
	- ```bash
	  ruby -e "require_relative 'system-core/lib/campaign_management/campaign_config.rb'; Configuration::CampaignConfig.switch_campaign('dresden-lite')"
	  ```
- Then use campaign-aware commands:
	- ```bash
	  ./system-core/bin/computer --context content "Generate urban fantasy NPC"
	  ./system-core/bin/computer --context dresden-lite "Create Boston location"
	  ```

## Content Organization
- **NPCs**: `/pages/campaigns/dresden-lite/npcs/` - Urban dwellers, supernatural creatures
- **Locations**: `/pages/campaigns/dresden-lite/locations/` - Boston area locations, hidden supernatural sites
- **Factions**: `/pages/campaigns/dresden-lite/factions/` - Supernatural organizations, mundane groups
- **Items**: `/pages/campaigns/dresden-lite/items/` - Modern equipment, magical artifacts
- **Events**: `/pages/campaigns/dresden-lite/events/` - City incidents, supernatural occurrences
- **Mechanics**: `/pages/campaigns/dresden-lite/mechanics/` - Modern combat, hidden magic rules

## Campaign Tags
- Use these tags for content organization:
	- `#dresden-lite` - Campaign identifier
	- `#urban-fantasy` - Genre identifier
	- `#boston` - Geographic setting
	- `#hidden-magic` - Magic concealment theme
	- `#modern-setting` - Contemporary time period
	- `#masquerade` - Supernatural secrecy

---

*"In Boston, the old magic runs as deep as the harbor, but the new world demands it stay hidden."*