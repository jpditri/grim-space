name:: Singer
type:: class
hit_die:: 6
primary_ability:: Charisma, Wisdom
saving_throw_proficiencies:: Wisdom, Charisma
skill_proficiencies:: 6
armor_proficiencies:: Light armor
weapon_proficiencies:: Simple weapons
spellcasting_ability:: Charisma
spell_list:: singer
xenocortex_class:: true
campaign:: [[kepharion]]
source:: [[Kepharion]] Campaign
last_updated:: 2025-07-02T16:30:00Z

- # Singer

- **Hit Die:** d6 per singer level
- **Primary Abilities:** Charisma and Wisdom
- **Saving Throw Proficiencies:** Wisdom, Charisma
- **Spellcasting:** Half caster using Charisma
- **[[Xenocortex]] Specialization:** Memory Archive and Empathic Resonance

- Singers are the lorekeepers, artists, and empathic heart of Vaarn society. They preserve memory, culture, and emotional well-being through specialized [[xenocortex]] memory storage and empathic harmonization abilities.

- ## Class Features

- ### 1st Level

- #### Hit Points
- **Hit Points at 1st Level:** 6 + Constitution modifier
- **Hit Points at Higher Levels:** 1d6 (or 4) + Constitution modifier per singer level after 1st

- #### Proficiencies
- **Armor:** Light armor
- **Weapons:** Simple weapons
- **Tools:** Three musical instruments of your choice
- **Saving Throws:** Wisdom, Charisma

- #### Skills
			- Choose 6 from: Deception, History, Insight, Investigation, Medicine, Performance, Persuasion, Religion

- #### Archive [[Xenocortex]]
			- Your [[xenocortex]] is specialized for memory preservation and empathic connection:
- **[[Xenocortex]] Rating increases by 1** at 1st level and again at 4th, 8th, 12th, 16th, and 20th levels
- **Memory Archive:** Can store unlimited memories with perfect fidelity; others can experience them through touch
- **Cultural Repository:** Double proficiency bonus on History and Religion checks related to Vaarn culture

- #### Empathic Harmonization
			- You can sense and influence emotional states:
- **Emotional Awareness:** Can sense the emotional state of creatures within 30 feet
- **Harmonic Stabilization:** As an action, can calm one creature within 30 feet (Charisma save negates)
- **Resonance Field:** Allies within 10 feet gain advantage on saving throws against fear and charm effects

- #### Spellcasting (Half Caster)
			- You can cast singer spells using Charisma as your spellcasting ability:
- **Spell Slots:** Use half-caster progression (like Paladin)
- **Spells Known:** Charisma modifier + half singer level (minimum 1)
- **Ritual Casting:** Can cast spells with ritual tag as rituals

- ### 2nd Level

- #### Memory Weaving
			- You can share and manipulate memories:
- **Memory Transfer:** Can share specific memories with willing creatures through touch
- **False Memory Detection:** Advantage on checks to detect altered or false memories
- **Memory Healing:** Can help restore lost memories damaged by trauma or magic (requires 1 hour)

- ### 3rd Level

- #### Singer's Path
			- Choose your specialization that shapes your [[xenocortex]] and abilities:

- ##### Path of the Lorekeeper
- **Living Archive:** Your [[xenocortex]] becomes a repository of vast cultural knowledge
- **Historical Insight:** Can access memories from previous generations stored in communal [[xenocortex]] fragments
- **Knowledge Network:** Can mentally connect with other Lorekeepers to share information

- ##### Path of the Healer
- **Empathic Mending:** Can heal psychological trauma and emotional wounds
- **Pain Resonance:** Can take on others' emotional or physical pain to heal them
- **Harmony Restoration:** Specialized in treating [[xenocortex]]/brain disharmony

- ##### Path of the Storyteller
- **Narrative Reality:** Can make stories feel so real they temporarily affect listeners
- **Inspiring Tales:** Can grant temporary bonuses through powerful storytelling
- **Mythic Resonance:** Can tap into archetypal stories stored in collective [[xenocortex]] memory

- ### 4th Level

- #### Ability Score Improvement
			- You can increase one ability score by 2, or two ability scores by 1. You can also choose a feat.

- #### Memory Mastery
			- Your [[xenocortex]] memory abilities expand:
- **Perfect Recall:** Can perfectly remember anything experienced in the last year per character level
- **Memory Search:** Can quickly locate specific memories or information in your [[xenocortex]]
- **Memory Fortification:** Immunity to memory-altering magic and effects

- ### 5th Level

- #### Song of Power
			- Your voice gains supernatural influence:
