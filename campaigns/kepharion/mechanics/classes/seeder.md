---
name: "Seeder"
type: "class"
hit_die: 8
primary_ability: ["Intelligence", "Wisdom"]
saving_throw_proficiencies: ["Intelligence", "Wisdom"]
skill_proficiencies: 4
armor_proficiencies: ["Light armor", "Medium armor"]
weapon_proficiencies: ["Simple weapons", "Martial weapons (finesse only)"]
xenocortex_class: true
campaign: "kepharion"
source: "Kepharion Campaign"
last_updated: "2025-07-02T16:15:00Z"
---

# Seeder

**Hit Die:** d8 per seeder level  
**Primary Abilities:** Intelligence and Wisdom  
**Saving Throw Proficiencies:** Intelligence, Wisdom  
**Xenocortex Specialization:** Adaptive Pattern Storage

Seeders are the pioneers and catalysts of Vaarn society, those who blaze new trails, nurture growth, and ensure continuity. They excel at adaptation, problem-solving, and environmental mastery through specialized xenocortex programming.

## Class Features

### 1st Level

#### Hit Points
- **Hit Points at 1st Level:** 8 + Constitution modifier
- **Hit Points at Higher Levels:** 1d8 (or 5) + Constitution modifier per seeder level after 1st

#### Proficiencies
- **Armor:** Light armor, medium armor
- **Weapons:** Simple weapons, finesse martial weapons
- **Tools:** Herbalism kit, one type of artisan's tools
- **Saving Throws:** Intelligence, Wisdom

#### Skills
Choose 4 from: Animal Handling, Athletics, History, Insight, Investigation, Medicine, Nature, Perception, Survival

#### Adaptive Xenocortex
Your xenocortex is specialized for environmental adaptation and problem-solving:
- **Xenocortex Rating increases by 1** at 1st level and again at 5th, 9th, 13th, and 17th levels
- **Environmental Patterns:** You can store adaptation patterns for specific environments
- **Problem-Solving Matrix:** Advantage on Intelligence checks to solve complex problems or puzzles

#### Pioneer's Instinct
You can sense environmental dangers and opportunities:
- **Danger Sense:** Advantage on Wisdom (Perception) checks to detect environmental hazards
- **Opportunity Recognition:** Once per long rest, you can reroll any Intelligence or Wisdom-based skill check

### 2nd Level

#### Growth Catalyst
You can accelerate natural processes through xenocortex-guided intervention:
- **Accelerated Growth:** Touch a plant to make it grow as if 1 week had passed (once per long rest)
- **Rapid Healing:** When you take a long rest in natural environments, regain maximum hit points
- **Seed of Change:** Can create minor beneficial environmental changes (purify water, enrich soil, etc.)

### 3rd Level

#### Seeder Path
Choose your specialization path that shapes your xenocortex development:

##### Path of the Explorer
- **Terrain Mastery:** Choose two terrain types; gain expertise in Survival checks in those terrains
- **Pathfinding:** Always know which direction is north and can navigate by xenocortex pattern recognition
- **Xenocortex Expansion:** +1 additional pattern storage slot

##### Path of the Cultivator  
- **Life Sense:** Can detect living creatures within 60 feet through xenocortex bio-pattern recognition
- **Growth Acceleration:** Your Growth Catalyst ability recharges on short rest
- **Symbiotic Link:** Can form temporary mental bonds with animals or plants

##### Path of the Inventor
- **Technical Integration:** Proficiency with all artisan's tools
- **Innovation Pattern:** Can combine two stored patterns for enhanced effects
- **Adaptive Construction:** Can jury-rig equipment repairs using Intelligence + xenocortex rating

### 4th Level

#### Ability Score Improvement
You can increase one ability score by 2, or two ability scores by 1. You can also choose a feat.

#### Pattern Optimization
Your xenocortex becomes more efficient:
- **Pattern Overlap:** Can store patterns that work in multiple situations
- **Quick Access:** Can activate stored patterns as a bonus action instead of an action

### 5th Level

#### Environmental Attunement  
You become one with your surroundings:
- **Terrain Bond:** Choose one terrain type; gain the following while in that terrain:
  - +2 to AC from environmental awareness
  - Advantage on Stealth checks
  - Resistance to one damage type common to that terrain
- **Ecological Network:** Can communicate basic concepts to plants and animals in your bonded terrain

### 6th Level

#### Seeder Path Feature
Your chosen path grants additional abilities:

##### Path of the Explorer
- **Dimensional Pathfinding:** Can cast *misty step* once per short rest using xenocortex spatial mapping
- **Hazard Immunity:** Immunity to natural environmental hazards in familiar terrain

##### Path of the Cultivator
- **Accelerated Ecosystem:** Can create a 30-foot radius of enhanced plant growth that provides benefits
- **Life Network:** Can share health and status effects with bonded creatures

##### Path of the Inventor  
- **Xenocortex Interface:** Can mentally interface with compatible technology
- **Pattern Programming:** Can store spell-like effects as patterns (limited spell list)

### Higher Level Features

#### 9th Level - Master Adaptation
- **Universal Patterns:** Can adapt to any environment within 24 hours
- **Crisis Response:** Advantage on all checks during emergency situations

#### 13th Level - Xenocortex Mastery
- **Pattern Synthesis:** Can combine multiple patterns for powerful effects
- **Environmental Control:** Can alter small areas of terrain to suit needs

#### 17th Level - Pioneer's Legacy
- **Permanent Change:** Can make lasting improvements to environments
- **Pattern Teaching:** Can transfer patterns to other Vaarn or compatible xenocortex users

## AI Decision Making Preferences

### Combat Tactics
- **Primary Actions:** ["analyze_enemy", "environmental_advantage", "support_ally"]
- **Target Priority:** ["threatening_environment", "group_threats", "isolated_enemies"]  
- **Positioning:** Tactical positioning using environmental features
- **Risk Tolerance:** Moderate to high (calculated risks for group benefit)

### Exploration Focus
```ruby
def seeder_exploration_priority(environment_data)
  priorities = {
    "unknown_terrain" => 1.5,
    "natural_hazards" => 1.3,
    "resource_locations" => 1.4,
    "adaptation_opportunities" => 1.2
  }
  
  return priorities[environment_data[:primary_challenge]] || 1.0
end

def environmental_adaptation_response(threat_type)
  xenocortex_patterns = get_stored_patterns(:environmental)
  
  if xenocortex_patterns.include?(threat_type)
    return { action: "apply_pattern", confidence: 1.4 }
  else
    return { action: "analyze_and_adapt", confidence: 1.1 }
  end
end
```

## AI Personality Integration

- **Risk Averse:** Uses environmental knowledge for safe pathfinding
- **Risk Seeking:** Actively seeks new environments and challenges
- **Group Focused:** Prioritizes party survival and environmental advantage
- **Self Focused:** Uses adaptation for personal exploration goals

## Equipment Preferences

- **Weapons:** Versatile weapons that adapt to multiple situations
- **Armor:** Medium armor with environmental modifications
- **Tools:** Survival gear, environmental sensing equipment, xenocortex interfaces
- **Special:** Terrain-specific adaptations, growth acceleration devices

## Multiclassing Requirements

- **Minimum Scores:** Intelligence 13 and Wisdom 13
- **Proficiencies Gained:** Light armor, medium armor, herbalism kit

## Related Classes
- [[ranger]] - Similar environmental focus without xenocortex specialization
- [[druid]] - Nature magic vs technological/biological adaptation
- [[artificer]] - Invention overlap with different power source