- **Harmonic Spell:** Can cast spells through song, making them harder to counterspell (+2 to spell save DC)
- **Mass Harmonization:** Your empathic abilities now affect all creatures within 30 feet
- **[[Xenocortex]] Chorus:** Can link with other Singers to amplify spellcasting (group casting)

- ### 6th Level

- #### Singer's Path Feature
			- Your chosen path grants additional abilities:

- ##### Path of the Lorekeeper
- **Ancestral Wisdom:** Can access ancient memories stored in deceased xenocortices
- **Knowledge Synthesis:** Can combine disparate information to gain new insights
- **Living Library:** Other creatures can access your stored knowledge through touch

- ##### Path of the Healer
- **Emotional Surgery:** Can precisely remove traumatic memories or implant therapeutic ones
- **Empathic Link:** Can establish permanent emotional bonds for healing purposes
- **Mind Bridge:** Can temporarily merge consciousness to provide direct healing

- ##### Path of the Storyteller
- **Reality Weaving:** Stories you tell can temporarily alter local reality in minor ways
- **Character Summoning:** Can temporarily manifest story characters as illusory helpers
- **Narrative Prophecy:** Can predict likely futures through archetypal story patterns

- ### Higher Level Features

- #### 9th Level - Cultural Resonance
- **Community Memory:** Can access and contribute to collective Vaarn cultural memory
- **Harmonic Mastery:** Can influence large groups through [[xenocortex]]-enhanced performance

- #### 13th Level - Memory Immortality  
- **[[Xenocortex]] Backup:** Can create permanent memory copies in crystal matrices
- **Consciousness Transfer:** Can temporarily place consciousness in other compatible xenocortices

- #### 17th Level - Living Legend
- **Mythic Status:** Your stories and memories become part of Vaarn cultural mythology
- **Reality Anchor:** Can make temporary story effects permanent through collective belief

- ## Singer Spell List

- ### Cantrips (0 Level)
- Guidance, Light, Mending, Minor Illusion, Prestidigitation, Thaumaturgy

- ### 1st Level
- Bless, Charm Person, Comprehend Languages, Cure Wounds, Detect Magic, Identify

- ### 2nd Level  
- Calm Emotions, Detect Thoughts, Hold Person, Lesser Restoration, Suggestion, Zone of Truth

- ### 3rd Level
- Clairvoyance, Counterspell, Dispel Magic, Hypnotic Pattern, Mass Healing Word, Tongues

- ### 4th Level
- Confusion, Dominate Beast, Greater Invisibility, Locate Creature, Modify Memory

- ### 5th Level
- Dominate Person, Geas, Greater Restoration, Legend Lore, Mass Cure Wounds, Scrying

- ## AI Decision Making Preferences

- ### Combat Tactics
- **Primary Actions:** ["support_ally", "heal_wounded", "crowd_control"]
- **Target Priority:** ["allies_needing_support", "mind_affecting_enemies", "group_threats"]
- **Positioning:** Safe distance while maintaining empathic range
- **Risk Tolerance:** Low (preserve self to preserve knowledge)

- ### Social Interaction Focus
		- ```ruby
		- def singer_social_approach(situation)
		- empathic_reading = assess_emotional_state(situation[:participants])
  
- if empathic_reading[:high_tension]
- return { action: "harmonic_stabilization", priority: "de_escalate" }
- elsif empathic_reading[:deception_detected]
- return { action: "memory_verification", priority: "truth_seeking" }
- else
- return { action: "empathic_connection", priority: "relationship_building" }
- end
- end

- def memory_sharing_decision(requester, memory_type)
- cultural_value = assess_cultural_importance(memory_type)
- trust_level = assess_relationship(requester)
  
- return cultural_value > 0.7 && trust_level > 0.5
- end
- ```

- ## AI Personality Integration

- **Risk Averse:** Prioritizes preservation of knowledge and cultural memory
- **Risk Seeking:** May risk danger to recover lost knowledge or help others
- **Group Focused:** Strong emphasis on community harmony and collective memory
- **Self Focused:** Balances personal knowledge accumulation with sharing duties

- ## Equipment Preferences

- **Weapons:** Simple weapons, often ceremonial or cultural significance
- **Armor:** Light armor that doesn't interfere with performance or [[xenocortex]] function
- **Tools:** Musical instruments, memory storage crystals, harmonic resonators
- **Special:** [[Xenocortex]] memory interfaces, communal archive access devices

- ## Multiclassing Requirements

- **Minimum Scores:** Charisma 13 and Wisdom 13
- **Proficiencies Gained:** Light armor, one musical instrument

- ## Related Classes
- [[bard]] - Similar performance and knowledge focus
- [[cleric]] - Healing and community service overlap
- [[enchantment-wizard]] - Mind affecting magic similarities